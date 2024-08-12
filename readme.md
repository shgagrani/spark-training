## How to setup pyspark and jupyter notebook in a conda enviroment

Create a conda enviroment
`conda create -n env_name python=3.10`

Activate the conda enviroment
`conda activate env_name`

Install Java
`conda install -c conda-forge openjdk`

Install pyspark and jypyter notebook
`conda install -c conda-forge pyspark notebook`

Test spark installation
Run this command in a terminal
`pyspark`


## Different types of joins 

![Different types of joins](https://iomete.com/resources/assets/images/all-joins-03ec2ff69556ac2b668e58a4bbfa764e.svg)

Pyspark Join syntax<br>
`df1.join(df2, join_condition, join_type)`

PySpark join type must be one of:

- inner (default)
- cross
- outer, full, fullouter, full_outer
- left, leftouter, left_outer
- right, rightouter, right_outer
- semi, leftsemi, left_semi
- anti, leftanti, left_anti

Default join type is inner.