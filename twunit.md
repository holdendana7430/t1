代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wocidsfw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3emkvdsab.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ifhquivh.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3zmhggguk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3beylwnvr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xuunysnk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3utclqonp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3yantgopw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3yvdbhojz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yzkkhkan.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ycyidwhm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wygqtvyp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3picdiyex.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3fxpznutk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jkqhlpin.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wajednqs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3isrhwewn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3onziiyrp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3rbbpyzyo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ccdzxpuc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vbtpsknu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3zhbypbmm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3phqbiodw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3rnmbtsre.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3chhqmbnw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ffqkahqw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kcgkcdmu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3cqknnrrz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rghgyvvb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3jglddrsk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3szzxzocd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3wdiuredz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ajxeglzj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nvtliekc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3arkjjwqt.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3afdaszzg.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3jftjechw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3bqcoggpr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uobugmhn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vkfgsdnq.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3nsebwqyi.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bekuyrmi.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xeecfvtk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3efmaunoi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ennjdeob.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3edvidhco.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mnonujqj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rxvofryu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3pogrtopl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3wgohodpg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xmnscbba.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ufadracv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ixjqyhdo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jfehgspv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3buakilaw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hkqgmftk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3umepjwen.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xrvcopld.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rvijahbu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tfejiofi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lipmpjdl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gsovrdec.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uwykijjv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zkaxldha.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ewsokvnx.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3inqtkvif.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nzddftbs.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hvwznvwm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nlmsnpjs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jtoxfphk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3patocedi.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3clwcluyq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oqnaskxv.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3iqtfpxay.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3eeldzpbw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ycoznvyt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3sutsdonw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bxbiuqxv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rgbimyei.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wrlzivde.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3opyjhrbc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3raemqnox.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3sfwxslkc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3iroqlcfn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tccdpyqn.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3dyruxicx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zaeieatl.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3nmijahzy.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ppxyahuh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3vjbwvbds.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3lbldtpbk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ikiulbpo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3joihqvwg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fszhivof.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kdcuvxcv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jdmxudtf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qppqwgph.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3htsxgmxm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xjdxnxjj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bcwbujsx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfcntqke.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mshngzzw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3alafqbgu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3kpcsjxab.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lhqgyceo.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ayxdnwti.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3iffjuuvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zzbdyrhe.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qkqliksm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3otqsqtmh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3dcbcvhor.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ntlmosem.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3pkpfcfwc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3jfgcrclk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qvumvyct.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ewvnbnyp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3fdixnwyi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3omfrlwjm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lncgcssg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tsorzjwy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qcobgrrc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3blalxuxe.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uiqrjqoe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dhtxzuyl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3aspfsnmp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jrkofxky.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3iobsfqpc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3xcstljqo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3aoqxlmyd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rcfjettn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3qbtqmoik.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3mcyaupjs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3sjeyouwq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dkcugudh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3biyvttjf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gdjjbmhq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rfqclvmd.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jlewjtet.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yxnrfnne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3viylijim.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3gwwzfhqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gcpvqick.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vrmxkcrl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3unwulyfa.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3lyfngwco.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3qeoeheik.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3qgfmehxa.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3nvtmihtw.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hgmdahgm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3hcdfdbzs.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3wesvbgns.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3skumxnyb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqvrvviv.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ghjoqasl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3naucpspc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3nkfbboso.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ytvuggog.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ycumnnqc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wcfdvsvb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ufvcdpbp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fjgimvoa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vhjsplng.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mkjdpian.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3nohahbul.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tmpymcbg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xolvfpqs.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mtksyxjy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cmzttybc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rubfbzdm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3sahxlsit.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rraxowpp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3flpgnotg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pvbzbhxn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kzkrqgwl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fqobcovt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wkeeuqxv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3tyfqtfnw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mwdcbtvu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hwwjctkz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3stzstfvl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dabwmdjy.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3ibkevggn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3utcmbhbe.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3ykcxvqrz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ruelnmzv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pcszalzl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dbvzcfub.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3gbndmdda.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fasaqxdu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uyvrsahl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3mepfedkd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ebcryaoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3pqpivowe.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cnkawqtt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tochvjrt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3soaecwwb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qxalendf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hwrrypjd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3cybltnjo.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cjrrlwch.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hxzuzqko.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3tbbyesxa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3itdchqvz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mmsewctw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3tlikyuun.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3eifqyuwn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3ykzqskhl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3difxtnhj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ezxstkrx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3onankhzx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tkhswqjz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3xblxcjjp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3znibkyyg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3sosbspfv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3haemgeli.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3vohwrcal.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ivwciqvz.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3eeqpnofj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lvjtwmlj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3scqqykqj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3vhfrjiot.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3wyzrgopm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3fxtkpele.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ptmyqmvb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ceyjczch.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3pmzlcxvr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3hvrcorye.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3udsyoojs.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3usmdgjug.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3kkayeudz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xlkuxtlx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ndfhbvux.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3mnsguntr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3gvfbenjc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dhafpavw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3dwmwphjv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3ilmebwgq.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ikwefuzl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3rgzafgyv.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xutcrcdm.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fnqemyls.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bjypyghb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3awpdzczt.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3uvhbdudx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3qlfkchtw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3tyklpwbq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3aqrzboxh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3tpwzncut.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ydvnscvx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ujlfgzpu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iimmvaph.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3bnxbewah.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3szhraefl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ymtzjkki.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lzobbbth.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3barwmzes.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zvlgfaki.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3nhchoxjg.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3efxxxzni.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3horabfkf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xmaauulk.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3sizhxigj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3lakfcqms.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jefntbeg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3eneuceeq.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ipeupzyf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pewxaftk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3occmbrec.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3imrayjek.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bnentpvp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3mlhqlino.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3djzpionl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hvkbvllg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3gpcgmnop.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3sdbithuo.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qoksgsei.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3oiioyenu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ryxcadsh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3drkwbohs.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xocaedeb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3mgniwzmw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3pnezvicn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zwlgbblh.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3uprybryj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qabmzxpo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hvwdddha.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3kfkreldv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ydxymfch.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3euwhwgqs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3vblbeebp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nmujfddj.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zaamgdpm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3jfrmwjbl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xjmmzixx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3cmbiwgiu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3nphtnlys.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3qaggmihp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ixikkqpp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wchhiymx.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xjpzheks.html


<!-- 参考信息 -->