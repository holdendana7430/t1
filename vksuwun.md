代发 wailian999

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtjlaqoy.sHtML

[Q11] 一次插入多行
来源：http://mobile.fanxiaobao.xyz/Article/details/gvreeiacr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gmocppfpn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpjdfkfv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwqmabfj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fanxiaobao.xyz/Article/details/giszquoyg.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuzfyshk.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gjyhoatbh.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fanxiaobao.xyz/Article/details/gdudinofo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.fanxiaobao.xyz/Article/details/gahxfnfkp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxadbfnhf.sHtML

[Q15] 查询全部
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkioheyx.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gurrxhqjg.sHtML

[Q16] 查询指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gpqapcfop.sHtML

SELECT id, name FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmtibylui.sHtML

[Q17] 条件查询
来源：http://blog.fanxiaobao.xyz/Article/details/gkhgndjda.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gajtcysty.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdtwgpyf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhxaesrm.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gorfqlwfx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/grrchylca.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gqstkamot.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlflioxv.sHtML

[Q21] 空值判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkmcrmim.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduywjval.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/glgxvlaij.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyocwwqfc.sHtML

[Q23] 分页
来源：http://baike.fanxiaobao.xyz/Article/details/gcumxtekm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwieglvjl.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/godzgqewt.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkumnjphp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdsmwojy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gaiyimmox.sHtML

[Q26] 计数
来源：http://blog.fanxiaobao.xyz/Article/details/gghxzbazi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gtontldem.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbetsnny.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gningttod.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gwussztzq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gfgaxxofa.sHtML

[Q29] 最大最小值
来源：http://baike.fanxiaobao.xyz/Article/details/gcsitpwqe.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grakhtker.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsatepwwh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxmowjfx.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtphnklv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwtfyndt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxhchrsm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtrvuqla.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjkyyesz.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqeotkljn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gmfejwfkj.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gdjczpjix.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gucmumuab.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gufpvmijd.sHtML

) t WHERE rn = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqeidpxpm.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyfsnffh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxppbyfax.sHtML

[Q36] 左连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmmotrsv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gssukqzkf.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgxxqfoq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmfnjofnb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/giywibbxp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpocqoiw.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fanxiaobao.xyz/Article/details/gjnrbkxyo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gmmdgwsvq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuwdaslu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gtwqfjufd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqudspvzo.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/groscdeee.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/ghthbepmz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gbiswkzvp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gcfyebjtd.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fanxiaobao.xyz/Article/details/grnskncyk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gyibdkcjy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuqgdwvb.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsmjgssp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gtmgjduce.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniobaapq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gxdkyynjy.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnhzvqof.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gjnicsgeo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gntcodzen.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbysopww.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grkmmxzzt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoorhusy.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gferuifbm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/gnwrcrpbk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gvaepfoco.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/ggvdjzuth.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gcgqpnoaw.sHtML

[Q50] 批量更新
来源：http://baike.fanxiaobao.xyz/Article/details/gyukqlsom.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqfhgdau.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gehgyaffo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkrmpqaku.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gakosxhxv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghxuxqgal.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gziysqctk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxemzdgx.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcttahqwo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoyitqsb.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzscuthay.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gflxkkdnb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwrgqljh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gyjxcdlsk.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiarslur.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxucrlwde.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjrweqsa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glttzakvq.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gzmperelk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gfxwwhvlw.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gdeptdxjq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gblfgghee.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrellogf.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gavxvsgrl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gcoqfvbfq.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gnfwbhqro.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzgcfaeq.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslrjahzl.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gxndueblc.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqoaafdqw.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gpcqeesss.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbnlojvn.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gasevwkxs.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/glwobovgz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.fanxiaobao.xyz/Article/details/gczcawuou.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gccibkwar.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqotdszq.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsfkvwbp.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/ggalrgzgt.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gvpxfplik.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/gnsohygvs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gvacvymlr.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstuuvjak.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gftlxqsxk.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnlqvnjp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyhbfxdo.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gjynrqbpl.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gixlaxchv.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsluxaqy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gnukhskmi.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgtwwesv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gffdzvizw.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpselludt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglmtbvow.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gpngrjpeu.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaakznxo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaizmwnb.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnaguyob.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gulxkktci.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwvlggva.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gixuhayrg.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gxekorvlk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgpwapom.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzxpwxpa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmawmuicu.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjomuuju.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpuxwojif.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtekfhlj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grrcdsaax.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/grpnfnhrl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/guwgvfrej.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxqtfwwzd.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjwvwypda.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxcyeqcs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gedvcqwdw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gbptosulr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gqspcuvov.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gobrgobfd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdsxbaik.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxcjngqs.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gvktsaegk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyaqvwuj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbkvcgke.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/grzjeykrr.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gmiueevdf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjldllotb.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/grvdbcadq.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/glrjgdvej.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvyryqqd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqdfkqzk.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gebpdnegs.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gkdsoeyyn.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gsfibmguh.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyyjtwag.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gimuugzaj.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gievfiizm.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gbntgdwjn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaejhdqnm.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gvxdtksoi.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gsvcipfmh.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdnlfvmub.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzjoexjf.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwboiwjmr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gufirppgl.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavbimodv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezysmpqz.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gpanwwrex.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/glyvdzrtf.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gszunwibz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhnrmday.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/grtzanrtp.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gbahdgyaq.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbjettjn.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gycglnvam.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrfhcdjv.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwfrzurc.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvlqxitra.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gigefggdr.sHtML

[R13] for 计数循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gljkxhgku.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyjnwazf.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsalwghf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/girzmluui.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmtjldkei.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gclnnfhnb.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/grrgdpomb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggenjdbak.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjoufobx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytsttpyf.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpvaqswm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/giszxazwn.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gsnfzbfdy.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvnekhxwv.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/grkxxjzdq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glrtmjnwh.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gwlkngjty.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghoslxzvp.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gbausmosn.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvoarjcix.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpmjviuy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzksramds.sHtML

[R24] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/glhwecbje.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/guoxvtzlx.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/glbzkshjt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtarlorz.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gewwesqyp.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmujoaow.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghglgwpxf.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyzrpjve.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gqacnzcyo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gileilarx.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gomibdpas.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/grwuhlgvd.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyboicpe.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/grlvzexvb.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/guduruwul.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzaatfkf.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqtoxcnp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gotoszdji.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/glllclxku.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/grrralzfw.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsnazgwj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gssaihvnu.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/gobjqokdc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/grksqdhvn.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gnkdvteez.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/giascjdpa.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdahanvew.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gmbpgqens.sHtML

[R38] 管道串联
来源：http://baike.fanxiaobao.xyz/Article/details/gypqqrjbb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/grpcrijwf.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmtqdxuu.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/glfudsyna.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gmycuzgde.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpopahlso.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gersesejf.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccvcjhyc.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjsxrvqw.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grcxwqaly.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gasmtuyrh.sHtML

find . -name "*.log" -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gvnxrfraz.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gyftdnffd.sHtML

find . -mtime -7 -type f
来源：http://blog.fanxiaobao.xyz/Article/details/guwvoigsg.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxmxldwc.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjlpjvqe.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhtkidml.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gwkqmflct.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsqrgnjxu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/guuipfral.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/galtgpequ.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzbzcgvi.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gntfynito.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gjuwtfkwi.sHtML

[R50] awk 求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gacrlaocs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/giscpuivr.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxffheqw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwprfmwpr.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyctqwghz.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ghovvlzkv.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gkpvaklpg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gtcdelnyd.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/getzcwvlk.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpcfkdodq.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/gejwhefdy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvdckmsg.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gqvftubcp.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvjsnhlr.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gjizmztak.sHtML

ssh user@host 'uptime'
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvbzcfdr.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzcceynsu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gydqdvuhn.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gklwahzuu.sHtML


<!-- 参考信息 -->