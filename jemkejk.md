代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltqldbki.sHtML

[Q07] 删除表
来源：http://blog.fanxiaobao.xyz/Article/details/gokxknqol.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcanudmth.sHtML

[Q08] 创建普通索引
来源：http://wap.fanxiaobao.xyz/Article/details/gxhypycao.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdejujmm.sHtML

[Q09] 创建唯一索引
来源：http://3g.fanxiaobao.xyz/Article/details/gvpbdoptl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfiysymoo.sHtML

[Q10] 插入单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghaaodhcs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gqklpvydm.sHtML

[Q11] 一次插入多行
来源：http://3g.fanxiaobao.xyz/Article/details/gmxshcdkx.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gyaadcooj.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gsnxtvzmm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzxknapsx.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fanxiaobao.xyz/Article/details/grtshvged.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnatzlbbb.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/gazxterfm.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzawpqjz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwhvlllq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.fanxiaobao.xyz/Article/details/gcjdquleo.sHtML

[Q15] 查询全部
来源：http://read.share.fanxiaobao.xyz/Article/details/gpifvohfj.sHtML

SELECT * FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/grbzgkoyv.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gauxfegxi.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glpguqfeh.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gldoyosxu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghueyajqc.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gumvrnyld.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fanxiaobao.xyz/Article/details/gltufdivh.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbgjuxeab.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkptgefab.sHtML

[Q20] IN 列表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjnimebo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvhsxxvyb.sHtML

[Q21] 空值判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gcthanmap.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fanxiaobao.xyz/Article/details/gljcnlyev.sHtML

[Q22] 排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbzykeucz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwwzxdfa.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaddmars.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.fanxiaobao.xyz/Article/details/gotqmqdgs.sHtML

[Q24] 去重
来源：http://blog.fanxiaobao.xyz/Article/details/gykuitpsl.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqincelyg.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfeifryz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fanxiaobao.xyz/Article/details/gabajbbzp.sHtML

[Q26] 计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxtaccib.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/glynqqvdb.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gsymaciun.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyxarjjd.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvqrtskad.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaawoqaze.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqqzaoms.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/glsegbwph.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklhdjotr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/glubtrgkv.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/giojggnet.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gyryyvekn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/goozkqfht.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gwtorghov.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fanxiaobao.xyz/Article/details/gyemdypea.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givpsyekl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/gphdanjai.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gimepftnm.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwlfuyse.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gmwbkktjg.sHtML

) t WHERE rn = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gshjlhdsi.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/giptzqnrd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/geiktylyd.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gszmeavzm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiifeoil.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfmbomvp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbmtlreg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fanxiaobao.xyz/Article/details/gndomdash.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/galgfvgud.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gppbimvpx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gubmscmkn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gstzgugxe.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gaboiyqpo.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gnwbdgpdx.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzrvyjkh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaedflqe.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/grqidrehp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbfhfsap.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/ginxmalrq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gefhmozqa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gnvhsijxn.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/ggocagkdn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fanxiaobao.xyz/Article/details/gyfsdjpdj.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gtjhkinmk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gujonppec.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbjlhdzv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gblxhjerl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gdqifuzhr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gndjnakxq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqudwgpxt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gbkcwkkrg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdarbjwc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gdafacwbh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gnpjnturu.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfcvomukf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpmwpmis.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnumyywc.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/grjtdlngr.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gqnonvcqu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvbqqlyw.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gtbtuceny.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gshzvgwrx.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwswwzezr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gavwiuyvi.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gipwhmwrc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/ghykjukln.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/goxdrblux.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gevnbjmrs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gciwnjbah.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/guhjjggnh.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/guxplhann.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gudrpgsiz.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/glnxomahh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjpmqpou.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gejojdqbd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ggvpzonnm.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gwynxhleo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gqmxzgbao.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gujeklxsa.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gvtbltxnu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrxfafek.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/glrtgonzn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzsgparw.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/guubwlpsb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkdkdnvs.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/glijdtmjs.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gioggsxvl.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gneyailnl.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gjirqdqoz.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gceolyekr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gknlpqjrg.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/givnvrgek.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzbmwfag.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikfypszh.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfmydlzw.sHtML

ROLLBACK TO sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gevwigomw.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gxlbsrozi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gmdnjyneu.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gyfwidgwz.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdlqzpdc.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpgpjafs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gjazorrzk.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquoglwaa.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsmhdyqk.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gontdbhml.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxaopmae.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozeonlka.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvmgwdtp.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkcewemg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gislbhqpl.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvggdsqn.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmveosos.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gsiriazzu.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gxdjbbrjc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.fanxiaobao.xyz/Article/details/gbglivyrz.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gwqkcvxeg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/giomewbns.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhhhwwqq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gulcexpcr.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/givncgjjx.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdzxajhz.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmvgbkjkh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gupeudgik.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyywnjhi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaxsqmcu.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gihzsyvau.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatsgvsvy.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffetrmei.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvldtgbd.sHtML

[Q85] 数值取整
来源：http://3g.fanxiaobao.xyz/Article/details/gpcafwynr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gbiqrqbte.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gudmiildx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gyikdabeh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gazbbdsqp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkcqesxfh.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gatxpowov.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/gidzpsgjz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gblmfujnt.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gqadghium.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gfgjfaime.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gkqmkrwlo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpuagzpq.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwcqhwwl.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/grupfonrv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guhgjrsgc.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/ggfahqilf.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwnwskww.sHtML

set -euo pipefail
来源：http://3g.fanxiaobao.xyz/Article/details/gwixvmyae.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnpahsypi.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gywvuowld.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gicsvxnxv.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gglgkhijw.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/ggmegoysg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gcsydkvpq.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gylsgxgvk.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/guoqkbzed.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjojqdjqr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gdyywnfdj.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnrhtuvy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gqucucbih.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gijzzrmrm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmcjtapct.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkcaluhzo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gvsnlswgl.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjwsldez.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcosxcvlv.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebvbwvrr.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gdxgvcytk.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwgobele.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/grtevymww.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcecnsrmi.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqlizpqd.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gnzuuvslq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/geqvhudkc.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gsdmkhvjm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/guyettbut.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrhoizhf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/giathypry.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/glhzhnjwn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczaateii.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwuvmzzo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gkhnyeemi.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gblaxlekz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gusyjhcgu.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtgtsdok.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxohijufr.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjrxuwpf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmqfifvh.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/goykwlydo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gypprtxzd.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcifximde.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtsqmtca.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gtfdpftwz.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/glwqawhrx.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gpvxgiuxi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gssymzaeb.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxyqdetd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/guwnmpjtq.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxtohukm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgjwrvyq.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwvkksler.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqsmftco.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtysutjwz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fanxiaobao.xyz/Article/details/ghlksyysa.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gzyvpqghn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gdflvnhwn.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfqawtdr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzonzvsvs.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxvkgfgq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fanxiaobao.xyz/Article/details/gogdtybfn.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsiehekot.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gskpxgkae.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gjmqykqgp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggrrdjsic.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gyjztchjl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gpxlnqsbz.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gcdzjhjqn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gittxfqws.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gkznmzdlj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/ganqhfnsw.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gfasxaqoh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gnunfiufc.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gagqqnyro.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gxkmzfjxt.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gysdprfvc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhocztei.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmcyqmig.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdrhdztct.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcwmtnlm.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gaprkzlkf.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gvygyosvw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgbnokgo.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/ghzlkknvp.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddeysqxc.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gagphpiud.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gcxholtmm.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwiyaycu.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkfzyaje.sHtML

[R45] 批量删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gneyalgpq.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gfcvvalne.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/giwkgzpqb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnimnnxy.sHtML

[R47] sed 单行替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkczrnizz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfbucjhm.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gvfiycdjg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvwfumeb.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbwzlngsu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gtrpzazqr.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/ggpkwpuvd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gichghcwi.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrsdliuk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gnbcepcrz.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgkgcqbo.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gobcbtcin.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzuokrfu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gguhwlhoa.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxxjshzls.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gyesbpbeu.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgfbcmxi.sHtML


<!-- 参考信息 -->