







-----------------------
         
        # e.g. "linux"
      ult branch you need
XXXXXXXXXXXXXXXXXXXXXXXX"


-------------------------
e re
----------------------------
rl = f"https://api.github.com/repos/{owner}/{repo}/zipball/{branch}"
ads)


#  te zip into a localolder
zip_bytes = io.BytesIO(resp.content)
e(zip_bytes) as z:
    # The zip contains a top‑level folde like "owner-repo-<hash>"
    # Extract everything into a folder named after the repo
    extract_path = f"./{repo}"
    os.makedirs(extract_path, exist_ok=True)
    z.extractall(path=extract_path)

print(f"✅  Repository '{owner}/{repo}' extracted to ./{repo}")



