# Task
#include<iostream>
using namespace std;
int main() {
    int n;
    float cost, discountedCost, totalRevenue = 0;

    cout << "Enter number of houses: ";
    cin >> n;

    for(int i = 1; i <= n; i++) {
        cout << "Enter cost for house " << i << ": ";
        cin >> cost;
        if(cost > 2200) {
            discountedCost = cost - (cost * 0.10);  // 10% discount
        } else {
            discountedCost = cost;
        }
        totalRevenue += discountedCost;
        cout << "Discounted cost for house " << i << ": " 
             << discountedCost << endl;
    }

    cout << "\nTotal Revenue from all houses = " << totalRevenue << endl;

    return 0;
}
