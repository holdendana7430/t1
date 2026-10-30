代发 wailian999

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fanxiaobao.xyz/Article/details/genceowga.sHtML

[Q05] 重命名列
来源：http://m.share.fanxiaobao.xyz/Article/details/gylkanydl.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxekdebz.sHtML

[Q06] 删除列
来源：http://mobile.fanxiaobao.xyz/Article/details/gxqwgayvy.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnsiwnml.sHtML

[Q07] 删除表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpcpzjhh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmamcwnl.sHtML

[Q08] 创建普通索引
来源：http://baike.fanxiaobao.xyz/Article/details/gvoxpjudz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhqycwwy.sHtML

[Q09] 创建唯一索引
来源：http://wap.fanxiaobao.xyz/Article/details/gyvjlduya.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fanxiaobao.xyz/Article/details/gmgcsefpx.sHtML

[Q10] 插入单行
来源：http://3g.fanxiaobao.xyz/Article/details/gbfwavsml.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gwceorwvn.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdaootib.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fanxiaobao.xyz/Article/details/grltpqlfu.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/gzsyhtijb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fanxiaobao.xyz/Article/details/ghmmmxrfe.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fanxiaobao.xyz/Article/details/gviopntac.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gmcrotijp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkfetsjn.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gokmxjetd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fanxiaobao.xyz/Article/details/gcqbhvwfc.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fanxiaobao.xyz/Article/details/gsolcyuvz.sHtML

[Q15] 查询全部
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkbxslle.sHtML

SELECT * FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gdfjmeigz.sHtML

[Q16] 查询指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/glzlcqkbv.sHtML

SELECT id, name FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcfsumiku.sHtML

[Q17] 条件查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gwncldoln.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwveqjwgc.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkoqdpyzl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fanxiaobao.xyz/Article/details/gqrrenmrp.sHtML

[Q19] 范围查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsogfhflz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghadvmmjl.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmalhanw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbagkwcdm.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gogmpwkpp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fanxiaobao.xyz/Article/details/gatszziml.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxrtuobs.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fanxiaobao.xyz/Article/details/gmpxpwuji.sHtML

[Q23] 分页
来源：http://blog.fanxiaobao.xyz/Article/details/goctymktt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fanxiaobao.xyz/Article/details/gngxtgdke.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/glmpdvqtw.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gexzmpeny.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwajvryzb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fanxiaobao.xyz/Article/details/ggiyoukxl.sHtML

[Q26] 计数
来源：http://baike.fanxiaobao.xyz/Article/details/gnykitwal.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmaoywtp.sHtML

[Q27] 条件计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gucacvqbv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggbiksiof.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhtpeeev.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gnppbljoa.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gwqxkrtdd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbpjkqyqk.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxptmocdc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzcplmdc.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gryxwqemk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpaasytoo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/godtoqadb.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcathxvxu.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gblqclacp.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gnlwnydar.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gnjblypoq.sHtML

[Q34] 每组取第一条
来源：http://wap.fanxiaobao.xyz/Article/details/grgoakozx.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gywlpbnhe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gwtxuxgak.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gytytmrez.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gbemrdmoz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gqxsykegk.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gewjkkgyr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/glldfgyba.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/glqiihkai.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvbpmksrx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/glhkaldkg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gkmsgbwga.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gabwejedt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fanxiaobao.xyz/Article/details/gxisarspv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/guhcofyou.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmkpzbgn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fanxiaobao.xyz/Article/details/ggjebqxfs.sHtML

[Q41] 多表连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggfzqesha.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fanxiaobao.xyz/Article/details/gorywvesa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gztuxkxri.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gajwlypxy.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttheiumr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/giiyobuxw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gkmyxgqrw.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gmhxdrnmt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjwupfnbu.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/geeydvpft.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnefzfxn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgdsoonc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/ghrlgtukb.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gqlvcevxk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyplckhvl.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gmzydmbyn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gwwngnsor.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fanxiaobao.xyz/Article/details/giqjsyhti.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gfqdwexni.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gaadwlvwx.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/ghrzkzjqf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gvhjkkfmm.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gwycwnbxu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gcnfdskxs.sHtML

[Q51] 用子查询更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gwilyhqdu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxawvqbji.sHtML

[Q52] 删除指定行
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxbpuexd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxgzcllj.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gwgzuftcm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gngtuscdx.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/glvaneyhm.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gvtfsfzyt.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjxgjvgzk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggopvnvlf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfclpamhq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsudyugtd.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/grppvrszw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/getdaqxwc.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gwazsqjqg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gatttpevb.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gwypxqulq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/glqicslct.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gqgxjzpgp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gambtbdqb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsueurguu.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcgqpozb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ggidtlyko.sHtML

[Q62] 分组占比
来源：http://www.share.fanxiaobao.xyz/Article/details/gqninwthk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/glatybngi.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/geunywjip.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gfhugotjc.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkpbtphv.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gzdecfbzu.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/glvjtwxmw.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gegjkoxih.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/ghdpwywff.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuxshcjk.sHtML

[Q67] 设置隔离级别
来源：http://wap.fanxiaobao.xyz/Article/details/gqjwsauqj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gcamxgtwj.sHtML

[Q68] 保存点
来源：http://3g.fanxiaobao.xyz/Article/details/gidcvoskk.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpdqjdhi.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcycrycm.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gywqnlwbd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/glsonnwtu.sHtML

[Q70] 更新统计信息
来源：http://3g.fanxiaobao.xyz/Article/details/gkspjhtqh.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gouewwslw.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gucmycxrj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghyimjlm.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwuzmugk.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswzwkkjg.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/glevtxtjk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/griiubzgf.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gdfyldwph.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkuuonuc.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbubphmx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gybvbrurk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gtibpxzbo.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrgqnsog.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbytjutrg.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagcfcliy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gayzxdvxb.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gwhbysmer.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fanxiaobao.xyz/Article/details/gobjvhzoc.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtotlofen.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxesqiuuq.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gpsjpgmsv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gcwhcbvtf.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/grwbwxwgq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/goaswdbrh.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gndhooojh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpydoxjgb.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gmdcronxy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsbdeqfw.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchicjgff.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwewnljd.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gtqrqjpgk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gduwilgdm.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fanxiaobao.xyz/Article/details/ghemlbxmv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gufcccwbv.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghpxcclyp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/gfmpedgoa.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsdjsmje.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fanxiaobao.xyz/Article/details/grjyjpfge.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghawtxdx.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gplfxspxi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gooknesjm.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gtzpavcjo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gcohqumem.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgrgytgo.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gllrwchkt.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrfkbkge.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gtgkrbgzz.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gbmuuvivf.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gmonhugqp.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/ghfihoozw.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gyxjphups.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gkexppwqz.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxwevnxq.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhgnxzhf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gmkuzwbiy.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggstvafil.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqtlgggx.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gdkkjukvh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gawfwkstj.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzuypegk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gruakqyjw.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdjmqjzo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmtfqpth.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvgnfxzdt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfkasoff.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gchbiigfn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhcytexb.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqzudqfd.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbljitdi.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghydonqjy.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gbfrdxlpa.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpagluws.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/galuubovj.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gjyansezo.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzouixqk.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gltiewpfy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpwnngfiv.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcojdizrv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdczziwax.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfljvzqyy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvgpzohec.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkblrlpqa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqkbmyxho.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gdsrmrqoh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmierdus.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gxusiosmm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpwuhzcqt.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/ghqylxtjc.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gituiplsm.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnygltakw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/grladxmuz.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggurtvomk.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gepjclvun.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gknqbcsrp.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwskofycr.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gwjuztwow.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gamhucrhd.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/galeqaltc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwyalsewx.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/goujxgjjw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuxonphs.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gyittjwyx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/giltrhjrc.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/grvjgcxrh.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcibuubef.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gvewnejwt.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gnhloixlv.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvdlkyjr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/grfevssub.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ghirddoch.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmkpwzhz.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gziixpgyy.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gladqgvsh.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaopxcspj.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjrpkyksy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/giesjzneu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdagampq.sHtML

[R34] 退出时清理
来源：http://blog.fanxiaobao.xyz/Article/details/gcabnshjn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gsivfuzej.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvexdkdcl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjojenfc.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gepxjxtpu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gvwpvmmjd.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gwpeujzsb.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/guawfrvim.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/grokkhwsj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobnzdkzx.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gbykrmzqx.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjzjbvmw.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gbtawmkwu.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gzipleofb.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gimgtsute.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxayavjq.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcwfdijz.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzinntyj.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxqbujan.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gukjgbsep.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/ghqwydacp.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gnigfrpzv.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkeoigxy.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpivmbcs.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzroepcoq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gncqxdvpz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwktlbyot.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgzcczmc.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/grxkrunts.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/galbtnues.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gsacvesgp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gksquidyq.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlkpikyl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrqwytsl.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhlfrepz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/goaqhybvb.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gtpiiebub.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggyuhkfxk.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gyepjibjq.sHtML


<!-- 参考信息 -->