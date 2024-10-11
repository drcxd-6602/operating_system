# What are the outputs of the following programs?

## 1
```c
int main() {
    int x = 10;
    
    pid_t pid1 = fork(); 
    pid_t pid2 = fork();

    if(pid1 < 0 || pid2 < 0) {
        printf("Fork failed\n");
    }

    if (pid1 == 0 || pid2 == 0) {
        printf("Lol\n");
    } 
    
    return 0;
}
```

## 2