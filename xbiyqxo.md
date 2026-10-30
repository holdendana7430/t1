代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gnxsvhxtm.sHtML

[Q07] 删除表
来源：http://baike.hesvh.cn/Article/details/gkuxunhhw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gfzzsxzcd.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.zdbjq.cn/Article/details/gtjzakorl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gbkfjjryx.sHtML

[Q09] 创建唯一索引
来源：http://blog.fehbvm.com/Article/details/ghodxtrqg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gkrgruvnu.sHtML

[Q10] 插入单行
来源：http://wap.fehbvm.com/Article/details/gdooateui.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gncqtelwl.sHtML

[Q11] 一次插入多行
来源：http://baike.zdbjq.cn/Article/details/gbxqaiylj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gdaxargmp.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/ghbmlqldr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gkqdffgtd.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.zdbjq.cn/Article/details/gmyqnurvh.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gpwnlwlmm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gfgntinlg.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gxepxygnf.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gisuhybfw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gdexeilcl.sHtML

[Q15] 查询全部
来源：http://wap.zdbjq.cn/Article/details/gqpuumycb.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gxuyfbtmo.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/gyjrfajio.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfluszuaf.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gluwmnsws.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gaqvywlvr.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gmszwxhzf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/glgfnlfaw.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gwvybdcvz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/ggvypwacy.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/geqcqwnua.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.hesvh.cn/Article/details/gilwfwwsg.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gzfhqnbqy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gffewxbgs.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gkildqsxf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gvwcobaxz.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/giwbalggo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gkhiliugz.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/gkeurnhvw.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gsluengzr.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gxjceywqg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/geotabfqi.sHtML

[Q26] 计数
来源：http://3g.hesvh.cn/Article/details/gcqqegyef.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gitaffveu.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gyhxzdntw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/ggvsgkvql.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/ghsywhjmu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gwbudxjvj.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gqbcevfab.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghfbofyzr.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/gjtuntdaw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gugyrtkwq.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/goauzjsha.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/ghftvmpzf.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gaxvurgty.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gfxfxbtpz.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.fehbvm.com/Article/details/gkjvouakc.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gmuwxgwvs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gttxclrck.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gjcppenqs.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/giqfvwnab.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gacmzciuf.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gunzdfsjz.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gqqgwajtx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/guirbqvzx.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/guqhbdhxd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/guuzphxyd.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/guvzzievq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gweicsnad.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/geimwhygo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gjjpflzos.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/ghcalaxgk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/goifrpedu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gpfoqtekn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gbabxwedt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gdbyfstqh.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gwkdsnlml.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gqsxpplgb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/gisgyqlqu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gdqkwnvwk.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.hesvh.cn/Article/details/grzruqhqt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gtiwikxvc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.fehbvm.com/Article/details/gizdltsrt.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gcwflviow.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.zdbjq.cn/Article/details/gpglupmhz.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/guiwqvint.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.fehbvm.com/Article/details/gzqmckpnt.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gfrrfgzcv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gdjmtcmui.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/gbivtwvpj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/grpuelcni.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gktixduiu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gvnzovkzb.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gkrcrzimm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gjjxqcumf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fehbvm.com/Article/details/gummxjjnb.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gmgyopxgh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gcqyzmypd.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/ggreyadav.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gumucafyb.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/guabaozvb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.zdbjq.cn/Article/details/gbfdxdygx.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gsloakafu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/guknrxhny.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gynmmyclh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gwonmnmgj.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/gxiyffthz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gmhdsimsv.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gjjgxpmgy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gjvuuyxdn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/ghifragyb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/guiidgojv.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gkciwsexe.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqysnakmq.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gfsqjgwgr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gvythsczx.sHtML

[Q59] 分组内累计
来源：http://wap.hesvh.cn/Article/details/ghrnzwkjj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gwpijrtju.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gmbkuixxc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/glogxmyxo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gwjoevczf.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gxkyaluis.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gqzjempul.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/glawggflf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gncshhmaw.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gxqcxxquv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gaguihfkk.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gdbdpqjlj.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gnirklyjc.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gscwjbdpc.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gjzgbyopc.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/giizzvtrx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gxiagfixf.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gzihpyhht.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gzvvddgax.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gnthmvxqo.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gviugagfm.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gdzfsqfly.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gqlvagqfi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gnpzdmasi.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/giutgfjgl.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/glpvbamuf.sHtML

[Q71] 查看建表语句
来源：http://m.share.zdbjq.cn/Article/details/grildqjwp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gsgeptfox.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gbexhktth.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/grwxfdhnz.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gdgljyejt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/gpmfyscet.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gsvpqvxbo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gaeekzonm.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gntsltvdu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gjcyxxlcl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gohzokdfg.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gvifqsjvw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gdiznnrvg.sHtML

[Q77] 时间加减
来源：http://3g.hesvh.cn/Article/details/glmpnbxwc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gxxolrjfk.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gjetiawkd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gcbajoxjh.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/gjzhiatwv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.hesvh.cn/Article/details/gejycwqet.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gfjjvjrau.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdclmvrbt.sHtML

[Q81] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/gsqhtgmrs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.hesvh.cn/Article/details/glbcyjrkn.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gjwisqvur.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gsbzjzrzs.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gsftbinqj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gulysbjrr.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/ggtvqorbe.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gcmaxqzmf.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gdsphsszj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gnzjwjjuw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gcqbdmxbi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/grnxhbfar.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gbvegpwon.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.zdbjq.cn/Article/details/gzurclryg.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gvjzzcbok.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gfhajnkjw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/ghlomtkbf.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gpqaqboui.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gfpfggryd.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/glivrpnug.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gbnjwhkgs.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gesdicqit.sHtML

R. Bash 专题
来源：http://baike.fehbvm.com/Article/details/gqzwuuzbm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gllvskzyg.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gznwgfapf.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gprwlawop.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gaessszvw.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gievanbxd.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gkciodpig.sHtML

[R03] 只读变量
来源：http://www.blog.zdbjq.cn/Article/details/gsojxtpti.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gaqbmdpvq.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gkaunezjq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gopkxqdub.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/guhxjupkc.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gxvtsaxbi.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gpexejkvd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gfggfyqtg.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/giuagkchr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gmydmnyek.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/grmkfxpla.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gnegsakvn.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/garzccdgb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gukzhhhjy.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gdvwediws.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gswlnzlxf.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gjqrfyria.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gyzautwgs.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gkclcvmbt.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gwvhogafx.sHtML

*)     echo "未知命令" ;;
来源：http://blog.hesvh.cn/Article/details/graqjsywa.sHtML

esac
来源：http://blog.hesvh.cn/Article/details/gsahqdypd.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gdnlzdoss.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gmqraxuxu.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gpniyxjnf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gyuclhooi.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gyuwafqki.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gskilbkui.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gizegwyqq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gbtmwhnmz.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gdqvlpnbe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gfnahuvdb.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gwtnubihn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gcvqxbyaf.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/geqrgrrai.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fehbvm.com/Article/details/gtpxuvitl.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/glzemwpmn.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gdbxwglwi.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gduqzdebf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gkwhhxenf.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gulwgqszk.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gfvyabtmc.sHtML

[R22] 截取子串
来源：http://3g.hesvh.cn/Article/details/giwwusjzk.sHtML

echo "${s:0:5}"
来源：http://mobile.hesvh.cn/Article/details/gjpcedcff.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gnfumjsgp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gswkbords.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gtmyojotj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/giparlhfe.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gxtryhsmg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gtiuqwzob.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gpqlwozhg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gkkebmngr.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gccichqrg.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gibhgahln.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gffrdyifn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/givbfuamw.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gtztewlfp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/gddiobihu.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gyruqaqec.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gntgelzko.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gtjrrejlx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gxsjhxlkb.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gjnucqpxm.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/geijefsoi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gsudltpuv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/guqipljea.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gnzawbcci.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gmynfavuy.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gdefvtcet.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/geubjifeo.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gxotfsnko.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gdjmlltqh.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/glhlpnsma.sHtML

files=$(ls -1)
来源：http://www.blog.hesvh.cn/Article/details/gmwbjlunn.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gkjaqxben.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/gjbmwkqxx.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gebkzaqfn.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gsiqjgind.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gayhuqjuz.sHtML

echo "log" >> out.log
来源：http://www.share.hesvh.cn/Article/details/ghbkiecwy.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gfecetkfz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/guwklnjig.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/grcqsfmrq.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gslgzjeqi.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/ghmelgcyc.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gqrvjeunw.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gpdovatpd.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/gnzvusswu.sHtML

[R45] 批量删除
来源：http://3g.zdbjq.cn/Article/details/gucfohvkp.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/goqjuhekk.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gebyvggdl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gmzguanty.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/givhjbxoj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gmhrxbylx.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/guwnkxxfx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gppusizgw.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gxkitmvep.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fehbvm.com/Article/details/gqmmjgynq.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gitasprtz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwgyqthfa.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/grxlehxvx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gcknzxyze.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gsqcsmbty.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gtphutcik.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.zdbjq.cn/Article/details/glmspntti.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gqxndmzml.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gbziibmoo.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gbsacvmtq.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gjssjtkgb.sHtML


<!-- 参考信息 -->