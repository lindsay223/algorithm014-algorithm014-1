学习笔记

递归：
	代码模板：
	public void recursion(int level,int param){
		//terminator
		if(level > MAX){
			return;
		}
		//process current logic
		process(level,param);
		//drill down
		recursion(level+1, newParam);
		//revert status
	}
	思维要点：
	1.不要人肉递归
	2.找到重复子问题
	3.数学归纳法：n=1,n=2时成立，当n成立时， n+1 成立
	
分治/回溯： 递归
	代码模板：
	public void recursion(int level,int param){
		//terminator
		if(level > MAX){
			return;
		}
		//process current logic
		process(level,param);
		//drill down
		recursion(level+1, newParam);
		//merge subsult
		merge(subsult);
		//revert status
	}
