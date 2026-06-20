# vscode-setup

Configuração pessoal do VSCode para replicar em qualquer PC.

## Estrutura

```
vscode-setup/
├── snippets/
├── extensions.json
├── keybindings.json
├── settings.json
└── README.md
```

---

## Como usar

1. Clona o repositório:

```powershell
git clone https://github.com/caioxdev/vscode-setup.git
cd vscode-setup
```

2. Instalar extensões:
```powershell
Get-Content extensions.txt | ForEach-Object { code --install-extension $_ }
```

3. Copiar configurações para o VS Code:
```powershell
cp settings.json $env:APPDATA\Code\User\
cp keybindings.json $env:APPDATA\Code\User\
cp -r snippets $env:APPDATA\Code\User\
```

4. Reiniciar o VS Code.
---

### Fonte

Cascadia Code — instala manualmente se necessário:
[github.com/microsoft/cascadia-code](https://github.com/microsoft/cascadia-code/releases)