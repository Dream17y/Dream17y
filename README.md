i = 3  # 循环次数
while i >= 1: 
    Account = input('请输入账号')  # 变量
    code = input('请输入密码') 
    if Account != 'admin' or code != '123456':  #验证是否与数据库中相同
        print('账号或密码错误')        
        i -= 1
        print('剩余{}次认证机会'.format(i))
    else:
        print('登入成功')
