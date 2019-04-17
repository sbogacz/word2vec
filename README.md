# word2vec

Our first Lunch and Learn workshop, on Word2Vec

## Install Conda

You can download conda [here](https://www.anaconda.com/distribution/#download-section). 
 

### Additional ZSH instructions
```
# >>> conda init >>>
# !! Contents within this block are managed by 'conda init' !!
__conda_setup="$(CONDA_REPORT_ERRORS=false '/anaconda3/bin/conda' shell.bash hook 2> /dev/null)"
if [ $? -eq 0 ]; then
    \eval "$__conda_setup"
else
    if [ -f "/anaconda3/etc/profile.d/conda.sh" ]; then
        . "/anaconda3/etc/profile.d/conda.sh"
        CONDA_CHANGEPS1=false conda activate base
    else
        \export PATH="/anaconda3/bin:$PATH"
    fi
fi
unset __conda_setup
# <<< conda init <<<
```

### Check the install

If you source your shell, you should be able to run `which conda` and see it. If you run `conda env list` it should contain one environment name `base`.

## Create the env

Once you have conda installed and this repo checked out, you should be able to navigate to this repo and run

```sh
conda env create word2vec -f word2vec.yml
```

That should include several of the libraries that we will need to get started with the data preprocessing in the tutorial.
