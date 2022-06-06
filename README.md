# Multi-Stack-Front-Next
## Checklist do Ambiente

- [ ]  Instalar Node.js
    - 📥 [Download](https://nodejs.org/en/)
    - 🔗 [Guia de Instalação](https://www.treinaweb.com.br/blog/instalacao-do-node-js-windows-mac-e-linux/)
- [ ]  Instalar VS Code
    - 📥 [Download](https://code.visualstudio.com/)
    - 🔗 [Guia de Instalação](https://www.treinaweb.com.br/blog/instalacao-do-vs-code-no-windows-linux-e-macos/)
- [ ]  Instalar extensão Styled Components

## Checklist da Criação do Projeto

- [ ]  Iniciar o projeto
    
    `npx create-next-app pets --ts` 
    
- [ ]  Iniciar o servidor

Em caso de erro no Windows, executar:

`Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass`

## Checklist da Organização do Projeto

- [ ]  Jogar imagens na pasta `public`
- [ ]  Apagar pasta `api`
- [ ]  Criar pasta `src` na raiz do projeto
- [ ]  Jogar pasta `pages` em `src`
- [ ]  Apagar arquivo `Home.module.css`
- [ ]  Criar pasta `ui` em  `src`
- [ ]  Arrastar pasta `styles` para `ui`
- [ ]  Arrumar caminhos da importação em `index.tsx`
- [ ]  Arrumar caminhos da importação em `_app.tsx`

## Checklist das Configurações do Projeto

- [ ]  Instalar Material UI
    
    `npm i @mui/material @emotion/react @emotion/styled`
    
    - [ ]  Configurar tema
        - [ ]  Criar pasta `themes` em `ui`
        - [ ]  Criar arquivo do Tema
        - 🎨 Tema (clique aqui para abrir)
            
            ```jsx
            {
                palette: {
                    primary: {
                        main: '#AE0FEA',
                    },
                    secondary: {
                        main: '#C5C5C5',
                    },
                    text: {
                        primary: '#293845',
                        secondary: '#9EADBA',
                    },
                },
                typography: {
                    fontFamily: 'Roboto, sans-serif',
                },
                shape: {
                    borderRadius: '3px',
                },
                components: {
                    MuiButton: {
                        styleOverrides: {
                            root: {
                                textTransform: 'none',
                                borderRadius: '5px',
                                fontWeight: 'normal',
                            },
                        },
                    },
                    MuiPaper: {
                        styleOverrides: {
                            root: {
                                boxShadow: '0px 0px 39px rgba(0, 0, 0, 0.05)',
                            },
                        },
                    },
                    MuiTextField: {
                        defaultProps: {
                            InputLabelProps: {
                                required: false,
                            },
                            required: true,
                        },
                    },
                    MuiTableHead: {
                        styleOverrides: {
                            root: {
                                '& .MuiTableCell-root': {
                                    fontWeight: 'bold',
                                },
                            },
                        },
                    },
                    MuiTableCell: {
                        styleOverrides: {
                            root: {
                                border: '1px solid #D8D8D8',
                            },
                        },
                    },
                },
            }
            ```
            
        - [ ]  Adicionar Provider em `_app.tsx`
- [ ]  Instalar Axios
    
    `npm i axios@0.26.0`