    # union-of-two-sorted-array-  
     class Solution {
     public:
     
             vector<int> unionArray(vector<int>& nums1, vector<int>& nums2) {
             set<int>st;
             for(int i = 0; i<nums1.size();i++){
              st.insert(nums1[i]);
    }
    
    for(int i = 0; i< nums2.size();i++){
        st.insert(nums2[i]);
    }
    
    vector<int>temp;
    for(auto it : st){
    temp.push_back(it);
    }
    
    return temp;
    }
};
