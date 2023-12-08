# Forget Me Lots Bargain Bazaar (FMLBB) by Thanawat
Thanawat as in Thanawin and Nawat. Thanawat is not a real person. But he is now hurt ;(

We have the following repos:
- [Deployment](https://github.com/thanawat-fmlbb/deployment)
- [Control Panel](https://github.com/thanawat-fmlbb/control-panel) (for running tests)
- [Backend](https://github.com/thanawat-fmlbb/backend)
- [Result Collector](https://github.com/thanawat-fmlbb/wk-irs) (nicknamed IRS)
- [WK-CreateOrder](https://github.com/thanawat-fmlbb/wk-create-order)
- [WK-Payment](https://github.com/thanawat-fmlbb/wk-payment)
- [WK-Inventory](https://github.com/thanawat-fmlbb/wk-inventory)
- [WK-Delivery](https://github.com/thanawat-fmlbb/wk-delivery)

How to get this whole thing up and running:
1) Clone the __deployment__ repo. Ensure that you have Kubernetes installed and `kubectl` works. Ensure also that you have access to the private packages.
2) cd into the cloned directory and run the following command **in order**
```
./signoz-setup.sh
./deploy.sh
./port-fwd.sh
```
3) Now that the app is running, Clone the __control panel__ repo. Make sure that python is installed, along with poetry (for dependency management).
4) cd into the cloned directory and run the following command **in order** to run the test script.
```
poetry install
python3 auto.py
```
