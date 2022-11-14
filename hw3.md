# CShape.java
```JAVA        
abstract class CShape{
    protected String color;
    public void setColor(String str){
        color = str;
    }
    public abstract void show();
}
```
# CTriangle.java
```JAVA           
class CTriangle extends CShape{
    double a1, b1, c1;
    public CTriangle(double a, double b, double c){
        a1=a;
        b1=b;
        c1=c;
    }
   
    public void show() {
       
        System.out.print("color="+color+"  ");
        System.out.print("area="+0.5*a1*b1);
    }
   
}
```
# app11.java
```JAVA
public class app11 {
   public static void main(String[] args) {
    CTriangle t1 = new CTriangle(3, 4, 5);
    t1.setColor("red");
    t1.show();
}
}

```
