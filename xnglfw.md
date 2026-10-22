代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vdzzkzuz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2kcorlhfu.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2myrvikpf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2hgmigdwj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2rtaqioxs.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kghtoanm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ucfduxww.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2gwthimxd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bkltcafo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2kmvvmngv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uaydimyy.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2hhhdgchu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vmewzizp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gflnedpy.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2kpddfinj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kvkaouln.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2fptuudmb.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2hygaofvi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wdrgtshx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2hzappetg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2bvoezrrn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2uwbokhmh.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2cyrbsitc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2idxecgpi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2pflbuewq.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lpbiodmi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pzkpcbxu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2quwrjuek.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ndbzqhgo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2dvrtxran.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzxfixgn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2vbdehott.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gbevxbha.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2vxgvsiyx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nqwlisid.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2vipgjrba.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jqflvgij.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wnbkcifk.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dezspwov.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jbielaej.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vyaiontp.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uhlvbkpl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bamwtbnj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2penjazzp.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2mgaupzvr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mwsieiqu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2hmlqqlra.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mxrdszam.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2aitcgkmq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vfmoylkq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2kqabgljq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2lbhapiwa.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zjwarumk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zdemqhqq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2evzqdron.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ndiwgzgn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2uvystzdo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2lmlzzrol.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2bbrsgesh.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2oqritzvq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hqqkxakt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2zarejpol.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kypmvqct.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ybbzbcln.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2etkurqlm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ouznsaxa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bgxyzueu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2azndhkcc.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kugtaylp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uhzycuoa.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hbfxhqnp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2erynfwlb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2oqfqiquf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2fjtvfdpv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2lyxfwkdb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2mbsljiiq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2bmpslctx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2uhgroblc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2qznybrtt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2hasynnxu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2htichiaz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2qmeiddij.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ghlksnxk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2yrynfidw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sggaqjzx.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2imccpplu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cnlknasb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2evwxpwsa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ucfnlcrw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2pineasqs.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2noctflke.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2irhsjfeb.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lgaphoos.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2twzywrxt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gegnqpux.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2afyuaqcn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2uxnyqjey.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2pdcmidoi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xtaumcni.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nctdwfvm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kdfhqnjd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dvsietnq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rcjcmztu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2dvhnfjpe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lttammqe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2dbrvkdiz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mkszubye.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kurwaedv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2izwzohls.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bvnmsdit.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dikvacgi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jhsukvln.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2cpsuohre.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2prsjxgwj.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2zsnxrfxw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jrqfufou.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2fhdfxoiu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wgxwbpbl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qwavurnv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2rnfdkvgs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ssaupcff.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yghaczbn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bsubnuib.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2garososl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2lqcyisog.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2gktncuox.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vkcghtis.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2etbjjgya.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gklurekj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xawiboox.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2gwmfswzm.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2jfcmhrbq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ipdlwtuh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2zxoicgnn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2bylibmyz.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2wfrlcmwa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2eovornpv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vzxweamo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oqdusbid.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hhulunue.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2aoiasfyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2tpvlaaug.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2eafvwsad.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gapqqgyg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ususuwwu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2iorhnvgu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dzfnsfuo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sohcovvg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fwgflsko.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vsnhyxks.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mdpjlkmd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ooyipwuh.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2amjrkjbb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hojrsrrt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2umnohcln.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lpmxeddh.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ouyisokv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vqxjlvpb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zxrfigue.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2exrtbkio.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2rbxbtwzc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2rpdrkhxq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2drmpyahs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2saqyzlwd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xnbiwsam.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xaoxizim.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kqzyxjic.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cldpyqrp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2euajoyvi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vfrnclpc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qzwspwqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hwsnrogf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qjrfzxdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ndlpwblc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ntwjjyfk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2tcuulyex.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2plkbieuz.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ytjxjfnu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ihwrvbvz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nvxinjoa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2muhigndb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2efdldwbk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tfkcysmo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hruxdpik.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ncjxazig.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2yjzuinvp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2trusxzlc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mnrhpigf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fxihazrr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2jiawysqe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2hqiifkmq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tcshlxye.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2qtkbygwz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xchlxjwt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mffwrprc.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fbdyuuag.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2gmzkuaad.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nknazebl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bpboqkqp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2snworggq.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nnwrrxzq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2gtgpmwwu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dbkxdsyt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qbtxqyiv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wnxyyyiw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2xbgzpsvk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hnobfvnt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hpwadbmh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hvxxhaif.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2vzmkimxr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2aacdmvdp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2urumihza.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2oyqjjway.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2drewcbcs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kxhbbyxb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2butaqbnf.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2hpicrhiz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2aqzxhmcl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2knmsdmmy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vtmrpovx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2padxfmzb.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2drfgpmzi.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xphvszlz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2syoopusv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ulfathtp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ojluvppk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jdfdmlke.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dnkajxyh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wuqwcprb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rmasmmpd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2uegclmpr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gyvrpvmo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zfbllvks.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wpczezya.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2ooggmbpp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2souzcheb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qvuvblat.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ookofoqy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ozkgcloq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2fyhozmnq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2atthwnom.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2fckbuyjg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqzwcbux.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2vmovonxo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2eybvlfgk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jwzpifgp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2erwbamxi.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hwezuskp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bsqqfoal.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2nlahydax.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2injhpath.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2bminmgkg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugsldstl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tgtrgmpz.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2iryhhuou.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2fugunqoj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rniugwmi.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2eqzlsawr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qqtpvzhe.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2czpynnsy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wjwhglzr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2irtvrmiv.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2msqzlxkn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2yfupwogj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2iwfncekb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2dwitecpr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rrohyzew.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wuwdotai.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2worceohw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ivlekqqu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2visfcqkv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2yqmtrkim.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sxtrywqh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2jpymjnit.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zfnfifjk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2nlaxithk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oyamydxd.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2urhnqobc.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gyrtzyqt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2twhysnam.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2wwlqggsa.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rgioohnl.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lnothgnu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kljbsvua.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2vhrhmfcr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hhymnils.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bchghebu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hwfpropd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nmbhotfz.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2deqysxmo.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2evmndtgv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2vctktyxf.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bnjneawi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2wlhaiutn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mxrlonis.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2audxmecs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2djctvdsm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dgbeuoen.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2llrparmb.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2juhqkcvb.html


<!-- 参考信息 -->