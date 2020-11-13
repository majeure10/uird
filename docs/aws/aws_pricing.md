# AWS 计费与结算方式

## AWS 计费方式

1. 按实际使用量付费[^1]
    
    AWS 针对云服务提供按实际使用量付费的定价方式，且无需签订长期合同或复杂的许可协议。 
    
    计算资源方面，以小时为单位；数据存储与传输方面，以GB为单位进行费率计算。

2. 购买预留容量

    对于特定服务，如Amazon EC2 [^2] and Amazon RDS [^3]，用户购买可预约容量，预留实例，用户预付的金额越多，享受的折扣越大。若用户预付全部费用，可享受最大折扣

3. 分级定价[^4]

    对于传出数据的服务，使用量越多，为每GB支付的费用越少

## AWS 结算方式

1. 12 个月免费：这些免费套餐产品仅适用于新 AWS 客户，在自注册 AWS 之日起 12 个月内可用。当 12 个月的免费使用期过期或应用程序使用量超过了免费套餐限额，只需支付标准的按使用量付费的服务费。

2. 永久免费：这些免费套餐产品在 12 个月的 AWS 免费套餐期限到期后不会自动过期，而是无期限地提供给现有的和新的 AWS 客户。

3. 试用：这些免费套餐产品是短期试用产品，始于第一次试用开始时。试用期过后，只需支付标准的按使用量付费的服务费。[^5]


[^1]:[AWS Pricing 定价](https://aws.amazon.com/pricing/?nc1=h_ls)

[^2]:[Amazon EC2 Reserved Instances](https://aws.amazon.com/ec2/pricing/reserved-instances/?nc1=h_ls)

[^3]:[Amazon RDS Pricing](https://aws.amazon.com/rds/pricing/?nc1=h_ls)

[^4]:[Amazon S3 Pricing（分级定价）](https://aws.amazon.com/rds/pricing/?nc1=h_ls)

[^5]:[AWS Free Tier 免费套餐](https://aws.amazon.com/free/?nc2=h_ql_pr_ft&all-free-tier.sort-by=item.additionalFields.SortRank&all-free-tier.sort-order=asc)



