# Teste_Conexao_Python (testa velocidade de Upload e Download de conexão com a internet)

# Instalar pip install speedtest-cli


import speedtest

teste = speedtest.Speedtest()

down = teste.download()

rsDown = round(down)

fDown = int(rsDown / 1e+6)


upload = teste.upload()

rsUp = round(upload)

fUp = int(rsUp / 1e+6)


print(f'Download é : {fDown} mb/s')

print(f'Upload é : {fUp} mb/s')
