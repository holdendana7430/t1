代发 wailian999

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuubmaqc.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gehgaqfop.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gaaljzfiy.sHtML

[Q10] 插入单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsmdrvej.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gsnrgrkdn.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gnoqfdobe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fanxiaobao.xyz/Article/details/gahydmokc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqevbzyb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxzvvozo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fanxiaobao.xyz/Article/details/gqjpgwsyp.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmnwelyi.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzdeiytj.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.fanxiaobao.xyz/Article/details/gdhhsvciv.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fanxiaobao.xyz/Article/details/goviiegbh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gnpysqmuh.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/guqkrvvhb.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfwrrziw.sHtML

[Q16] 查询指定列
来源：http://baike.fanxiaobao.xyz/Article/details/giakefyus.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkxikafk.sHtML

[Q17] 条件查询
来源：http://3g.fanxiaobao.xyz/Article/details/gadflpyiv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjunekac.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gidvovgpc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtgybbxc.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gtuytgygv.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fanxiaobao.xyz/Article/details/gwpslivps.sHtML

[Q20] IN 列表
来源：http://blog.fanxiaobao.xyz/Article/details/gbcobvzna.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/ggkrqrugi.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/geeiwchup.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fanxiaobao.xyz/Article/details/grljaejhe.sHtML

[Q22] 排序
来源：http://blog.fanxiaobao.xyz/Article/details/gxwfobknv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpupknxg.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/giitklzid.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjvhevqkt.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/gngzmlujg.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpuyjcdhl.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fanxiaobao.xyz/Article/details/gvcilbcsp.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzkplcvi.sHtML

[Q26] 计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpvilovi.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjknzhtn.sHtML

[Q27] 条件计数
来源：http://baike.fanxiaobao.xyz/Article/details/gsytveowy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfghindo.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gdflgnxpt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbfqwcyaz.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gimebaexo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gicayrxdf.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gkcjpkuoh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gyenbfdrl.sHtML

[Q31] 分组后过滤
来源：http://3g.fanxiaobao.xyz/Article/details/gfvelmbio.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzcwtslo.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/glgxuglfj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysicxoen.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gatcvoigy.sHtML

[Q33] 多列分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gafdnjwxu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gpdoraovh.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gblrnxmnn.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gftmijils.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fanxiaobao.xyz/Article/details/gawzjjhuf.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/grzljfycc.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/ggkdkmjaj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gronzxzbb.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/geldmulkf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/goijchjvb.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwuxyzkv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnspspzw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/guqotggoo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gmxsshyam.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduvcvgzl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gjdyioxuk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gxhmjpzvj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqebdbese.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkqrtjdp.sHtML

[Q41] 多表连接
来源：http://baike.fanxiaobao.xyz/Article/details/gzrltgwrq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fanxiaobao.xyz/Article/details/grmtqjldf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gfdddxbef.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gmntuyybc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtxexyao.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gdjuqgbns.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/grblnonhw.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtfutaldn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grarebwhf.sHtML

[Q44] IN 子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gaifjtrye.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdroyfjqb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoeexnzv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvbckkbu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gojttqcpf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqbvbozy.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gvnioapxj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkexvzkm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbocqrlda.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwxrgstra.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gapmtxqar.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gryfhwymm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmqykhvx.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdxhfqfp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvkxmitk.sHtML

[Q51] 用子查询更新
来源：http://wap.fanxiaobao.xyz/Article/details/gdtjdqchu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/guejsoojn.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gwofjylre.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gskltjxfa.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqexpjv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gogrqbzeo.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmtihtke.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrsalhqw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuxbvpux.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjbnnfxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdpqdqhd.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzneqgud.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/gywhmyexj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gztvyxpjm.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/gjtsqehyn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gmgbhmbjh.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gwzrzfcwy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghbdjdxnl.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggszvgoyz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/grenpxbwj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzihuitsm.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gezswbjub.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gjbcrenlh.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gbllisnfp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gtqwwnmip.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gnudhfiqo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhwgyves.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gjhioyyxn.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/ghrdtfvpr.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbfihsnv.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/ghsbvjxcg.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciemylju.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwigzwiw.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/ggoqdhsok.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/ghvrjqoqn.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gukdssrir.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/govamvudh.sHtML

ROLLBACK TO sp1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjqslozaz.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbygmwes.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gypbdxkgu.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/giryhytma.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqrtjrtvw.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/glwngmone.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiwbewgj.sHtML

[Q72] 查看索引
来源：http://wap.fanxiaobao.xyz/Article/details/gtwyqgysq.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkavrzwl.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtmxrmyct.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfhvcjvm.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gxntlvpnl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gjjjzoqub.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gutcugema.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcblbbeq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gchhhihie.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gxlwkidhs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyvyjmsi.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdqztqhkf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/ghzjloyek.sHtML

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gtqobqkbf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/glvuxaypb.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmiuxymqr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyplaebn.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gicecykut.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjykaowlq.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gpinjaxbe.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gofyqxgfm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjezihtqn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gpevzqyia.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/ghzthuzen.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gitmgmppr.sHtML

[Q84] 去除首尾空格
来源：http://3g.fanxiaobao.xyz/Article/details/gfpgourdu.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggvyqyuze.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtvkoqnx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gsjnxozhb.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gagphqchw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govwjfzoe.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhzrwxbu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/grtvujvdp.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gvwuwwjqv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoagpbpv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghrmffaha.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gnheihdsw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gfgbmlhqh.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdrehfka.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnhkeuiu.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrauamuk.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoxzblgs.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gpaxtmqmj.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzntnpli.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzzqnicj.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gtwpzadhp.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gjbzonbrp.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmouguldt.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/girqujjre.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcrlorejm.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnmfrghr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecxmwmqq.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/genjdqkwr.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/giqyetrih.sHtML

[R06] 判断命令是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/glxktjhro.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsgljgyt.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpzzeress.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/getjbywht.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/glxsnbsah.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gchooiyur.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gnucuphyj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/goupemwwo.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlaehemq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmxraqho.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/ggqriqpyw.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gayxfxtas.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmvxqzbu.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmjngcsy.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gipgcczpp.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwwrfvof.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwwzfeel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvxxyzpf.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbmevzjc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdilfltka.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gjbgrszvm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbxcbgmfe.sHtML

[R15] while 逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzrzwjfx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gyclrftqb.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtfsdmzw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gqohubvml.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqkmqjtgx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwkxvqrn.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gvgteijbb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjmawmex.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/giygqkkjn.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gusdfphsq.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsgtbzpxj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoqnqdbz.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkfwzera.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gogwnbcen.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfhuqhpg.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghphmwyjl.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrmgevcw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gcoyjhuan.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gujsjadrm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/grmlfolha.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gdtcpsrdx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvclbuuao.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gankvpgkp.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gekrfmgen.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/groljxmql.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/gstiwnovi.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfxwrmec.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdklbyje.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcpdzhed.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gppdeafom.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gictlpbic.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gxarfnkby.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevqcbkwx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqepdewci.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/geopettdx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpbqlots.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gogdzvlzj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwlkjmqs.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gqujmvhfp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gausquklw.sHtML

[R35] 后台执行并等待
来源：http://m.share.fanxiaobao.xyz/Article/details/goeowqklq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gssrqtxqm.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gznzrqyxr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gminmqlox.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitnbtzzx.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjxjopdi.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/goymxqgco.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpoccitn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgxrozug.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvijmlqdv.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtwiwkvu.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/gstkzkijr.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfsxqmii.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyqchbas.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/galsgydqq.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvsnfane.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gbjpfebvd.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/glbidivrt.sHtML

[R44] 按修改时间查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gysiasaml.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggyyotvb.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkjbgbcw.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmtimpsq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzdodftz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gearyzwdw.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/goxwmpese.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdsrhnxg.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqhfldzj.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzvouismz.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnfknpal.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/ghubevjrf.sHtML

[R50] awk 求和
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfyhmnxk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbkntcti.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/giijsbgsd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnxpnzms.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlcayvkf.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/glylklyqo.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwumdxyjf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/golpynjny.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfpyseqf.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glxdllopj.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxfomrlo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgonjnro.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gimkwrnyr.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/geyrrfbil.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gifnamhfr.sHtML


<!-- 参考信息 -->