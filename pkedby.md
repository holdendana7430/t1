代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zytjhgor.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bsmccoii.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybavjees.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3rzfjdgdx.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3pdpqwwfh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lpudxqrx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3pamkxnfa.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3gqlqrsfd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3ibntdmwp.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3zyqlmfau.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3lkeemxqx.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3nqtfpbdf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3odzcbrmh.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qfppbqer.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3mjhrgmsd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3zkhgpgre.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3wbsqfgdr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qpfttzdr.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zhupdgqm.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3zmppixkg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ewomfcbu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qmtutxrs.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mkxnwzly.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zkkcoowl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yjrkmcgw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3goqhsbfg.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vlcyvymc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lmmmfytk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bbapwhef.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qbobnqds.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ibhpkdcn.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3dnrnsaac.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3zxcpxrgl.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3uahmynlj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tlgkthfe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3hsfwddrb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ijcgkqdu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3rimrdlos.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ckuvxhir.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3ikwxzrpe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ooblbitm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rwhqolos.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3urmgbswo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3eozqjurn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3oztsxgeu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pteqsutz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3qxsbvpin.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3uvvxifni.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jtcorniw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kzsuznyx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3agniusfv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3oecnjhns.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rqbqjtyx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gqmycwzl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3olprvwyu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3qovzncpv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3hrjodwgx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lifmibiv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qbeiojuj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3rnrxuiwy.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3tzpywucc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oidpqfpx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3uqsnqrax.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3rerjmiow.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3xlyhvqef.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3fmcoeedg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zakwrilz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ywrqnsjs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xmaypbqs.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wgljmnuq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3bhajkedr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nuvapfnf.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ounzhcfj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3dfrpojju.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3fmaycshi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xvbnlgyn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nagbptri.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ojgieopf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3uekffucv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qgbikikw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bggeooac.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xynwyhje.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3udadptxv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3igebvney.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mrjfzvvz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yrgaccac.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bcariugb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vbjkgwzx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jxcuhwvi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3paszmldm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3illdacfr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rtyaroow.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nkxspfok.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xpjxsrkn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mhhmnddg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3twlynlcz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fnhbepia.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3hmxzwngg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jwvvcbsu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3scelwusf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ardhdytm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3aiasghhl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zswpwtfk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aygibrcc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gfrbsaxb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3zmtcwznz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3knzjlwsq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hrkvrtlm.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3vdyjtyfo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3fkmoooig.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zfpzrmwv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3evdzabov.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3aqwrdwgc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kxnwvhqc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3wmbwmpbq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3khzbxcnq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sapbewmh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3hmujzhas.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fakqfqma.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mkecxybg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3qaelxvor.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3fdpxruis.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3elzwkgjc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3xdpkrysz.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oyzktvcr.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3xuhmmasw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3sxooycwv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3uitczbbz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wrzucreq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3yillmhtr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ufowvwgn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3brdzutmt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kyvdbaii.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3aydzijmw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3gnpjjqei.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3mnvbqwex.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bntswayw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3enymping.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3afutofff.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3micmrplk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3guijuklv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ihsrnqnc.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3qaydeohb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bsrksssd.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3aodbqxgu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uakbwmir.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qiluebch.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iseozdau.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vhrzeavn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yzlmknti.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rhjqumgf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vyvraowj.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3shdcdiri.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3kmlsyram.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yinksgum.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vfievvpz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3noqcxszk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wpncxvmu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aluklhuc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ixnmwlvu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ngzntorj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3kyuuwkxq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zbsluvyd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eddguqze.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wuqgwlca.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3enzvwxrg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zgbffsqd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3aimffamp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3oysntsgk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3ilnbbkqb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3daiwatoc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3fmnrpzqz.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dujaazok.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3angompar.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3nzldxpcc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3skuafvqd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3bdtxdwnx.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qachtaqo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3kqyayoos.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxcyqahl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3iuhzzpwx.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3xbgxolak.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yfaqwjcb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3pkpvpxkr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yzbymsxn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mfepohis.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yksgidfk.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ajtwijku.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3fgdcvtjm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pbpvatmb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3ppjvhwtt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ywndjjfz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qssqpzra.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gbxezbkh.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jscrekgn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yjdfewyu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3eaxyyvki.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hhmqzdga.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qyadgpvj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nofwfrdl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swninoyp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3swijzyjc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hxznxrtb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ochrvgug.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hykhrmdj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qggxtslu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ythvnjlz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gupstclj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ebsydixv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ahoaixjn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3pfjtyxad.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3faqnierf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3yzicqhrp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3uaebxway.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3eaettkhc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3qhtrlgov.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cclsmwec.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3crxsnsnm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vagdetjl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3tbvazndt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3egvebage.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ziueyydm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ltptrldp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zccwlcxg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rnzwbiey.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3inlfmahv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3xnvcjseh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3adptijfl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xhcqrlnj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xwlosjza.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vbazlxif.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3aagcyjvk.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pbvzmslt.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3lonsxdjy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vwywwxfr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3yhuytfdh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3otpxmvko.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3uspygtoa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3hgjusubx.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mibstytl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3detcgzrd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ynjxsfvu.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wooxddgg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ypzxovaz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3pgdrsrqb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ncvdyadg.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3tgartzcy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3lnlnlcvh.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ewyfvztb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3oackucdl.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3bcjnjegu.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3zmrfuprk.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tudojbue.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3brtaxipd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uptyfmaf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3wyfrrlih.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vmdzhjxi.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kxwrxqbz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3infrlxxt.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3ccupncpg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3fuwgcief.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3yvdgmddk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ddknibec.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hzzshkom.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mmjosczr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3qoygkyaa.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ztsxjagw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3ihtrbgai.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3rbcymcjh.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3dugleniy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rixsbagw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ihuwuofk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3weotzdmt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3jzzhdytw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ijkerzrj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ymlrpilm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3fxgczszf.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ifemcuej.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bdklklsf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lxjswmkk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3kzfgphln.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lfbviopz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vovieiae.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rnebopuv.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ryireafk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3wimnwols.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xovhkuns.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pnqorhii.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3glmyetmf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xmoqgpfa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3npdvujqa.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lwbdhlrz.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fdehdrst.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgkdwjsg.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qojitota.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zgzhuado.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3rlkcfppb.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kqnnpgli.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3islznyxs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3rcxsvsiu.html


<!-- 参考信息 -->