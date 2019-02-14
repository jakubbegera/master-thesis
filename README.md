Master Thesis
============
# Software for distributed control and data readout for network of Timepix3 particle pixel detectors

This repository includes theoretical part of my Master Thesis, writen in LaTeX (using the [K336 FEE CTU template](https://github.com/macekond/k336_sablona)).
For result PDF file click [here](https://github.com/jakubbegera/master-thesis/raw/master/diploma-thesis.pdf).

## Abstract
The aim of this master thesis is to design and implement Pixnet software - modular distributed system for control and data readout from network of particle pixel detectors. System consists of two main components - handler and master. Whereas handler is used for operation of subset of detectors and master is used for controlling of handlers and for providing API for controlling of whole system as well. Primary consumer of this API is a single-page web application but it can be consumed by 3rd party systems as well. Scalability of system is realized by adding handlers instances and distributing detectors across them.
The presented system has a modular architecture - instance of detector is given by his communication and data module, which has to implement defined interfaces. Thus, the system allows to operate heterogenous networks of detectors in homogenous way. Furthermore, the presented system includes a module implementation supporting Timepix3 detector, operated by Katherine readout interface.
For development and testing purposes, an emulator of the Katherine interface has beed developed. Emulator implements subsets of commands which are needed to basic configuration of detector and data acquisition setup.

## Abstract (Czech)
Tato diplomová práce ze zabývá návrhem a implementací software Pixnet - modulárním distribuovaným systémem pro řízení a vyčítání dat ze sítě částicových pixelových detektorů. Systém se skládá ze dvou hlavních komponent, kterými jsou handler a master. Handler slouží pro operování podmnožiny jemu přiřazených detektorů a master k řízení handlerů a poskytování API pro řízení celého systému. Primárním konzumentem tohoto API je webová single-page aplikace, ale mohou jím být i systémy třetích stran. Škálování systému je realizováno přidáváním instancí handlerů a distribucí detektorů mezi jejich instancemi.
Navržený systém je modulární - instance detektoru je reprezentována jeho komunikačním a datovým modulem, které musí implementovat definované rozhraní. Systém tedy umožňuje operování heterogenní sítě detektorů homogenním způsobem. V rámci této práce byl implementován komunikační a datový modul, které umožňují podporu detektoru Timepix3, komunikujícího prostřednictvím vyčítacího rozhraní Katherine.
Pro účely vývoje a testování byl v rámci této práce rovněž vyvinut emulátor vyčítacího rozhraní Katherine, který implementuje všechny příkazy, které jsou důležité pro konfiguraci a spuštění akvizice dat.
