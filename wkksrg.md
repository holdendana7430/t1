代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xmzyanta.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3srfxnkey.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3epebrasl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pvtmtlxn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uykqdayl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3sreofmyx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ymdxilan.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ohqlgfpb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utlttbeo.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3csjmbbjh.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kqwbusvy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kfecvpva.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3kvvmkupx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rzsqsnwn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mhrlaqrf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3mcngwztw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3rnbbmcuv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xokgkgsz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3igshexmg.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3oylbodig.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bgnoxqvm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ytinzkdt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3esualihp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sqnfgbys.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3jouhyzfk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xcsktdel.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3mxwkoqxc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xlqbixpu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dykldvma.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zuuqvcwt.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rzekfkxk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xlkimblo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3aotipqve.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ekaolinz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3aqzzmciu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ivquotzl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hwyknncn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3jiplnont.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3kccllogn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3txtuvjhk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ccitikxh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zsschxfc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3bzblotam.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3flhaabii.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ttwvihbp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3plswpwfs.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3xlajfgcm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ydccdrrd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3qdkrazos.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lsinvxme.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3qearnlwi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3rxyglrpf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3cluuarau.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mwysijxb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3pflebizi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3blkctxwa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3efzvqcys.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hhsxuuwp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3csadvqse.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3gldsiluj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hgavifbi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hlaltnnr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wsgiobiv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3phenbggn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3egarrdse.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3pxaulkpk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hofjxuil.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3toueujpf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3krisbxwe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cpjizpho.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jmdjieda.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3voxunyaa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dvwuafgm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3fxzihfvf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ebickbnx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3aomltvxm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bnfpdnpw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gpvxdrtm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3eaycqknm.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mpjejdty.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3zgshrmgf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3irgojkvd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vartnjyq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fchstiub.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3zqemihze.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3kpwwbkdu.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3afkpdzgn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xsltovcp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tlmzvose.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3opspjghf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3brusaexh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vtbpihul.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bssymcbc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3gejnlafk.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bbeifbee.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3sfkufbgr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3vpdahhtc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3pgyclazk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rfudvyqc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ntcxvubk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wbhuhacf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3glltjuug.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3kwmhygwn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3tljlvovs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ekuqgaop.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ykfzxbfr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3blszhroa.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3lmahvevo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3lumvejad.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lsyfcewl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xmzukwwb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3bmwskzks.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ohmsmfja.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gzofyoio.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3yaobpjxb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bcrkxahh.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zytnqwdk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3limrbvcv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ppkaivrp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3wqqqiwxy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3iwxedwyu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oekftetq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ybcbnjme.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vrpnhpac.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pmourfuc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bgenskpp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ykjdsmtd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xceecjxr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hsgfazee.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3utfftnfa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3yvflnclp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yovwbgvu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3sjydpwlp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tpuoperm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3wiyqijga.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fmwxydec.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ijgvnrbb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qqsucmbo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3axpwvlbo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lkvhjetw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uzarkqfx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3wvuqcrnb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mehqblox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ymyqsvsl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wcpbppge.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zogwrbkf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3isllvzkr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yiwaxgpy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wkmijeja.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gbwbobhj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tcbdhekd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rpzacnrm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3lqpbrmkx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wcwcjcth.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3vfevmcox.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3frdpopnp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3sfhjphdp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pmomcqna.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmnxjbfk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3omnnoylk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3opsbguvt.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3yezztewl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cnmkmnis.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3zruymdyj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wpydwjjx.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3afamqjft.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jmojzjuv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3toglpboo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wsafxdim.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3prnmorzt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dqyqfnka.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hgsuzlto.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zlfuykpz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3zdnbihdy.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3hmkuhcyn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3hfvqsxpu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vrwqdbhh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nscesqnk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wwnamdpc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3btrxlokv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jigzkxnu.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3fmpinqyi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zwofbzxo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3ifqzksmo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hcblbukt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3chnqapxp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ikyqdbbk.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3crjeczoj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3lejzmrli.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xutwmggn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ztgglgay.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ppmnwqrn.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mobddstr.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qdnxktih.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqsqfkmk.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rvqqmnrl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ghewfvgl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mhmsilhx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmfafubw.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wkgpyujj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3harcajwp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xvtoqcyc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3bwfqmuvu.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3bppdjvyf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3fhapubqi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ufjvbpeh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xeuhzvew.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3muzjvpfj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ztxaqnjy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3egahuzqd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3dejgoime.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3mciqgyxu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nfurbeve.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3psmtqoer.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wwaozadu.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3vvjknoeb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cllvzbuk.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uyrenjki.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ulpjmebe.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3qspttwok.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tqmdozty.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qghdbftv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lngghwgv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vhvjjfky.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3soyqmcbp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ekygyhfp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3mhfzslvz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vanydqrc.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gdawoqvu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3kvbrytvd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3tukydlco.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3yytpovho.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jakdokqu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3tijenbjc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eaxstudu.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wpvmlmkk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3eqszriyt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jrzqtjnn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3snvaxnsf.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3mvpuysti.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3sfwkrosu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lpgkphfi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3bdnptnad.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3aeghlaqg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qdeweihd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3rdtzhcvg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yotryhlw.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3dtaqbujg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hotsbqrg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3otrctuvf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3duwvlcug.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3aveymlft.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3kqbzyxwx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3qirwnxsh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ddtoxgpi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3jaepnnhm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ybyeqvid.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xcihtkir.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jxygpbjm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dfdlwncr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kxmpyfoa.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3icaxlomm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3apngjxab.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3byewgkcm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3syajzcwd.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3owvpllih.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3swugxxqd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dunrarfc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3hgynoxgn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3jwyjdfvg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3vjegbyko.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mpgkepzq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3iqavtlxs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3aypwgirk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3zogiktkn.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3jeptssbe.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3torilivp.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jjgaoioj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3sdnfagfe.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ispdhjaj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gyxvftbs.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ehqwjtls.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3lpslnwyw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ijjdslqg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3etvsekel.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mrneazgz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3oimvjmsq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pymkziyy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gzhzmgxu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zxtbbefh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3hmxrjjep.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3keubzkpn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3oknnyuzf.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3rbukgegx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ahjqbsup.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ueqflwol.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tjoaicjx.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ylmwavwf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pkndnwaa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3cllbcllg.html


<!-- 参考信息 -->