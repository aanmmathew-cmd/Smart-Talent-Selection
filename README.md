# Smart-Talent-Selection Engine
##  Overview
A system designed to simplify the hiring process by automatically selecting the best candidates based on predefined criteria.

## Problem Statement
Recruiters face difficulty handling large numbers of applications manually, leading to time consumption and errors.

##  Solution
This project automates candidate evaluation using logic-based filtering and ranking, helping companies make faster decisions.

##  Features
-  Candidate Filtering  
-  Ranking System  
-  Fast Processing  
-  Smart Decision Logic  

## How It Works
1. Input candidate details  
2. Apply selection criteria  
3. Rank candidates  
4. Display best results  

##  Technologies Used
- C Programming / Python  
- Basic Algorithms  

## How to Run

### For C:

#include<stdio.h>
int main()
{
int n,i;
printf("Enter the number of candidates:");
scanf("%d",&n);
int exp[n],skill[n],score[n];
char name[n][50];

#input Details
for(i=0;i<n;i++)
{
printf("\n Candidate %dName:",i+1)
scanf("%s",name[i]);
printf("experience: ");
scanf("%d",&exp[i]);
printf("skill score(0-100):");
scanf("%d",&skill[i]);
}
int req-exp,req-skill;
printf("\n Enter required experience:");
scanf("%d",&req-exp);
printf("\n Enter required skill score:");
scanf("%d",&req-skill);
for(i=0;i<n;i++)
{
    score[i]=(exp[i]*10)+skill[i]
}
#Find Best Candidate 
int max=0;
for(i=1;i<n;i++)
{
if(score[i]>score[max])
{
    max=i;
}
}
#Output 
printf("\nest Candidate:\n");
printf("Name:%s\n",name[max]);
printf("Score:%d\n",score[max]);
return 0;
}

##Team Member
Ann Mariya Mathew






