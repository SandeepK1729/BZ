# BackTracking

Steps
- add current
- move required directions
- remove current


```
void backtrack(int i, int j, vector<int> path) {
	if(!isValid(i, j))	return;

	path.push_back(S[i][j]);
	if(isVowel(S[i][j])	print(path);
	
	backtrack(i + 1, j, path);
	backtrack(i, j + 1, path);

	path.pop_back();
}
```