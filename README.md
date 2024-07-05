
install

```
pip install graphrag

mkdir -p ./ragtest/input

curl https://raw.githubusercontent.com/win4r/mytest/main/book.txt >./ragtest/input/book.txt

python3 -m graphrag.index --init --root ./ragtest
#windows 下使用
python -m graphrag.index --init --root ./ragtest

python -m graphrag.index --root ./ragtest

python -m graphrag.query \
--root ./ragtest \
--method global \
"show me some Prompts about Interpretable Soft Prompts."


python -m graphrag.query \
--root ./ragtest \
--method local \
"show me some Prompts about Knowledge Generation."


pip install chainlit
```

