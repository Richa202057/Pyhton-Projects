def printBoard(xState,zState):  #passing two lists to this function
    print("{} | {} | {}".format( "X" if xState[0] else "0" if zState[0] else 0,"X" if xState[1] else "0" if zState[1] else 1,"X" if xState[2] else "0" if zState[2] else 2))
    print("__|___|__")
    print("{} | {} | {}".format( "X" if xState[3] else "0" if zState[3] else 3,"X" if xState[4] else "0" if zState[4] else 4,"X" if xState[5] else "0" if zState[5] else 5))
    print("__|___|__")
    print("{} | {} | {}".format( "X" if xState[6] else "0" if zState[6] else 6,"X" if xState[7] else "0" if zState[7] else 7,"X" if xState[8] else "0" if zState[8] else 8))
def sum(a,b,c):
    return a+b+c
def checkWin(xState,zState):
    wins=[[0,1,2],[3,4,5],[6,7,8],[0,3,6],[1,4,7],[2,5,8],[0,4,8],[2,4,6]]# all possible combinations of lists of indixes to winning a team
    for win in wins:# here win is also a list
        if(sum(xState[win[0]],xState[win[1]],xState[win[2]])==3):# doing the sum of all 3 elements of list win ## this loop checks for every list win that this condition is true or not for xState list
            print("X win's the match")
            return 1
        if(sum(zState[win[0]],zState[win[1]],zState[win[2]])==3):# doing the sum of all 3 elements of list win ## this loop checks for every list win that this condition is true or not for zState list
            print("0 win's the match")
            return 0
    return -1




if __name__=="__main__":
    xState=[0,0,0,0,0,0,0,0,0]
    zState=[0,0,0,0,0,0,0,0,0]
    print("welcome to tic-toc-toe Game")
    printBoard(xState,zState)
    turn=1
    while(True):
        if turn==1:
            print("X's Chance :")
            value=int(input("Enter position: "))
            xState[value]=1
        else :
            print("0's Chance :")
            value=int(input("Enter position: "))
            zState[value]=1
        printBoard(xState,zState)
        #before going for the next round,  check that if anyone is winner or not by checking current xState aur zState list values
        #for this we have created checkWin function
        if(checkWin(xState,zState)!=-1):
            #it means it have returned either 0 or 1 it means winner has been selected so, break the loop and stop the game
            print("Game is Over")
            break

        turn=not(turn) # so that next iteration another team will grt chance.     

