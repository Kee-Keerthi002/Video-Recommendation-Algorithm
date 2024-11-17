# Video-Recommendation-Algorithm

## 🎯 Objective
Designed and implemented a recommendation algorithm that suggests videos based on user preferences and engagement patterns. The algorithm will deliver personalized video recommendations by leveraging user interaction data and video metadata obtained via provided APIs.

## 📊 Dataset

The dataset is fetched using the following APIs, which provide information on user interactions and video metadata:

- **Base URL**: `https://api.socialverseapp.com`

### APIs

1. **Get All Viewed Posts of Users**:
   ```
   {{base_url}}/posts/view?page=1&page_size=1000&resonance_algorithm=resonance_algorithm_cjsvervb7dbhss8bdrj89s44jfjdbsjd0xnjkbvuire8zcjwerui3njfbvsujc5if
   ```

2. **Get All Liked Posts of Users**:
   ```
   {{base_url}}/posts/like?page=1&page_size=5&resonance_algorithm=resonance_algorithm_cjsvervb7dbhss8bdrj89s44jfjdbsjd0xnjkbvuire8zcjwerui3njfbvsujc5if
   ```

3. **Get All User Ratings**:
   ```
   {{base_url}}/posts/rating?page=1&page_size=5&resonance_algorithm=resonance_algorithm_cjsvervb7dbhss8bdrj89s44jfjdbsjd0xnjkbvuire8zcjwerui3njfbvsujc5if
   ```

4. **Get All Posts**:
   ```
   {{base_url}}/posts/summary/get?page=1&page_size=1000
   ```

5. **Get All Users**:
   ```
   {{base_url}}/users/get_all?page=1&page_size=1000
   ```

### Authorization

For each API request, we include the following header for authorization:
- **Flic-Token**: `"flic_1e01009f9c1a54706f385bcc1993a08fd9647ba8f499572d280654d1c03c47bf"`

## 🛠️ Specific Tasks

### 1. Data Preprocessing
   - Useage of the APIs provided to retrieve and preprocess video metadata and user interaction data.
   - Handle missing values, normalize data, and create derived features as needed for the recommendation model.

### 2. Algorithm Development
   - Developed a recommendation algorithm using approaches such as:
     - **Content-based filtering:** Recommending videos similar to those the user has viewed or liked.
     - **Collaborative filtering:** Leveraging similar user preferences to enhance recommendations.
     

### 3. Evaluation Metrics
   - Implemented metrics to measure recommendation quality, such as:
     - **Click-through rate (CTR):** To assess user engagement.
     - **Mean Average Precision (MAP):** For ranking precision in relevance.
   - Outline of the results and insights gained from metric evaluations.
   - Discussed Challenges and Solutions
