# MNIST Addition

This example shows a simple implementation of [MNIST Addition](https://arxiv.org/abs/1805.10872) task, where pairs of MNIST handwritten images and their sums are given, alongwith a domain knowledge base containing information on rules of addition is given as well as artificial inconsistent information. The task is to recognize the digits of handwritten images and accurately determine their sum under the existence of inconsistency in the knowledge base.


## About the Codes

1. `kb` contains the knowledge base code for ABL as well as the logic programming code for addition rules (`add.pl` for classical logic based knowledge base, `para_refine.pl` for the paraconsistent logic QMPT0 based knowledge base.)
2. `training_logs` contrains training logs for both versions of ABL on the task.
   
## Run
Install [SWI-Prolog](https://www.swi-prolog.org/Download.html), please make sure the version of SWI-Prolog is below 9.2 as `pyswip` does not support version 9.2+, `swipl` should work in your command line shell.

```bash
pip install -r requirements.txt
python main.py
```

## Environment

Details on the specifications are listed in the table below.

<table class="tg" style="margin-left: auto; margin-right: auto;">
<thead>
<tr>
    <th>CPU</th>
    <th>OS</th>
</tr>
</thead>
<tbody>
<tr>
<td>Intel i5-8400 CPU @ 2.80GHz and 16 GB memory</td>
    <td>Windows 11 Pro</td>
</tr>
</tbody>
</table>
