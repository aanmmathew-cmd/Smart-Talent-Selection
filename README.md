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

int main() {
    int n, i;
    
    printf("Enter number of candidates: ");
    scanf("%d", &n);

    char name[n][50];
    int marks[n], experience[n];
    float score[n];

    // Input details
    for(i = 0; i < n; i++) {
        printf("\nCandidate %d\n", i + 1);

        printf("Enter name: ");
        scanf("%s", name[i]);

        printf("Enter marks (out of 100): ");
        scanf("%d", &marks[i]);

        printf("Enter experience (years): ");
        scanf("%d", &experience[i]);

        // Simple scoring formula
        score[i] = marks[i] * 0.7 + experience[i] * 0.3;
    }

    // Display results
    printf("\n--- Candidate Scores ---\n");
    for(i = 0; i < n; i++) {
        printf("%s -> Score: %.2f\n", name[i], score[i]);
    }

    // Find best candidate
    int best = 0;
    for(i = 1; i < n; i++) {
        if(score[i] > score[best]) {
            best = i;
        }
    }

    printf("\n Selected Candidate: %s with score %.2f\n", name[best], score[best]);

    return 0;
}


##Team Member
Ann Mariya Mathew






