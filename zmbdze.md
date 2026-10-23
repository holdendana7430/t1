代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rnnsghab.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ixbqgjii.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mwrhztut.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hcnqiufk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cobaqtaq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3cymurgbc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wtrretgt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ishrvncx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bwxifeti.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jdqfwrsg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vzumennj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3wweivhto.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3eeznkwvd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3tfctlgne.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3gxeofmoj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3itzssojj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3oypefsrq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3smcmwdpx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3hrgkxsgb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3papyunyf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jgaenija.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3duurnrox.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xqwrdpsz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zfxosayw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rauykvzq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3muihyxgo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3djyloept.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yzmspyhw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kztxwjrc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3sagjvdfe.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3cfnnhddj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3tsljroml.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hafgdkpx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lxvjneop.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3fpwruunt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rywwmyxl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dyygkpeq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3krlsefsp.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ffhmhcnp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3teckwuof.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rjvtwegv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3ushzjnpv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nateqrky.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3oqmmtsak.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3razhnbfg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3kcdlstpe.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3yqiusbii.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ojewabgp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3qxismbez.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3oyzdbmwo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3icgbsnet.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3ixwoptii.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ylqjxwmj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3bgccvrnq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3keyosqta.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ungbjggo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vfvkxuli.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3zwonmcwn.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ldgufdzx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3tetgujyk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qvoqouan.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3uphswybl.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pzjwvcml.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fkutmtgc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ehwzxhgw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hwhyskxh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3werjdigu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3abnwwxqn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqpocotq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hzfujjze.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rciffsjx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3jwsysllz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cltxzqnm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3rqjdtplh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hygmonhb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xktumjcj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3upbjdgqj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wjuqojnk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rotkijhi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3vunlocfa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3otgesaga.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dbmluucl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3kjlnlqpu.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3tsxypqhe.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3sybunsor.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3vzrxrjzx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dqhukzsp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3apbtatam.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xeypleae.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jwymnnvs.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tozxdlro.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mdrayang.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3erxcasds.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3adeudaox.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rnjjtuav.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3swuieevw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gglehjjg.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wpcvafyw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3rfmhtuxe.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3hdebidnv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bcrkenxu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oynfqwec.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xbzituqa.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3bwprcpem.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3mkvvbvgn.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aywnjsxj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xxhfgwaa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ymvzodtx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hrdgxkbl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3uhzldswb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fvsuhlwj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mrcsoafa.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qgmunezb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3lyjfjaku.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vdsmniam.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3rchdpspc.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3biripini.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xvtkgaqp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jejghdid.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dgdzznlk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3admklrjw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lvhxnnno.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rowtszyy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gsfufjel.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3xmdoxlox.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yxdaojmr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3zcghbbop.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zblarfid.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3oybevten.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mugdnbps.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3svnrrfhk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3wbrmecyh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zdufujox.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3axmcfnod.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iexdpiln.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ycubfppm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3luervlrj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mijrsljd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3plecntzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eallzzdp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vuigzieq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ivgdzkcm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3bwbgxlob.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3edxfrllu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3avksktao.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3wkfwewbz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zclihvhc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wzqklsmn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wdxqeayn.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3izukirlh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3iuramsqp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jhdtnanv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3owrvbnfk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3njtiydbj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zpzzydix.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsythewy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3olqcmpcg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hkxlqxfi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xlnksvvs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jgkuixhg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3olnicqvh.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3zgnmxvjf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lbuxuhss.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ehghqmrk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3stewcoic.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3easrgasj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qnfeeiqy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lrlmgmlt.html

esac
来源：http://www.52xcode.cn/Article/details/gt3xsyqomwb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3mzuljafr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yiptbxmo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gwpawglh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mlmigmsf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3uzjmscqh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vwrskpwe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jtagfvgb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3egbxtifr.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vgwjmpof.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3akrsslmy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3hbpfnfms.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yxjuzydw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3sksabsfd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kvteoima.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dlstxsub.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3njxoydty.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jfwlvxwu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmfcbpcz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lziypagj.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rncsfppk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tkbiswlb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fkejgtyj.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lpnrkyqm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3hnaosavq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dqmswnqe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3eyuxebbn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cogcglss.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3arvxkcex.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3xuvlyiwg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ctapggmy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3zfcmdatu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gvjnyean.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3sglprdis.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3gjfqtcbw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3etlquykn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3exofhxth.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wumftbie.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mpsxdnhv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3kltwhxwe.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xvfmntxg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xjzqnyzf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oaubvgum.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vwnghvzk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3vuxcbaum.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mawwsaeu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lmabnuxl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ixsvdhji.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3toibylrb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wntromsu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3yvogyffh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rsdrjjkt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ghcdskyj.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3irwyxdcg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ykofwfbh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dyuebicr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3petfnqip.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3dwwgmnhh.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3koveoold.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vnupbiht.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gbqezyrb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vdctbufx.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3alvfzqwx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3jkfpqlpz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ldbnjfjy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3aybllhhy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hpposurf.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3pchswevn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3kfltqegr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3vicaqeca.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3dvnxmamg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3vligmkmg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ikeezwyb.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bzrpbcwj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zcoxbqij.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3vwhektdn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cygumtyi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3uvxxiast.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rfbxqudi.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wvmtjuxu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3aegoyhil.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3lpohgfqk.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fclpurbp.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vexhkzmq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3afdukllp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3epordvfb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3natoeffi.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3hjclmdhk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3yrshxdbr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3arkdfljk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3iwfbumtf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3gzzxnywa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3ybkwgkjm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jclzisvv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3dehrsfjp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3ldslggsx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3uyzssepq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3igpfyrbr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ixmjieun.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qhxgdqwq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3yfjqxwwp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3xncgdqvi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3cwdfcjfl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3yojbuuym.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3tiuikzmh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3qnofsicz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnlbnao.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zweowjxp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3usgzasba.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ndvjnmgf.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3cfzeshdw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3mhlxgvif.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3cfvngfwu.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3jkplftvn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ftglggrx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3thjdhrwp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3fbwifaqn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3cbsvamht.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3apwijjgi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aezldqec.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3yebvfoaw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3jxwxamem.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ijbyxeee.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3yrtnyojq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rccuneyd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3gxfmadzh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mfpqdyic.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3hbthwanw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jtxfwbcl.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3lhbxwaog.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ccvprfta.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3nvovkpxn.html


<!-- 参考信息 -->