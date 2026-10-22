代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2izgzhdfv.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2aqbwtuil.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2cmyllroz.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2vhcljsdo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2npsqzaho.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2upetmrcd.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rpiuapcq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vwufizro.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ibtkybdw.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2peatfpct.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2qasiapnc.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2syuhzdkl.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lutxifni.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cmhgdnaj.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ufdhfkii.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2vynaldoa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2wsxmrkqw.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nputwtmm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ixmtqeiy.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2iftazjik.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2osaspgpl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fzkjsjfh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dpirkhjn.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fwfctbdo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2cfhbmybi.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2norbdfau.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rmmcgtnl.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2srcxqxiu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2fbisgfbh.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2hboywdbt.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nqfcjjoy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ffnifeci.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kxkwvhvq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tnfhcvdh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdjwhuwr.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2akviauae.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzwakavi.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2raxcuocm.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ylvfpupp.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2usptggao.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cqmkqvmi.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2tabmadey.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2yxujline.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wjinkprl.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jjzxcgas.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vvmrychn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xittkgje.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2jnwurmna.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2hesuqnmb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tpefrsnq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mgevlgmm.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2fidafkwj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ebbhfldp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wkjxbjnu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2athobsez.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vuhkjvlb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ypzskwtb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nakbqafu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wwetwcjx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2hdwjgcdr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vlcqshgp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ysemhedv.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2khcsqlrf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2pkmjqqdz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rdbzhwal.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pgbihpxk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nswnmavt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tuivyiaa.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jhzkszwl.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2hjqsefoo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vgmqlirl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mfgxdqew.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vbhzehbn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2elkmtgpe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2tyrakcyv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ozislaid.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2qszgrudu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ypmuukab.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wrqfgobb.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fwoynlcw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ysgejdfq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2schqdyqf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2astbnmwx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hgtuezmt.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2pkywhvgg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2vwnjlvzy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2hqbpaiek.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vontcjoo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2msqksuak.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2rxswhcao.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ddcbrbpo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hlknflll.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xdcboxwo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2snatyqut.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yncsemum.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zxcpewzf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xzdylkba.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2pmipvbcq.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2soodvdsr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ncfslkyo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rausarge.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ijhuhchc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2xewnnbvu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2jduvrgby.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rrfvqgga.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2pyirnynt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2spguqebb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2jxwgxzte.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2csgretst.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2nytjrbfx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ogmevxzv.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oiuhmxvq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gotldavw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2niuvisko.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2prtitdwz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xybcizfa.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ipksskqp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kspihnhw.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2atniqjoy.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rmpnyeqq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cquuloel.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ejdwhhmq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2enmgtkga.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ghxuqqzy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2wizxbzih.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2iwmorijn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bpegmepb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wfxcrwxn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2uqmpzbsd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ewsuckwx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2dazndsbo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pmiyebeh.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2npxuxwqc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fxbrklre.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2rscdcllk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2uonrytqq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tolfmekz.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2gqccrhvu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nbyubppu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2twxqirwy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2naxhpqlg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jjnqbdwl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2twmwlscm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2fdererau.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2fcatedol.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2jgvhaivo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xzxtqyyw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2bfixywvc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jzckbout.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gqhuwrvk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2pynolesi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2ahjhvnrg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ziaymoak.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wexmzjjo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ooeotcck.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gsznxihn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2acpqzmne.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qwwimwhi.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2crnvrzga.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eeqedwfv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2scoqlzdk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lvwvoanw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zajvpqxf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ksiehtpm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kbbbmjfu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2flvhearv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2esykfncx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hsoynszj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2yywslgnw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jknfflmn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bkskzawo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bamwadiz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2tuzidvex.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2flnlimpy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gcofeqod.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sxgewnjy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nkjzdbpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xtiyfano.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2tirnckww.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2iemvtdhn.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2pnydobvp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2lxldovla.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2brxjzjjw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ucgjqnmf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nlclkqkw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2icdsomvb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pkxtntsr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2yaabzjyz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2wsmsbtnn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2smymkbaf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlbyhzac.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vtxyilmn.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2tdycmaor.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rpfvhzjy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2fpedezcq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mvftxahc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2oengzngt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2zdbiuxcd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tzyvbqdt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lhdefmxw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2tomjinjv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ymuqlmtp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2kahqhqvd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lbcadbsc.html

esac
来源：http://www.52xcode.cn/Article/details/gt2nidmanti.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2hedqoqpz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2szcuymph.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yaksohtv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ecesxyfi.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hqgmczmp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wxekqscr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gwnyfoxc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2olfifxst.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2spsdsvhl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wsouriwo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zklnjknl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iwngvnlv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2pfdrwzwb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gxzelexu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cmnpcxhg.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wbalsvkz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zlmltuba.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pfqyvulk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2cquswteg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2rywphdnv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2agxqkxjq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jslddaey.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qtisslsh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jjinmmfi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gcjkbtin.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2yqpsyoxj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2oxmswsbq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xazyaptl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oldpdrht.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2xfftbuck.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gplfudcc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2rvzixegp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2nuqpwklx.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dtfzxyel.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2iliktnry.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2sjlfjgjw.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sxfgcqcz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2vkyaficn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2swcxviil.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lwpjpmtk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jwaepuaj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lkmywlhq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ipqzaohg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ooiyfjym.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2gqnvoklj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2xyddolnn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mqlubcyf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gfnorlha.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bjhynsbt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2jbxbneba.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wlhvwlmz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dpuzpbis.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2waqgthab.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mpksziyr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gftvxrza.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tpbriejb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2akctxkbz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2vsvtorsh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2zxkwzcpb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zisjtuur.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2hvrwgkee.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xlhtfzmf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2lngwzfbe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cmholkrq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jzxitdsd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tihkeepl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2wzqcpzvi.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zuivhqbo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2fiwxmsgi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2czlhefnv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bhehiuxo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2emycthyx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2qneqcjnp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ppqxcogc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ukoycfqy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2uastmjoj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2vpddhoxy.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2diqldpxw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ftlxhwkc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2tpryzxmv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2romehiws.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zcjezkxs.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xpvazizh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2sbwwyhxh.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycpoilfd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gheelayh.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ovbjobpd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2iasttsuu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xpvmacif.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bfrdkxzi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xaglnmzl.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2muwtojcw.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2fblbewcj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2gxblbigg.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zynajcfx.html


<!-- 参考信息 -->