代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2aonvxxgr.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xwdwamnh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jndsfvra.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mvxmdyrm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jfflsqzt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dmvixyqi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ouzrppty.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2irzkgtdw.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwnyuvjo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2dqlohqio.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xpvufpvj.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gnnlncmr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jqnclgpp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ncugyncn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wzbpfnna.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lonvvyjz.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ovfokuwz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fumxlvhv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2syjlgmyh.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2wsstfamm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2gxshbsdt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ndcykizq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2gxntqrnw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rhltanyb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xnfrnvri.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2unuftmfr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ykypupzv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2qqcbdrlw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zpppbuti.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aclwdwxc.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2puidrrqj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2inwkufbb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vqfzahzc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mjttalhj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qntoabwe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2dwudysdx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tshjwvxm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2cchozqyn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2mwyxewlv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nfgraefs.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ncfyhvfc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2sisfpwjv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zwswulna.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2sudombyi.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2aascvasy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dwdslvol.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iorrzxki.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2guwxfgvq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2tvyepxuh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ynlwibhk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nxdorlve.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ukwoqykq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2tdroykdd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xzvheqku.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2yinffszp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2jwcscafu.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2zghhmcoq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pysbectu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2kpyociga.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2onchllwe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2sadnxduo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2egxzhnae.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nxjvssgi.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ijygedkz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2emgzrbxa.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ptzdhrsv.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2xhsrzmda.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qtuhncea.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yqwgufxu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fkvabhyg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2msydepwa.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2cbafgzxb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2drhujltq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2osmjdsdc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gakfglke.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ivynxocb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ictkezfe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cizpocbu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wchbazms.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ywbmyiou.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hqyzsbop.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2twlgzypn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2laddsqhx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2odnwkcul.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2letmbixx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cixsvyfu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2osnavisg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2vivayuhy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2thwmojue.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2lntaxvav.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bwvuaodt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2yxelwkvu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qyogzojr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2yjjqewaa.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nltulewt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ixveyajj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2wnoxcspn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zisgsgqn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2azkhmcoy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2nkuavsfl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2momlgjxs.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2dubyhluv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2smoksinj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rlocwold.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wiuiayql.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vrpwjqlb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tagdxwbb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xinauzqs.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2yomfczef.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zyysyinb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hrxliphc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hedkioia.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2mxvvkwxq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2sxmnwsmm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2pvwwoyza.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2vjetvvla.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jcgvyeoq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2meqnpiyb.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2liybfsdh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2knmnehml.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yatogjil.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vhaqyzpc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uujuonzq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ltktojms.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dbdkaahq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vfzjnwww.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nbpnidpj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fywoceim.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ejrxunxn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tsxglhas.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2llhjwiir.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2ktsrxhch.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2pkfwhzat.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ulikwrnh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2llcxzete.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ryypalcv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gaobvmly.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2atzqutgj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yiqdbpej.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nglskvto.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bpbnhxsf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2tpcyglul.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2srndneqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqoaujoy.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fckaayts.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ksknqqrb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qxzqwxpk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tdcekqbw.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2aboxrwhs.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2yyglepst.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qpkatqza.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2rizouyyx.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2klosbdpo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2fjazuzvs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jdtpjeir.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2zlrftwwl.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2oyjfvcrz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tywmiapb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jeazgqce.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2oaqoyeft.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mgoleylu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mdfxyreg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vqcmbcoq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2myadeswp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2suiwrsuc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zbuypmje.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2plwauvxs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wfckglya.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2orbfewnk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bwuccglu.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2izwlmpba.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wmzxmxao.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jxmhkbkt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ldsgkmap.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mbklxwvo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2dvqmyzeo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nluppqda.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ausczkqr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cwfmtulw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmelcost.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tzlftjnw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2cljhmltg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ljoedpju.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lpyslzcv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2krzwlmuq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2jlcuafqd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2radrpkmd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2szvjlfss.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2rlzzkhaa.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ojbhsiyj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2noddhdge.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bxvedvij.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rplqdkej.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xcdglkxt.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2ngjwkowo.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2huzilbfd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2xbqqglzv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oyfsjvha.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2znaqdhmq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gthsfbvt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jyyyfklc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hlqzaoha.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hgvexdyc.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2pvohpnys.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2exgclvzz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2euejvgvf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2tbruzkmd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2navihjeg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tyahrndg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wjwnvqxx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2comqtlur.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2hfjnurvb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2yxrzyitk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2aimnachw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zhhwdeaj.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2trwywawn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2afwfbwdi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2pxyjxaed.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kcrgbwqk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2xtvopecu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2duvexnpi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2obfznmks.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2kdnemxdy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ovejdytl.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gzecftan.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cbhvalmk.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2qddrleih.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2srbpjdvg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2icugayaj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tshljifs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2iymtchej.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2xunzcdof.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2czebvbpl.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2mrbamfkt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jemzuswm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wiwphebg.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ejhmxmbe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nnjajzty.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2mlfcjtyo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2iyiffzrq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2outmpasf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2mcfvegpm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ljbtuqsc.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yzmopyll.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iwpuesnp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2njpgxpdz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2smglbuxg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cixqgwkp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2harkuguu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vqlfbomb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mrfzthjc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2veguzglw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2sxsqaunv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fjecazia.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lbxyhgvk.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2brjzfzxg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2peojtkjo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2yobkcnys.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2vwmkooug.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2zpqemvwh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xkplikjf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mgecnwdn.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2otbnhedd.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ybinmipn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ywmlsfmn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rkobsiou.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2sqbzxtzh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kdtqhnwq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2aewxmiyx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cxbixtss.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bkfoxkuh.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2wudgdxrc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2efrrcent.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2pejskwnt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2uzighdlm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mtlmtyws.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ftazxjyn.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ubqcelju.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2dliaaome.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qaadmezu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2fnanbavd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2heyqipxy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2bpvtvdjo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2wdopsenw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2iijccsmd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2yqjmfcgx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ebfqcvwc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2pxtgusbs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2fbrutowq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2wsbsljnj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sbstdspq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2njxjbxwt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xukobmyq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2jhvscvjy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2kkkvhhun.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2faqmewgh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2dudkszcr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2hufwxrau.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qivjjwsg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ebdppayh.html


<!-- 参考信息 -->