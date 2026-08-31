class Solution {
public:
    vector<int> twoSum(vector<int>& nums, int target) {

        for(int i = 0; i < nums.size(); i++) {

            for(int j = i + 1; j < nums.size(); j++) {

                if(nums[i] + nums[j] == target) {
                    return {i, j};
                }

            }
        }

        return {};
    }
};
int main() {
    vector<int> arr = {5, 3, 1, 4, 2};

    sort(arr.begin(), arr.end());

    for(int x : arr) {
        cout << x << " ";
    }

    return 0;
}
