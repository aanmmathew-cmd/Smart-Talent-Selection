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

### For C
#include <stdio.h>
#include<string.h>

int main() {
    int n, i;

    printf("Enter number of candidates: ");
    scanf("%d", &n);

    char name[50];
    int marks, experience;
    float score, maxScore = 0;
    char bestName[50];

    for(i = 1; i <= n; i++) {
        printf("\nCandidate %d\n", i);

        printf("Enter name: ");
        scanf("%s", name);

        printf("Enter marks: ");
        scanf("%d", &marks);

        printf("Enter experience: ");
        scanf("%d", &experience);

        // Calculate score
        score = marks * 0.7 + experience * 0.3;

        printf("Score of %s = %.2f\n", name, score);

        // Find best candidate
        if(score > maxScore) {
            maxScore = score;
            strcpy(bestName, name);
        }
    }

    printf("\nSelected Candidate: %s", bestName);
    printf("\nBest Score: %.2f\n", maxScore);

    return 0;
}


##Team Member
Ann Mariya Mathew






