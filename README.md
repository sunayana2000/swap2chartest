public class Task {
public String swap(String result) {
int l=result.length();
char a=result.chatAt(0);
char b=result.charAt(1);
if(a=='A' && b!='A') {
result = result.substring(1,1);
}
else if(a=='A' && b=='A') {
result= result.substring(2,1);
}
else(b=='A' && a! = 'A') {
result = result.charAt(0)+result.substring(2,1);
}
return result;
}
}

import static org.junit.jupitar.api.Assertions.*;
class Swap2charTest {
@Test
void test1() {
Task s= new Task();
String actual = s.swap("ABCD");
assertEquals("BCD",actual);
}
@Test
void test2() {
Task s= new Task();
String actual = s.swap("AACD");
assertEquals("CD",actual);
}
@Test
void test3() {
Task s= new Task();
String actual = s.swap("BACD");
assertEquals("BCD",actual);
}
@Test
void test4() {
Task s= new Task();
String actual = s.swap("BBAA");
assertEquals("BBAA",actual);
}
@Test
void test5() {
Task s= new Task();
String actual = s.swap("AABAA");
assertEquals("BAA",actual);
}
}
