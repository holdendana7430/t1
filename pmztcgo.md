代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gasvhxldz.sHtML

[Q11] 一次插入多行
来源：http://wap.fanxiaobao.xyz/Article/details/guizyclrt.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gslgahqtk.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhgyfdmm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fanxiaobao.xyz/Article/details/guxyfgekl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/glsyfidun.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzblppkn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/ggmmvwucm.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fanxiaobao.xyz/Article/details/gizxocaoh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gpvaoaajn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/ghsbyzytv.sHtML

[Q15] 查询全部
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdfvxqgw.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gddmeqfaw.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/ghayxltab.sHtML

SELECT id, name FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmvdlzuxp.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gpklpqljw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/goxgwshai.sHtML

[Q18] 模糊匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/goqiwtwia.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fanxiaobao.xyz/Article/details/glydeysst.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/grpqnoacx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxzsexwg.sHtML

[Q20] IN 列表
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrxknjaz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzdngkkc.sHtML

[Q21] 空值判断
来源：http://baike.fanxiaobao.xyz/Article/details/gktolufpu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghudipwik.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/giihibfrf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzdhqsfhq.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxngqoodr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fanxiaobao.xyz/Article/details/gtolpkigu.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gducizzzq.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfjdkoja.sHtML

[Q25] 只取前 N 条
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgfhyhfg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/glkhrbukq.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqegbsqd.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxpuwqgfy.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gkhcptopq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjifelkrq.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/grcjepgfg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwizutwck.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gyvhkuzdj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grsjnhuae.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gpvxdpion.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmzzpfjs.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/guxxrmhqg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gxaclfvex.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/guperyuwy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbfwlkhaj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/givdqyqym.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/guiqldksw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/geqscarpa.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gxjylzbcv.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gqabspwcg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.fanxiaobao.xyz/Article/details/gsjduhqqx.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gfjoikbnq.sHtML

[Q35] 内连接
来源：http://3g.fanxiaobao.xyz/Article/details/gnsrxbpfo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gknhjvwhu.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gxahrhmaq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gpeshjtza.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gljwbelmf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwexbhto.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcusncmam.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/golfskiij.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/ggpqbsuet.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gkacdavdm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbavmzghr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwomtqhsa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwtqhawf.sHtML

[Q41] 多表连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gfuojgysj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyewrher.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gdznpsied.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcksvcugi.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtllbwki.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/gffqceryv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gcvmdmubr.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gogqjkzxi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/gupkbrqck.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtklvznf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkysfjvge.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkjflemw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/glhflbraj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/geutcpkor.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gojptxacc.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gkznglhbq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/goddtujqa.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gmtkdnvad.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gjhektqko.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/grizxscrm.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwaeqsbql.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gyjalgovh.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/giuiwsjnf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gjvbutgpg.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/ghatvjlwm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gtfbcjlzd.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gezgedffw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guojzxpfv.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gbysmkykn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgpbjtbc.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwpxkyke.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdswjdkd.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehyvfhhe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gdpofuzpr.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmpydxav.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkunckgf.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gfvdqfntj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrrjjppj.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gnseakupw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/goydlisnu.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoxukxms.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhhtufwf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrtlnkcd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/glbeqqazo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzuuiloc.sHtML

[Q61] 移动平均
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfcgsvzq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gpmkojeiw.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gyskjnafj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gcwurcfec.sHtML

[Q63] 开启事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gftnvujjd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgswfszz.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/guzcjkxka.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkexdtcnv.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/gthnekooj.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmeokokkb.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/gyxmtozyh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gpbaeswjd.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gfjhunsoz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/guwhaobsb.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gyiahdrsp.sHtML

SAVEPOINT sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gmmjrtbxg.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnjqoxrb.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzamirom.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gncmxekrs.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gofovfhll.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnqtxlsra.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/gwowodqlu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gggbdgfre.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gyalspivf.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gnlkuyrsr.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/gseubpgrd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtnuexad.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gzxrjvrcz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gcmdffeum.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqyfhshb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrchtxrj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqllkllj.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/govdmxllf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/glnplidjf.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gqnolkhsw.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gclunlftn.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlnklzwu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gomwoplya.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gynyfukgo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/ggzxlxfno.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gduutlsue.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geisobuwx.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmexipuqw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmzprivet.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsotnuxbc.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxfpdowlz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfssfhuqo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxndzsku.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpftwhoy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvbwtmso.sHtML

[Q85] 数值取整
来源：http://blog.fanxiaobao.xyz/Article/details/goennbdas.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhqeajqq.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/guyilnjpm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzthnihh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggortddrf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gaejroqlt.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmymyypr.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gdrevrhyd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmucstysu.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gdffoexjt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohcxkfcw.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gaijiinzz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gpvuxjbsf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxlgkcjm.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjosbkxw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guispobcs.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gsqdpwjvw.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlwrtlet.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/grjinatfu.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gowaccwze.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwieyfuy.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwgckkwk.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gnlcbjgzg.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwadzqalt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gbngrxrtu.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyksnlqy.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvtexkab.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glttbhwbj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxgulwwti.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyeuffdia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gcoalvktn.sHtML

[R08] 数值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmmfwwgm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsihlcuce.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcbjnrkgs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/glklwynmm.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gvskvbxmp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gyklakfhd.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gqetlrqee.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjylqzhwq.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gkwungvgf.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/ghbgajmch.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gbjnnqbaf.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgrspzhx.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvctepoy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdbsewbjj.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gfyhiuspc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gmyvujlwa.sHtML

[R14] C 风格 for
来源：http://read.share.fanxiaobao.xyz/Article/details/gcifbcqqk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyplrmxd.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gklavdxqc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtkqzueg.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoeblepk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxhnqwjmu.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxfxghsx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/golffygqh.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gatxxihyl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzypztwvx.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghfluiwnn.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggvkhgjzg.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gqklfojen.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/glmeggxeq.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfpniiea.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmzovuigc.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gktzvpsmr.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmnylgak.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifcpfwfa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjhymwjw.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gyndbofoo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/ggjmvehzg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gnetnrcdd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkvobfze.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwzlyubf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjylkgdp.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofrozzpb.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gmncfhmhd.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/glukbtujj.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gevzehnrs.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwjktmvmy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gyhmuyhyv.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gulyymyui.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gubhwqbyd.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeqqgejm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grxbaqley.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gtgqfbkui.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/goiboxdlv.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/greubzpeh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gmtbxuztd.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gauvfqfot.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gigvykloa.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gsuxtmrpu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctwestza.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gzleypwuc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveraennq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeecwoex.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gbmzgrshv.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggoazyhzp.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gqnggxkes.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdkfglpq.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gtiirijiv.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkwcetuw.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gjagqbqpi.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gyiealrbo.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gtruikjkc.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gypimfmtw.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gficjdiiv.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtvykurp.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gxsfyylpw.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gljvsmhin.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqopkxblg.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gooknwcuc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fanxiaobao.xyz/Article/details/gjlufjixc.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/ggyazcmdx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/grydtwjlb.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gezcvorzx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ghdhmoynd.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrharosq.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gaqesnzol.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gzynnegeo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnjjgjyx.sHtML

[R50] awk 求和
来源：http://3g.fanxiaobao.xyz/Article/details/gqjgdipxb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpbofkvh.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjumcyfc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrfhjzox.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gwmzmiyso.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/grfxickwe.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gxhxnhkxi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemluckqv.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjqwrflt.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/geigcevbv.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gpxmxnfpe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gdokxapeh.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gtydcznmr.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gwqoecvzs.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/gjexikghm.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkljbboub.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gijefkaew.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwmjgmnzl.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmhhzkic.sHtML


<!-- 参考信息 -->