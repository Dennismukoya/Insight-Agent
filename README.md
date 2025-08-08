nginx 

Client → Cloud Run (FastAPI) ← Artifact Registry
              ↑
         Terraform deploys infra and image
              ↑
        GitHub Actions CI/CD on push

sh
cd app
pip install -r requirements.txt
uvicorn main:app --reload
