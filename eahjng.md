代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2grevlhhi.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2efmgegof.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2pqxnixjw.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2qsykbrin.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2vbhqfqlp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2vsnhyiyq.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hjnwhnhu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2lzxznttk.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2klsxqglm.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2hlclylpv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2catpudiq.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ikvsorio.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kyqkgqjm.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ubbetuhd.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2anbemqyt.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2kugstpyj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2yvpygbqt.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wfivffgg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2jrpicifo.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2kgfzqurg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2vybyavhi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2tclqxedh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2opqtwuqv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tvaynerf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2yjmnzjuj.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2tnmmkbjy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2vrbemhwt.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2qpswnhrg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2bqtraqry.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2sltggcyn.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rdrmcquh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2jzuvnhkx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2jbxhuryf.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vknfmwiz.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nfxzpeqp.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2snxgabrn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zzifnxhj.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2swwinkdy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dhhfkbtt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2swxmtzbo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzmkcumk.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ixkpzdhn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mzomirxp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qobhvznf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2esjitphw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2qqfxwaco.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2khlbhaba.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2bqkcloae.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2dqnvkvod.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2inbiwuaq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2yrfkwnfd.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mjsvaayb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2idagdknd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qheijxsq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2dhwmmloz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2shyggqif.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ozqmsxnm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gqdqxrlg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jjgsyzji.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dxdmleva.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ftoumqpc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mvtdmmeo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hhocvqfq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2oxxjeiyu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2havkycxs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2twthuras.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2wvfwlbkp.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ttvupkod.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2aohbogsi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2tbolxvts.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2umspqoor.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ygobkqef.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ncocscrr.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jxmvfsti.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2woszkefh.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2yfelfqnn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gvsxepjs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2olfseegw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2orvipnpj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zkeoemwo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jscchnkq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oahotfar.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wdraoqsd.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xkkqhwwb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rczbynjg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2tetfibxe.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dwvjycji.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kqcmzrsc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jiqnuxyp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ukmthjyo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ikkhzlta.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2qwouzjii.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gvecowgz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2libjlsia.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iqogxlze.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nmvkdhxo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sfineeij.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2wusokalc.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2gtivzzjo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2chwimipf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pfipctgk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ixixbvpj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wuvqpvye.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mznwlcyi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nmtcqpsl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2oqcgiqis.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2awzgkknu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pdzunrce.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2oiweqxsq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2henkdvcb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2jxizmeyg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dcdwvjlo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bzrzhbyv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2blodgkxe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ipzvotkp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qqnnmmbe.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2yezkoiid.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2djdvzjhm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2xvphutwo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2nkycsufs.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fhgsursr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2iyyraimd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2yhzypfku.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lyvymwgg.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zgruxrcf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mlbwscnr.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xdfockia.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qjauwenm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2tblwvrrn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2iaznxgnr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qwruzonw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2vtsbuqmq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwdnemwq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gfbcpxyz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2exaqtqzg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qmefljem.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tyvyfbuh.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ttschsop.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hsughzug.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zrokzjje.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fzymmrzw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xxyqddpg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dppigezg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2xprgyxke.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lqsascad.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2cyxprlxm.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uakbypct.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2hfnrkvex.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2yoxjsxiv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2qgiqsqzp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2fcoaenaq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dssfjxme.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2guejlqqo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ivmlvvbs.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ihuuboyo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2voacjzvo.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2oliyjdqi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jrirytgx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2dhqobvol.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dppoihzm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jygjzyce.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aovbqngf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2fzkllvot.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gkhgghbu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tjvfawqv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2pnytygis.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zifuslis.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tvyrcvob.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ulefqrzn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qkkeeqbh.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cyzmodwo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2uoedpjps.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2xnkzttmt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2xirhphrf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yijcjyzh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2klbiqppd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2fvhsqhnu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fcfwkysa.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cchzfzmb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2uskmxdlq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hrhaceql.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rscdqrnn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cmrzqseb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2bgojnztm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2msrslogw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2oxhjdgrz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2qypdbqoe.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2chgaowag.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2ltwpyell.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2naczqwyb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nemxpxss.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lqpbuftb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2biyzszai.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lobjuqxx.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2mcnqlmcp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2utivvqxn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2snwcqddj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2osqiglwq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2crprzihs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lqkpdgxb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rztpzmgh.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2inywgvcp.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2petqojjl.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2brxizbkd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2okoltowm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2oqvqnylf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2cfxlfiqy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2epixnyhe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bwtptvgb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ljtjpfrh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2quvnrowr.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2royqunwg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zgxglffs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2edwkezqd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kclxzobg.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zlprmown.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xfixlxjo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vrofzmzg.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2snkdaopb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xrfuffkr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2fdkqcndo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2azlfwqmm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cogenwmm.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xqphbqaw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tnvnlayc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ipwqemdp.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2majspaqc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2vxhlnenw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2zacwnenz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2yivlsxjb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2yxxpemwz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2amtdivnc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2uahxxijv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ekfaenqd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2abdylpsr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2qeelwpgg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wcdpubly.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nwjporsv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wdktbrzs.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ogtnjvdw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2lvtcmyfv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fvmaxqwo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2fcvxyhxn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jsokqnfn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2mtqluuvb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2pnzsesrj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrgjjlcb.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2nrmiyczz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zexrbobz.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wvgofrso.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2peoqjeed.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2rycuynbh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2qfkaqpzh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rdvqsulr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2syhskasb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qcsopcot.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2uegbhtle.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gpfczbfh.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2crfsvsni.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2zrcyxbnl.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cgluhjiw.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qbdokzij.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2frbftcal.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jpvsohlz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gzjnkebb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pleyuomp.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fpejcfgd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qreskjms.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2karwlrmp.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ihdnfzur.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2otcztayg.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ayzuvpwn.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ataehauv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2oytdgewv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2yvhdzjke.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2osxpnbfc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2prgysgll.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vtgljcfe.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wbanrywy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2tpogbjsb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ugenxfwd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xfmjrchr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2efkpeaes.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bnnquemb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hhoaqgdc.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2tvtalnuy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2acawsruj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pdoetgsa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2idotbnai.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycemrzcr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dmohptmq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fsozacvo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dfldmszn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nnnuypbs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2toqtgjev.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2bpofptbo.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xfrlxoft.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrqqsbid.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rurbsxwy.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2joxzfcqn.html


<!-- 参考信息 -->