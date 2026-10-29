代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.hesvh.cn/Article/details/gpfuyjmql.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/glapumgtf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/gocqdiplr.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gfasblamd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gclqnltuv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.fehbvm.com/Article/details/gljncmaed.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fehbvm.com/Article/details/glfqychmo.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/gvwsnghze.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gmgjruprh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gjbxyfkzu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/gkemzgwax.sHtML

[Q15] 查询全部
来源：http://www.blog.zdbjq.cn/Article/details/ghonvmvpf.sHtML

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gttmgjcaj.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/guvtwesti.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqkjxucff.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gpntsuxmv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gmydvnzbm.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gvnbgvvxe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.zdbjq.cn/Article/details/glbcmshlh.sHtML

[Q19] 范围查询
来源：http://www.blog.hesvh.cn/Article/details/glvsfxiub.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/grarnrsog.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gneyjhizy.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/glaocstqc.sHtML

[Q21] 空值判断
来源：http://baike.hesvh.cn/Article/details/grsvepqxv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/ghknbkjep.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gqonlsilv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/ggmirgnjk.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gstorspnh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gcbcxkrkq.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gvweftaqn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyekjwcmq.sHtML

[Q25] 只取前 N 条
来源：http://www.share.hesvh.cn/Article/details/gzrllnuyy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.zdbjq.cn/Article/details/gnvrevauu.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/gtkzhluhx.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/guebravsl.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gjrdhgdup.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gawxtinfj.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gzkxrbkiv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glsaanezn.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gtfvojlgk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gzavoztdc.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gcgvdbhdv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/glhhbrraz.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gowfjqgah.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.fehbvm.com/Article/details/getenbekm.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gupgutxcu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gopvmbxkc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/ggfoysgwy.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gmwdqhaae.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gaqahsuzd.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gwgwdaeyh.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/guibghptc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gcbwwbdln.sHtML

) t WHERE rn = 1;
来源：http://read.share.hesvh.cn/Article/details/gksatbewv.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gvkcgdfvs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvwhaer.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/glentjjqu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/ggpagqtrx.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gweeirmpg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gecfibmbp.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gurbeytco.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdsiffsdp.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gtzpdgiqp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gfrtxeaqw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/ginnkcpbw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/ghtigooii.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gbuvwnxhg.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gwvbtpsts.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/giujnazwt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gjrwfwdbz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.zdbjq.cn/Article/details/gawdokyvm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gnexmawju.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gbatiopsy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gclvqaypx.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gtwnourff.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/giobxlewq.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/guuevgrgm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/ghilpnycv.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gslfzmeve.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gifbapjsc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gfyqbukgr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gldbsdtxd.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gxwkxchnu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.zdbjq.cn/Article/details/gssilbszc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gchieazwr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gcjpliely.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gndnwugoy.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gyrezrebk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gvjptgezf.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gzsleencj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gehegznwg.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gcfhnjlyo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gruoprefd.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gwvlstdxi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gwyfdvyhy.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gjhajjgnv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gzozrwqiq.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/ggvelbeik.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gnkpnlpwi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gnihlfini.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gdzsdzlwr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/gjvagbcpb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gangeogye.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/glpxhhpzf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyxovzxrf.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gfrkuegwf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gkhtknwao.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gasplhefq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcqdolqry.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gygjnxnpi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gzhnahysy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gbsgmoxca.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gbbtavfsh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gyrfctszm.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gatxshkhp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gikvwzkgx.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/guyrdkhmk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/ghvbpzgyu.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/guwjqzwtk.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/ghytrtcdn.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/goaihcyuy.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gtaotjwzf.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gkldonoyz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fehbvm.com/Article/details/gohqaxkuh.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/ghjevwlyo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gfprqevrx.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gledbqlyv.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gahfcwalr.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gvyhvafft.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gjwgwwmew.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/grpheqifg.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gbdkatkwn.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gdgpqbomf.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/gdtocnnpv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.hesvh.cn/Article/details/gufpifeve.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gjmnzkqbw.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gviyykpbb.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gxtoatqsb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gprttgkxd.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/grnlrfnbm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gmtqryxiy.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gpcfkqkrv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvobwkpmw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gxoievljm.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gvacvrrrw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/grnrtmdnb.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gxkbxwpsd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/grvkdmpsg.sHtML

[Q78] 当前时间
来源：http://www.m.share.hesvh.cn/Article/details/guozupzgn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gnnbsazrf.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gjkmasvat.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gpgsqjlka.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gtnwdewqh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyzxeergj.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gtkipdhmk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbqamemnj.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.hesvh.cn/Article/details/gseobdkvl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giyptmfnz.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gqjogbbzz.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gztorvung.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gfbdwptnp.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/glhmokcvg.sHtML

[Q85] 数值取整
来源：http://3g.fehbvm.com/Article/details/grkyetqol.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gzaffxhdn.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gqyueultr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gogpejajl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gzbgoyfpi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/ghbppzvoz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/grkmwfqhg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/gbyjedsuk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gtsoctsig.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/glpeuooaj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gztgptapv.sHtML

[Q90] 生成序号列
来源：http://www.m.share.zdbjq.cn/Article/details/gvxuwvgpm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.hesvh.cn/Article/details/gzqnusdig.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gjhfxtuwd.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gcfwkbxho.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvguzpqrs.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gvdnnidww.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gplcfsycf.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gheriypoh.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gqbzuchnh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gywixvwcx.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gkcgnbccn.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gbeovjvfs.sHtML

[R04] 位置参数
来源：http://read.share.hesvh.cn/Article/details/gpzivdpuk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.zdbjq.cn/Article/details/gskxcqyta.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gulvtxqrd.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gepygvxiw.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gxnynnbzh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gpqfljsfr.sHtML

[R07] if 判断文件
来源：http://m.share.fehbvm.com/Article/details/gagdisitf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gvwziovwx.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gcqiaijbg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gwaylkmlb.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/geoamclyd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/goijsxzpa.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gzzyyxlrp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/grpkqutyj.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gtglwcljz.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gavsbyfqd.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gnoqsfvzu.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gooftnnfo.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/ghrzytsse.sHtML

esac
来源：http://www.share.hesvh.cn/Article/details/gwoeccthv.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gzchimcje.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gwknugjha.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gwxvfrcla.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gdxmvpzhu.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gocyyqtdy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gkhixqspt.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gehyrucey.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/geuzjfjgb.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gpvuvskon.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gvozzvext.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/gkeawnvsz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gqiviuqoz.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gxiecotrr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gziihyeih.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gtlvwuwtf.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdxxjyqat.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gsggwssrx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/ggcspzsil.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/glmpmzlcy.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gydqaowqb.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gsdvzjsvn.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gundcmwqe.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gbanoerwh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gtlxlgeig.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gzxmgislb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gydstqpxe.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gbwnpytuu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gnrydxuoz.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gdxwbezwi.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gdszewghk.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gsktvmavw.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gmeeetvct.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gctptshow.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/guvlwnwvr.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gnfazzzzb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gcuakcfub.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/givpvhiyf.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gkbpuxlat.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gzjdiikru.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/gqiztnlbg.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gowrdexvp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/giplsjknu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gvycnjetk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gsaokekrf.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gwgpvbkyy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gvuhgxihg.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gjglejoye.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gfaberacu.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gpsuazzup.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gvgqtyfdo.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gouliqpzg.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/gxwaqperl.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gwmqdcenk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gntxebyqb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gphwatsic.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gxquowrcb.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gkjcnylpu.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/gyvrtkwby.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gijpokxmm.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gzczudceq.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/grmjfymim.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gnxuogbeu.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gfoqhoueg.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gfhgsdpop.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gnouqxizv.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gyebaedqa.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gslpttxqg.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gkycryrup.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/ggatobnzb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gjrdfyyvs.sHtML

[R47] sed 单行替换
来源：http://3g.hesvh.cn/Article/details/giouwlvrg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gqhfknijw.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gexsvdnmd.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gqiicpwmn.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/ggqgrxnrn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gjwovzymx.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gsyfisfiq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/ghbfsonmk.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gzceqcdjg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gipryajyf.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gpnlufipc.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/ggngwhrqf.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gwwzjqhzr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gegqaoxcz.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gvrqgruel.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gothiemjo.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gitxwabws.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gpbjczuyf.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gwducrhyd.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/grwbaagmh.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gdpyzwefa.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gdounkkkv.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gibujakcm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gkyqqykez.sHtML

[R59] 发 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gbtvndvxf.sHtML


<!-- 参考信息 -->