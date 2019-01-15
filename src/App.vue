<template>
  <div id="app">
		<div class="container">
    <template>
				<Card>
					<div class="demo-split">
							<Split v-model="split1" mode="vertical">
									<div slot="top" class="demo-split-pane">
											<h1 style="font-family: '楷体';">基本信息</h1>
									</div>
									<div slot="bottom" class="demo-split-pane">
										<Split v-model="split2">
											<div slot="left" class="demo-split-pane">
													<div class="pic">
														<img src="./images/12170953.jpg" />
													</div>
											</div>
											<div slot="right" class="demo-split-pane">
													<Split v-model="split3">
														<div slot="left" class="demo-split-pane">
																<h3>姓名：朱茂琛</h3>
																<h3>籍贯：江西赣州</h3>
																<h3>身高：175cm</h3>
																<h3>电话：13169617210</h3>
																<h3>求职意向：Java后台开发</h3>
														</div>
														<div slot="right" class="demo-split-pane">
																<h3>年龄：20岁</h3>
																<h3>体重：55kg</h3>
																<h3>学历：本科</h3>
																<h3>毕业院校：暨南大学</h3>
																<h3>E-mail：1226823745@qq.com</h3>
														</div>
													</Split>
											</div>
										</Split>
									</div>
							</Split>
					</div>
				</Card>
		</template>
		</div>
		
		<div class="container">
			<template>
					<Card>
						<div class="demo-split">
							<Split v-model="split4" mode="vertical">
									<div slot="top" class="demo-split-pane">
											<h1 style="font-family: '楷体';">专业技能</h1>
									</div>
									<div slot="bottom" class="demo-split-pane">
											<h3>核心技术：熟练掌握Java编程语言，Java并发编程。</h3>
											<h3>前端技术：熟练编写HTML,CSS,JavaScript并且熟练JQuery体系和VUE前端框架。</h3>
											<h3>数据存储：熟练使用SQL Server、MySQL关系型数据库和NoSQL的Redis进行数据库开发。</h3>
											<h3>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;熟练掌握并使用SQL语言进行对数据库的操作，设计。</h3>
											<h3>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;熟练编写储存过程。</h3>
											<h3>框架方面：熟练掌握SSM三大框架，Spring Boot 框架。</h3>
											<h3>后台技术：熟练AOP编程，构造者模式，工厂模式，单例模式以及Apache Shiro 验证技术</h3>
											<h3>开发工具：熟练应用eclipse,InterlliJ IDEA,Dreamweaver,HBuilder主流开发工具</h3>
									</div>
							</Split>
						</div>
					</Card>
			</template>
		</div>
		
		<div class="container">
			<template>
					<Card>
						<div class="demo-split">
							<Split v-model="split4" mode="vertical">
									<div slot="top" class="demo-split-pane">
											<h1 style="font-family: '楷体';">自我评价</h1>
									</div>
									<div slot="bottom" class="demo-split-pane">
											<h3>学习上：勤奋刻苦、认真好学、自学能力强、能不断地充实自己的专业知识，并主动吸收新知识。</h3>
											<h3>生活上：活泼开朗、乐观向上、兴趣广泛、爱好打篮球；适应能力强、坚韧不拔、吃苦耐劳、</h3>
											<h3>&nbsp;&nbsp;&nbsp;&nbsp;勇于迎接新挑战；有良好的沟通能力，在学校有良好的人际关系。</h3>
											<h3>工作上：具备较强的团队管理能力，独立问题解决能力和较强的执行能力，具备抗压能力，</h3>
											<h3>&nbsp;&nbsp;&nbsp;&nbsp;责任心强，乐于助人，具备良好的沟通能力和团队合作意识。</h3>
									</div>
							</Split>
						</div>
					</Card>
			</template>
		</div>
	
		<div class="container">
			<template>
					<Card>
						<div class="demo-split">
							<Split v-model="split4" mode="vertical">
									<div slot="top" class="demo-split-pane">
											<h1 style="font-family: '楷体';">项目经历</h1>
									</div>
									<div slot="bottom" class="demo-split-pane">
										<h3>敬请期待</h3>
											<!-- <h3>项目名称：新淘购物</h3>
											<h3>项目职位：担任项目组长</h3>
											<h3>责任描述：在该项目中主要负责数据层，管理数据和表示层的编码工作</h3>
											<h3>功能介绍：主要为了方便用户在网上购买新鲜食物，然后通过“支付宝”实现在线支付</h3>
											<h3>开发周期：2017.10-2018.01</h3>
											<h3>开发工具：Eclipse+HBulider+Photoshop</h3> -->
									</div>
							</Split>
						</div>
					</Card>
			</template>
		</div>
	</div>
</template>

<script>
    export default {
        
    }
</script>

</template>

<script>
    export default {
        data () {
            return {
                split1: 0.2,
								split2: 0.3,
								split3: 0.4,
								split4: 0.2
            }
        },
    }
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
.container{
	margin-top: 20px;
	margin-bottom: 20px;
}
.skill-title{
	text-align: left;
	font-family: "楷体";
}
.ivu-card{
	width: 900px;
	margin: 0px auto;
}
.pic > img{
	width: 180px;
	height: 180px;
}
.demo-split{
		height: 300px;
}
.demo-split-pane{
		padding: 10px;
}
.demo-split-pane > h1{
	width: 120px;
	border-radius: 5px;
	background-color: #000000;
	color: #FFFFFF;
}
.demo-split-pane > h3{
	margin-bottom: 10px;
	font-family: "新宋体";
}
.demo-split-pane.no-padding{
		height: 200px;
		padding: 0;
}
.ivu-split-trigger-con{
	height: 0px;
	display: none;
}
.top-pane{
	height: 50px;
	text-align: left;
}
.bottom-pane{
	text-align: left;
}

</style>
