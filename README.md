# ISP-docker-project

In this project, text is generated based on the novel "The Old Man and the Sea" by Ernest Hemingway (using Markov chains). Also, WordCloud on novel is generated.

DockerHub Repository: https://cloud.docker.com/repository/registry-1.docker.io/blackitten13/oldman_project

To pull docker image:

```
docker pull blackitten13/oldman_project:firsttry
```

How to run image & extract the results:

1. Create a folder where the results are going to be saved (for instance, let it be `result_folder`)
2. Run the following command which outputs the results to `absolute_path/result_folder` (where `absolute_path` is an absolute path to `result_folder` - for instance, in my case `absolute_path` was `D:/DS/Skoltech/docker`):

```
docker run --volume "absolute_path/result_folder:/project/results" blackitten13/oldman_project:firsttry
```
3. Two files will appear in `result_folder`: `generated_text.txt` and `oldman_wordcloud.png`
