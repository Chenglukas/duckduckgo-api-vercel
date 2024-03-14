# duckduckgo-api

## 使用VERCEL

原项目由于flask使用了async导致报错，vercel配置文件也出现错误，已经更正所有错误；删除了docker配置，只使用vercel部署的本项目

可点下方按钮部署到自己的Vercel

[![Deploy to Vercel](https://vercel.com/button)](https://vercel.com/import/project?template=https://github.com/Chenglukas/duckduckgo-api-vercel)


## 自部署

```bash
git clone https://github.com/Chenglukas/duckduckgo-api-vercel.git
cd duckduckgo-api-vercel
python3 -m venv myenv && source myenv/bin/activate && pip install -r requirements.txt
gunicorn -b 0.0.0.0:8000 app:app
```
