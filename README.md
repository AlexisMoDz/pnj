Ceci est un script pour gérer la densité de vos PNJ's
[INSTALLATION]

1) Mettre le fichier "pnj" dans votre dossier resource [../fxserver/resource]
é) start votre fichier:
```
start pnj
```
```
git clone https://github.com/AlexisMoDz/pnj
```
[MODIFICATION]
```lua
DensityMultiplier = 0.25
Citizen.CreateThread(function()
	while true do
	    Citizen.Wait(0)
	    SetVehicleDensityMultiplierThisFrame(DensityMultiplier)
	    SetPedDensityMultiplierThisFrame(DensityMultiplier)
	    SetRandomVehicleDensityMultiplierThisFrame(DensityMultiplier)
	    SetParkedVehicleDensityMultiplierThisFrame(DensityMultiplier)
	    SetScenarioPedDensityMultiplierThisFrame(DensityMultiplier, DensityMultiplier)
	end
end)
```
Vous pouvez modifier le chiffre "0.25"
Si je me trompe pas, c'est 1.00 max
0.25 réduit pas mal de PNJ, et donc réduit les lags ^^
