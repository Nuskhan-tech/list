if __name__ == '__main__':
    arr=[]
    N = int(input())
    for _ in range (N):
        cmd=map(str,input().split())
        cmd_list=list(cmd)
        if cmd_list[0]=='insert':
            arr.insert(int(cmd_list[1]) , int(cmd_list[2]))
        elif cmd_list[0]=='print':
            print(arr)
        elif cmd_list[0]=='remove':
            arr.remove(int(cmd_list[1]))
        elif cmd_list[0]=='append':
            arr.append(int(cmd_list[1]))
        elif cmd_list[0]=='sort':
            arr.sort()
        elif cmd_list[0]=='pop':
            arr.pop()
        elif cmd_list[0]=='reverse':
            arr.reverse()
