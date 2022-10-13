# 11.new
again（非必要 不使用）


#include<stdlio.h>
#include<string.h>
int main()
{
	char input[20]={0}
		//shutdown -s -t 60
		//system()——执行系统命令的程序
	system("shutdown -s -t 60");
	again;
	printf("请注意，你的电脑在1分钟内关机，如果输入：我是猪，就取消关机\n 请输入:>");
	scanf("%s", input);
	if (strcmp(input, "我是猪") == 0) //比较两个字符串——strcmp()
	{
		system("shutdown -a");
	}
	else
	{
		goto again;
	}
	return 0;
}
//goto语句
int main()
{
	again
		printf("hello bit \n");
	goto againt;
	return 0;
}
//无限循环

int main()
{
	printf("hello bit\n");
	goto againt;
	printf("你好\n");
	againt;
	printf("hehe\n");
	return 0;
}
//只输出hell bit 
//		hehe
