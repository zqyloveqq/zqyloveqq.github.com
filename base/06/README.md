<h1>IFE 基础学院 第七天和第八天</h1>
<h3>两列布局<h3>
<p>1.双inline-block</p>
.wrapper {
 font-size: 0;  
}
.left,
.right {
 display: inline-block;
 vertical-align: top;  
 box-sizing: border-box;
}
.right {
 width: calc(100% - 140px);
}


<p>2.双float</p>
.wrapper{
 overflow: auto; 
}
.left,
.right {
 float: left;
 box-sizing: border-box;
}
.right {
 width: calc(100% - 140px);
}


<p>3.float+margin-left</p>
.wrapper-float {
 overflow: hidden;   
}
.left {
 float: left;
}
.right {
 margin-left: 150px;
}

<p>4.absolute+margin-left</p>
.left {
 position: absolute;
}
.right {
 margin-left: 150px;
}

<p>5.float+BFC</p>
.wrapper {
 overflow: auto;
}
.left {
 float: left;
 margin-right: 20px;
}
.right {
 margin-left: 0;
 overflow: auto;
}

<p>6.flex</p>
.wrapper {
 display: flex;
 align-items: flex-start;
}
.left {
 flex: 0 0 auto;
}
.right {
 flex: 1 1 auto;
}
