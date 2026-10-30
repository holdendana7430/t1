代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/glhqrizyw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fanxiaobao.xyz/Article/details/gtghikpuo.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gteecyije.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gqdcoglmc.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fanxiaobao.xyz/Article/details/gljqvrgno.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.fanxiaobao.xyz/Article/details/gxoknpzvh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkapobwpg.sHtML

[Q15] 查询全部
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmmwlmfv.sHtML

SELECT * FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwynjiafs.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhcxereg.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvyhdlzk.sHtML

[Q17] 条件查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjprddog.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqtvpvdcq.sHtML

[Q18] 模糊匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gbjvwzbdf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/griyyifrq.sHtML

[Q19] 范围查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgdhtczw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdlsevcj.sHtML

[Q20] IN 列表
来源：http://3g.fanxiaobao.xyz/Article/details/gxyycwwil.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypuqoulb.sHtML

[Q21] 空值判断
来源：http://3g.fanxiaobao.xyz/Article/details/gcvfoaqrc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fanxiaobao.xyz/Article/details/gvcsyxgxm.sHtML

[Q22] 排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdosbfuv.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.fanxiaobao.xyz/Article/details/gieipkioo.sHtML

[Q23] 分页
来源：http://mobile.fanxiaobao.xyz/Article/details/gapnihdts.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fanxiaobao.xyz/Article/details/gcgguusul.sHtML

[Q24] 去重
来源：http://3g.fanxiaobao.xyz/Article/details/gkztjiaoa.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscagygcr.sHtML

[Q25] 只取前 N 条
来源：http://baike.fanxiaobao.xyz/Article/details/gcjvyomrt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwrpuemob.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxvcighc.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gzcdalihi.sHtML

[Q27] 条件计数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnzbjgsx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/grrnqikxk.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gtkwgifxh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gknmdjfjd.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfwadquu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/glagfxfwb.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdtvybqe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfwafhnua.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmaxehmy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhqtoorn.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxydtuvfg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/galeetlez.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gswzmtmtx.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gugbatmee.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxsezjtq.sHtML

[Q34] 每组取第一条
来源：http://3g.fanxiaobao.xyz/Article/details/gflakpnsw.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfnkjesa.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gxxugpypg.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gcnmionml.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpcvqtbb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeicrzub.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/gdfrbyjpx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzihadpa.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gjhxktmkm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gynhfcoio.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/giakyaxpq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gxdjjqyys.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkzurxuj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/grqlevtyl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcajzhtpa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fanxiaobao.xyz/Article/details/glmqbgwcy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhekxuuw.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gnquvrxtj.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvqmvpqp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fanxiaobao.xyz/Article/details/gxosrujur.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggspcgngp.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gemnvxhbt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkiiithv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gnvuepedm.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gsvgmfugc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guselkcsb.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsadgtbqx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgkchyvh.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fanxiaobao.xyz/Article/details/gauzwxbuk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllvfnouh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fanxiaobao.xyz/Article/details/gvkpungut.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdamcjya.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqobehzq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/giixokfon.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/ghzwcdado.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/gjwrpuwrg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gvbptrshz.sHtML

[Q49] 更新单行
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsqrsdcc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckgbzczf.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrubturi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gbeoqeyem.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/gadslrvbw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnnpxfghn.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/ghkuzfdyo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gosgqqxbg.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gnictdcmh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/genrugshq.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gcblhwnxh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuznwwoj.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gsemcqjht.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwquyiyl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gmemoskce.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/ghzjaucvn.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/gipmvmynh.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/govfiyatf.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxozgwut.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjstrtxb.sHtML

[Q59] 分组内累计
来源：http://m.share.fanxiaobao.xyz/Article/details/gkitptbwq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gmnfgrshv.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gsqergvop.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdctprxt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjixpztkj.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxrtdsxw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gerdsereu.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkdwfpzu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtwteeaiz.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvztbsyi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gkirufvom.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gauhrysuh.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gsizerqkt.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevxfgnpu.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvylajzdy.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrruzjtg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpdwpcbe.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gjoshcwnw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtjjzueh.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbwhjqqz.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzehcknmb.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqkcnmqdr.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/grfjyxnev.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjdpzyiu.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gquoxohqk.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqygcezad.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpjxaahi.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gtyvxoywc.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxvfyvpt.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gfcplqazi.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/gtmmjlvaf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/ggbzgmdkz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfftaaod.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqutonlbv.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxadadqxq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfceykjkc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gwocrkvjq.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gxrvtmzbw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqsstxub.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gzxwrbaxe.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gscqwzwya.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffehnciw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gmauwnwwa.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/glrrlcomt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gtskdrenc.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gldsdngsa.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gvxlhcguj.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqrjogta.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmwcsdvto.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaykisld.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsngsetf.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gmseunhlf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gktfweqyt.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsazsisz.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbcztjss.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvjyevmz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/goioygcic.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gonmhkwie.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gelbhbvfs.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzxmupkgj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gprlroudq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/ggreaabja.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gzralfgbg.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/grgubnipa.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzrpqgdg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknrmccxj.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gftsjxtww.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/ghqkwqvdu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gizirejqi.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqwpyekb.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/griehtpip.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gwhtoomfe.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoisscrn.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/gpvvrqcnh.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fanxiaobao.xyz/Article/details/gddrktftd.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gneohggto.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkjaheiby.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gumufnjtz.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuwplzlp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gascirfkn.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/goesfegjn.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcpwzdpaq.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/geppardax.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqleenmfn.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzvyctlz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gsshmnqqq.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemnjrylb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdyhjnqh.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxbgogls.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gseywsklk.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjzahnzo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gllihcsqs.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpfifopy.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gosmsfuxm.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gupwgchql.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjmwrkgwc.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqxpohnr.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gkakfvuff.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gikvonugd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwaqyxug.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gesquxtgd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsnbshrx.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gaiodcuzq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghavadtei.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcyxlerq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/guqutrxkf.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gpuuduqxa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbzumvqh.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxzambtp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gfegcbjhi.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gskjlszpr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gfcniupad.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqyoyycfj.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gueuxhzbu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfaunppr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gfnolmccc.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gcenkyzjh.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gugoodtxs.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxbrgipk.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gmufopxow.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbubzrat.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggukltjfo.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdmweish.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/goafwovpr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsocvzgvb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/guptoelbm.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gmsspvlyu.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gthcthued.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gbcrgbaok.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcelurdl.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/grgkvburu.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdbfgijl.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gwuypidbf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoesezsq.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gxaaxquls.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gtqonazcf.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gojihkxfa.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/geuryxxmr.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gfzupfbtz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbduwmxhy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjryjrtir.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gdxmlpesv.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmrvsqomw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gzqtzpekd.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gjgzpnuns.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gspvwygcf.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdmrestj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeqvrhro.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjawpyphy.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gpapjflcr.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gfnyikvjg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkxbitft.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisqadpts.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxmhgvyy.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsbabqby.sHtML

echo "log" >> out.log
来源：http://baike.fanxiaobao.xyz/Article/details/gorargddd.sHtML

[R41] 丢弃输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbslqgcl.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbdazvlv.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlejmwsg.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhyrwihs.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gijbtvmnp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemojemip.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtfxmhqb.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gejijezwf.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gaiozkgsr.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgzeecdj.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhnmtuol.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gmvfjdgds.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgfzadoo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutnbngzs.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsvtqxsl.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkiamdyoq.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gyfakijuu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gzwknwfse.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gtelznzth.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvlacqab.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gofvqehwu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gzvbhkcpk.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/giljgnldi.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/govuiwgxz.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpetnkux.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gthfweuua.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrztmzpj.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gpsgrexbf.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/grvgvjwqh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gkceayzfg.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gsltjrdby.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gtolbnndx.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gzgzcfpds.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gvnndqnem.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrghjvrf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gtywxkshl.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/grupiceau.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gilmdcbuj.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gceehoydz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/grcujuhfx.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/grqojgthc.sHtML


<!-- 参考信息 -->