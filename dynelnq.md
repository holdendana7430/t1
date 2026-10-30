代发 wailian999

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fanxiaobao.xyz/Article/details/gjqzvuhnm.sHtML

[Q07] 删除表
来源：http://www.share.fanxiaobao.xyz/Article/details/gompyzlbw.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfevoatz.sHtML

[Q08] 创建普通索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvubwywu.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gnjkynfwj.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gzmymdjxg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdyoketn.sHtML

[Q10] 插入单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntwrorrk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxwcoqbf.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhzikhqe.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gvcrbvcuv.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fanxiaobao.xyz/Article/details/gowysxnpd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fanxiaobao.xyz/Article/details/gxqceiarh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fanxiaobao.xyz/Article/details/guqemhplr.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucocjosw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fanxiaobao.xyz/Article/details/gvmlyopwy.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.fanxiaobao.xyz/Article/details/gpybqzopt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fanxiaobao.xyz/Article/details/gconhombu.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmrwpguc.sHtML

[Q15] 查询全部
来源：http://wap.fanxiaobao.xyz/Article/details/gmqjcbbuy.sHtML

SELECT * FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgjltylj.sHtML

[Q16] 查询指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gehwspruj.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjfgdcyh.sHtML

[Q17] 条件查询
来源：http://m.share.fanxiaobao.xyz/Article/details/ggauiozmu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gybikhysr.sHtML

[Q18] 模糊匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gwmhqbzwn.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fanxiaobao.xyz/Article/details/gqxjcqpar.sHtML

[Q19] 范围查询
来源：http://wap.fanxiaobao.xyz/Article/details/gvajnogrk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvetrqhj.sHtML

[Q20] IN 列表
来源：http://wap.fanxiaobao.xyz/Article/details/gzrahqyoz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gtxnipdfs.sHtML

[Q21] 空值判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnygjxtgo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspwcrura.sHtML

[Q22] 排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gasaqvhut.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvrnugwn.sHtML

[Q23] 分页
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzczcnqi.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fanxiaobao.xyz/Article/details/gilvfciba.sHtML

[Q24] 去重
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkdmznvs.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gryxuqkox.sHtML

[Q25] 只取前 N 条
来源：http://wap.fanxiaobao.xyz/Article/details/ggeewffgs.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fanxiaobao.xyz/Article/details/grdopwvdr.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gbibkzioa.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/govesmkvz.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcysztdtg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ghhcoambs.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsasdbus.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/glmjhvxji.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gsuxijego.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrurhmwm.sHtML

[Q30] 分组统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gettawmxa.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyenfvdc.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gsnhyhrcy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghuqnsqbd.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/geezuwwqd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gknkasygw.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsyggnhj.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/grkerctly.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmldfuln.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzuzawbee.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpegbdhb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjqiibkum.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/ggiirzmjq.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/grhbdtgmr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggylsvwqk.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/giqplrprg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fanxiaobao.xyz/Article/details/ghomhhjru.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/ggzkybbwe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/guxmnepxc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gqkjirrow.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gulwmkhkx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgpjxtgc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutduugfb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlmcoopa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvdqanfk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzlsdwefe.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gjsztopam.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gobtezevh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsnkpglx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpieteime.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxiqvwwf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galiqyref.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gogkgesya.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gthlbqbgx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdlwmxvd.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwcpyrih.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gaztqxkes.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gbithiuzl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvgpmymo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gkqxmpmwg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/gadhkxjms.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gmrkhoydv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gztsonbpz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbbfybba.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjvqzuei.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gluflpwlu.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gbafnusbh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/ggkyuilhl.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gazwvdkqh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gcchpcaro.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/ggdonjeze.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbnwlkhu.sHtML

[Q52] 删除指定行
来源：http://mobile.fanxiaobao.xyz/Article/details/gnevshwow.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkjsefkp.sHtML

[Q53] 按条件删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqymikaw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnvcxbds.sHtML

[Q54] 清空表
来源：http://3g.fanxiaobao.xyz/Article/details/gairjbitq.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/guqqpjuvp.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/guthziwwk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbocooiek.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/grjstvepw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gwdpdpspz.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/ggerlpnwk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmkpyihac.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpvsbbqq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gizlrwurm.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqvbzyge.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gtcopivvi.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjrzxvme.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/glewqhbdy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnojpolw.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksbwdogo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gpeledckx.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gkwmgukdy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxekzdcn.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmvptocik.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghblwfuer.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/grvzcdpic.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwgqkwoc.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gselphllj.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gjpsijhqt.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gepysmdzz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gafouetzr.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gdpugihml.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gznsbfveb.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gttqkklti.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gattbtzis.sHtML

ROLLBACK TO sp1;
来源：http://wap.fanxiaobao.xyz/Article/details/gzrexnwan.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/geglxtrnl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjlehdrds.sHtML

[Q70] 更新统计信息
来源：http://read.share.fanxiaobao.xyz/Article/details/glluxaely.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimryeffw.sHtML

[Q71] 查看建表语句
来源：http://mobile.fanxiaobao.xyz/Article/details/glafxvqsj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gclqtumkg.sHtML

[Q72] 查看索引
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntktsehy.sHtML

SHOW INDEX FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gjkcswoyl.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyrqjigy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gdaondsuf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajcvrlan.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhoxzsjt.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gpeskcbcj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/greiiybde.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsokfmfai.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gmfkgfnak.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gtghvnkkf.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gwslelovg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gslxvvgki.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugcjdlef.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gqqqaiiuq.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/ghxuewwfd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gcugddiut.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxrxqiyi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapgxekkr.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghizbtbim.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpoxnfvpt.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gucaetfjb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtsnlwgx.sHtML

[Q83] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gnulxnakl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxbugvmw.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjfswkft.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnllucng.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gricfvrql.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkzrlrwv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gpszlzmec.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhgtkbpp.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/garxsdpro.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosopplaz.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/girzrogad.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakaqgbbv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gpvqhagfc.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuuwjwyy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gyqjjwvbj.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/geauyxddu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fanxiaobao.xyz/Article/details/gutjekagd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhegwbdm.sHtML

R. Bash 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmvuiszn.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjadncxzm.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gyvnendqo.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgazhmhx.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/grofnolzy.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gguvnztja.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqxiseoj.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/guhlvdugp.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqbumwte.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gzlicgido.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmxpfotr.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gpwzmypfs.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/gupdlbuxs.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlkjyjjq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtdpsirw.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzuaxwpq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gilkygvap.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gkvbeawol.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghkupcddf.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gfsgsjspt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gpedgxtsj.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfxsjutw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gewludnen.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhuxigzh.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowdnyipp.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gyqljplgq.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxrgsgns.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwlvjuphr.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvdmaapua.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnifcjhje.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gmdkqtbaq.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmdhiyrj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauonmzxw.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/guoxdwvsx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grkwvshed.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjqpovvs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhayrkic.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/guiehvwbe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghugbjwbp.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvckkqgn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpdkhwbu.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfnlpwyu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdfamxwz.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbuysxrr.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkyzkfiud.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gymbjheni.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gulanmhrs.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumwirkbe.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gxizcsbue.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gpmovkioy.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gytxgsefq.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefryjhso.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghyzewkew.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsubltce.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnptxuoc.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fanxiaobao.xyz/Article/details/gigmvhocr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gaussbiiw.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqjtqmmh.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gclqyaukx.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gxuilfhpg.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/glhfdnilt.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gdklfrocq.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigqahtav.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gpagbtoxm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gggkggrov.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmboelum.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtbipblg.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gobzhsuwu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyyqiuegw.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gdskpkggh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwosfpxuq.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/guamkseva.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gklftkbob.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmkotsxy.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtwsabqk.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/ghszhvwko.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gychffxhe.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/glparmjel.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcwoybsr.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmevjsoxa.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdwrtqqf.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/ggcdubgjm.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfxorrhj.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gbohjyuvv.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbejqtja.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfwusxrj.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjycsmwj.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gcyqjjxqh.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gmtmveaku.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gbomrztpx.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxfvndal.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gknhklhdb.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwfehdcn.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gfhntytjl.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gkxepsdsw.sHtML

[R45] 批量删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeafgwee.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/grfwznpbs.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxotohyyu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhkcbwed.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gceylljfl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgznqqtv.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gghfjlxon.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gubstoavm.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmojmzxxh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gfzdgnfgr.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gsqiytfcs.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gfytrgiyd.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/guzuaexhs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gfamtaqol.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsttajcey.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjvknqee.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gphhqmpsd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfyqvjrp.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxiisyhkw.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glntzefue.sHtML

[R55] 压缩与解压
来源：http://baike.fanxiaobao.xyz/Article/details/glyhakqqr.sHtML


<!-- 参考信息 -->