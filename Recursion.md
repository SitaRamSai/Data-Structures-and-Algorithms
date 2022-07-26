## How recursion uses stack

 Basic recursive function:

    Class main(){
    
      void recur(int x) {

        if(x > 0) {

         sout(x);

         recur(x -1);
        }
      }
            
      public void main(String[] args){
        
        int x = 3;
        
        recur(x);
      
      }
    }
 
 ### For the above function, if we take a stack and demonstate:
 
   ![Recursion-using-Stack drawio (1)](https://user-images.githubusercontent.com/57385355/180911442-849b1922-4eea-4b69-89ca-557e95ad7849.png)


- Every recursive call is adding a new activation record in the stack
- Once the condition is met, the stack is no longer updated. 
- Now for every recursive call that comes out of the function, the activation record is deleted from the stack.


## Analysing Number of calls and memory consumption

- For a value of x we are creating x+1 activation records, Ex: for x = 3 -> 3, 2, 1, 0
  - So for any value of N there will be N+1 calls 

- For N number of values, the memory consumed will be O(N)

  
  
  
