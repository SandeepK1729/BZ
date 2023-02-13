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
<br>

1. Problem : Number and character notes
- imagine a numberpad of old nokia phones 
- It has some issues, when you type any text it will print the number 
- your given with set of number, print all possible words

```
String s;
vector<string> v = {"", "uv", "w", "xyz", ...};

void printWords(int i, string word) {
	if(i == n)			print(word);
	
	for(char c : v[s[i]])
		printWords(i + 1, word + c);
	
}
```