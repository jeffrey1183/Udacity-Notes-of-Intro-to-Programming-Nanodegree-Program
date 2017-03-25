## **2.7 How to solve problem**

### **Make sure to understand question**

#### **computational problem**

![](https://lh4.googleusercontent.com/KQs2J-n5hALkeEPIO-l_8FrIG_COPGYbF_ujtru8QcI8uwFrytP3azVexAzI5uZg4eH-L4AvRLhhQO8SpA2vsUHxGI-AbcX5xrNykpcmXszMvVF5p1TOYdkx-GTMkNteBG48CBgU)

**  
**

![](https://lh4.googleusercontent.com/BLNzFNoXrEUWwMVX6swpWMKpQUie6HY0HERfAo4cMMTG327R70cXz59442zYh4FjT4u0QHSvtbMRlU5SxJruyFZnpMBKPF_6S6CSuqPwMi8GhG030pK7EBuOesEsWKS6IiN45joW)

**  
**![](https://lh5.googleusercontent.com/89jvKw1lztSYhmMLqU9FfLYPgf5fyqxDMWyXqu7Lo9y-Porw0w9L2bP4acL_HKYNE9VwMUAWvcX2pvuuLLOLdnaiwICMGFf6ZNZpkRbxh-nmsFnqdkpGQF4ualYjMvLSvl5iKxtB)

![](https://lh4.googleusercontent.com/FzjA4ZZ5pMVIt9ZJKICXnTO3TUtPPPyzJmLlHisIjMH-JrldqSZJmrzSpudnUinmsAZ6jROn45MwDOYeiDAXR8128e_TH9fvTF29Se5tfo_7C9udQvnMThWT74T_NkOVJvNi4fWk)



**  
**

**  
**

### **3. Work out examples**

![](https://lh3.googleusercontent.com/bu9Es_xDgGaDKmUBprv76X2WUkp4dGvbRWK_uyHb9f1yTqK0HJey_Am-ByeUyC-sPVgPcrtIVFgVgoFOhTyFReqdcaDbLwZKD8GWrrpDI08IHLgrOYGpPsrH-gA902kmwz2lqAv_)

**  
**

### **人類是怎麼想的？**

![](https://lh5.googleusercontent.com/zkogB_YCQpF5v4B3bvnegIy6KuBsHtvkVR6RYk40doz5vIkg-Jdtesvctj9S0CMqfylsOGeCGFoV3fkCZ0NvT1Pk8AW4YMYQnuHba10cCbOc48yJjiKoJ45Yh79vo9Q1Q0FvuIbP)

**  
**

**拿出月曆算**

  
**  
**

![](https://lh4.googleusercontent.com/ORGHxKXUZIOzmb5SMTU_Cwk7B3gKk3e9V5npSYfwyyQ8rZiVw2l23flRQcilH6uCh_wNvT8_DmRZ5ClYnxTFXt1ScootzWhLZ6w_VPWB248zQIFuUi5onDQPDF316yPKikBZsGYM)

**遇上年就不好算**

![](https://lh3.googleusercontent.com/Or-XVSmAn1xLhJAJoMC7S7iaell0tdzC70vog9NQzJWOchRjXuldasfrDXJYvxsXdtlhR7IbEmBKTlT_mO6H7TWzllM5YkIJF937IwxKqsgmQo0LGQmzXfZzja7KOAx-KSAcxyYv)

**  
**

**假設psuedo code（不管細節，寫的對不對），判斷能不能用**

**不要太複雜**

[**https://www.udacity.com/course/viewer\#!/c-nd000/l-4184188665/e-108281762/m-108325396**](https://www.udacity.com/course/viewer#!/c-nd000/l-4184188665/e-108281762/m-108325396)

**有什麼還沒處理的**

[**https://www.udacity.com/course/viewer\#!/c-nd000/l-4184188665/e-108281762/m-108325397**](https://www.udacity.com/course/viewer#!/c-nd000/l-4184188665/e-108281762/m-108325397)

**  
**

**提出另一個簡單的方法，一個一個算**

[**https://www.udacity.com/course/viewer\#!/c-nd000/l-4184188665/m-108325398**](https://www.udacity.com/course/viewer#!/c-nd000/l-4184188665/m-108325398)

**  
**

**再問一個問題，這個方法對電腦來說花費的時間？**

**1 billion instruction per sec = 1 nano second per instruction**

**  
**

[**https://www.udacity.com/course/viewer\#!/c-nd000/l-4184188665/e-108281763/m-108325401**](https://www.udacity.com/course/viewer#!/c-nd000/l-4184188665/e-108281763/m-108325401)

  
**  
**

**到底要先解決哪一個問題？**

**  
**

**  
**

**先做 nextDay\(\)，把下一天的方程式寫出來**

**  
**

**  
**

**繼續來思考 daysBetweenDates**

**要解決這個複雜的問題，要分成幾個步驟：**

**  
**

### **Solution in Three Parts**

**Well done for getting this far! The solution to this problem is broken down into three parts:**

**1\)Step One Pseudocode**

![](https://lh4.googleusercontent.com/Lz0b0FE_-shhG-9abetDi6iFB_mMIwKaUCheM_uR9TH1crTG4vL8LWpYS506UkEeaoxLFChWyfGa6gol-FBmlqO-lO25aiH11VhMyl3XVcqU6jzmrByxAB8ZgxidhVjqJYBDX_0K)

**2\)Step Two Helper Function**

**生出第一個 dateIsBefore**

  
![](https://lh5.googleusercontent.com/MhE_NMZkpMS5KpNG-MHqQvlKaJKdpo_c45vaowLtyirL0u5Ll2xEwCBHJPQ_fcJ3PuCihXLIkT984-EXagJmw_CuxlS6zinCUUUOc39fvM3JpCLzhnZhDNpvf58HOWkOi6Gc3l93)

**  
**

**3\)Step Three daysBetweenDates**

![](https://lh4.googleusercontent.com/9hRpKZBIT0wYZ8tuTbkiLwA5VJYv0xZUNiv7NqPwPi8sFgKR-vrShmWnBcjnnrc7GWlQMK1TLaB7RQ1CT2lwzW_6ftOPISdey7ckkM0dMF3OCZ5vgkSGqRcjQ_QmbAhsGSZ__t_2)

**  
**

**使用 assert 處理前面的input 如果比較大怎麼辦**

![](https://lh3.googleusercontent.com/cbrX_VAb0QLhEl140k_Wt37w9RFLPuhHmtxdXODaZ0lbXxFwBSeZhAG3nk14SdmuAO-fLghRpmF8lwUA2BnhHFSeA2gzYNIkIZvRmtHdjMHa2J1ieJSnRU_MbWsq5HfZHpMdo-a_)

**如果結果不是 assert 的這樣，結果就 GG**

**  
**

## **接著解決一個月不是30天的設定**

**寫一個程式daysInMonth去戳他，先修正nextDay，測試一下nextDay**

**  
**

**  
**

**  
**

**寫 isLeapyear，找出Leapyear的規則，調整入daysInMonth 測試Leapyear方程式**

**  
**

**  
**

**然後就可以來測daysBetweenDates**

**  
**![](https://lh6.googleusercontent.com/Z5EFZ0IMMHepubLQE_tPryB80x-JGYmKzjOROj8j9YrMKAQqU6KXzMl9lpZJC2bf7lSQJDKL6nqVgKxvDAcJHuoPxWS2Qbqth61k7Hq8kD3MZiMnMHFybAPLYN8DB07v_oIiFcoO)

**  
**

**  
**





