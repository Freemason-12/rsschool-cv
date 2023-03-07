#Maksat Rsymbetov

##Contact me:
* *Email:* maksatlego@gmail.com
* *Main GitHub Account:* https://github.com/Freemason-12
* *Second GitHub Account:* https://github.com/Maksat-Rsymbetov

##About me
Student of Suleyman Demirel University, hobbyist, Linux power user, likes drawing, 3D modelling, design, coding and solving problems.

##Skills
 * Java
 * Go (basic)
 * JavaScript 
 * Python (basic)
 * HTML 
 * CSS 
 * Blender 
 * Linux, Vim

##Code Example
example of Java code
```
class Solution {
    public String longestPalindrome(String s) {
        int l = s.length();
        ArrayList<String> ans = new ArrayList<String>();
        
        ans.add(s.substring(0,1));
        
        for(int i = 0; i < l - 1; i++){
            if(s.charAt(i) == s.charAt(i + 1)){
                for(int st = i, en = i + 1; st >= 0 && en < l; st--, en++){
                    if(s.charAt(st) != s.charAt(en)) {ans.add(s.substring(st + 1, en)); break;}
                    else if(st == 0 || en == l - 1){ans.add(s.substring(st, en + 1)); break;}
                }
            }
        }
        
        for(int i = 0; i < l - 2; i++){
            if(s.charAt(i) == s.charAt(i + 2)){
                for(int st = i, en = i + 2; st >= 0 && en < l; st--, en++){
                    if(s.charAt(st) != s.charAt(en)) {ans.add(s.substring(st + 1, en)); break;}
                    else if(st == 0 || en == l - 1){ans.add(s.substring(st, en + 1)); break;}
                }
            }
        }
        
        String answer = "";
        for(String p: ans) if(p.length() > answer.length()) answer = p;
        return answer;

    }
}
```

##Work Experience
Currently working as a teacher at CRTL+A School

###Projects
* *Minesweeper game:* a traditional minesweeper 8x8 game written in JavaScript
  _GitHub source code: https://github.com/Maksat-Rsymbetov/SENSEI_

*English level:* B2
