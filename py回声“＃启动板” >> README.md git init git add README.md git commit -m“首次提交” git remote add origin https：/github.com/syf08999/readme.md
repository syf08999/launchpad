def getInput():
    try:
        txt = input("请输入整数：")
        while eval(txt) != int(txt):
            txt = input("")
    except:
        return getInput()
    return eval(txt)
print(getInput())
