代发 wailian999

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gwursndcb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gywtantep.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gqmszetdn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gfmhmqkzj.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/grejcleat.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gyggiujos.sHtML

[Q02] 创建带外键的表
来源：http://baike.hesvh.cn/Article/details/gwaomcumw.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/geurqnkun.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gaaiisncw.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gqzjbnwyj.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gipijqdlk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.fehbvm.com/Article/details/gzkeigqqq.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gsnpwznai.sHtML

[Q03] 增加列
来源：http://mobile.hesvh.cn/Article/details/gvymydswg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/geqqgkbie.sHtML

[Q04] 修改列类型
来源：http://3g.fehbvm.com/Article/details/gpwilzmkv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gimdkykkd.sHtML

[Q05] 重命名列
来源：http://3g.fehbvm.com/Article/details/gsobajzjg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gmkxfhrtm.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gxvndxusr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/ggnbqdrbr.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/glayywpmd.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/geooagxea.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gfljpwait.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gmqknxdhg.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gzvjrxcyz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/ghmkbjlsy.sHtML

[Q10] 插入单行
来源：http://m.share.zdbjq.cn/Article/details/geohhifgu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fehbvm.com/Article/details/glbfceilx.sHtML

[Q11] 一次插入多行
来源：http://blog.hesvh.cn/Article/details/gmzyeeegc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gywyqwjrr.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.zdbjq.cn/Article/details/gnbofyshs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.zdbjq.cn/Article/details/gqldvrusa.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gzgroncsm.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gbfltpxwu.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gqurqdtrh.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gdetdkooo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.share.hesvh.cn/Article/details/gcpecixbp.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.hesvh.cn/Article/details/gaswkrsng.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gavecullg.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/giixeysid.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gpzdvlmzk.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gskxgjkpf.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gpqyszxxa.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/gyezgpqlx.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gxmczwevf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gnacfwxgp.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/ggeznugxj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gdistsgfj.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gzodlmzjz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/gaotdxzzp.sHtML

[Q21] 空值判断
来源：http://www.m.share.hesvh.cn/Article/details/gmyrfjdpw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/ganogtris.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gweazqyxn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gsmbftzhg.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gjsicnnpu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/guxwosujh.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gmpieebmx.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmxsbsyhp.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gdxpwxhjh.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/grzwpjdml.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gjcmwulam.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzbrmdamo.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gktacqzmc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gicabdnsl.sHtML

[Q28] 求和与平均
来源：http://www.share.fehbvm.com/Article/details/gsumjngbj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/glieysstr.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/ggfucqpua.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.hesvh.cn/Article/details/gppfwozha.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gaytwfgbd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gldsrzjii.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gwccjzfep.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/ggetngegy.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gbkwavrjd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gcolezclp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/geeranqbl.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gzkejcpyq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gascocoll.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gqwyktvqz.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/ghxmwnzmc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/guppiwpdj.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gwikmyipw.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/gqeuovmht.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gpeiacjsg.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gcgqzqygw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gxcfcrodc.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gygrkeeht.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gfwtitjyn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gpmwkfgsv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fehbvm.com/Article/details/ghjkkycoi.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gagzgsifx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gooijnjjj.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gzznxiaet.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gtxixmrmh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gdglyidlj.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gheyuzwvb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/gmmhgxuak.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gewwmiveb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gcbddxfet.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gfjbqetxd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gvabzdowf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gbdksoqyj.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/giooqtsye.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gixrixqcu.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gqssvapga.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gduqwbcfd.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gvhzjxvyz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gfidhzmcy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.zdbjq.cn/Article/details/giafucvmm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gmogxvnqd.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/geogmilzr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/getxidxpz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gstggmdao.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/ghuteaoxn.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/guploaiwj.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/gqgvxzcge.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gllpthcie.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gsfpielvz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/ghggeogwn.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gnpyhspqp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/glxwzkmcb.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gmyppmhrh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gbkfhcjwt.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gcqntbfca.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gjhykdqua.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/grmxxtire.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gmbfxdsan.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gszpmpfoc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gkwblycer.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gucgehgii.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gyztletca.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/gjkltawfl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gbootvltc.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/goeieaald.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghcalpvwa.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gfkmlfawy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gnkdrqqnd.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/ggpwtztdo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/ginfmkqvz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gwwgivlrr.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/ggjocquwd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gntsnhezn.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gxjpdnwtv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gyhzmxwee.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gcbuiblvv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gokzdoguw.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gmnkjrwlx.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/glrrjnkoe.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gqzvxlkuf.sHtML

ROLLBACK;
来源：http://mobile.hesvh.cn/Article/details/gdydbbjtu.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/ggrhebuxt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gngcxcndt.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gyijlxajq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gujaybxgg.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gpdxlrwqj.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gvdtdjflo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/ghrgqhstp.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gxsqzqqhp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gjqhxxwon.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ghmkuljin.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gzhqubvwf.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gfqjbjpjd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/gjazsjqxb.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gqkcgemtl.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gzuvjqtcq.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/glwjektnv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gungimeur.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gkcpndbri.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gzkjqqvpb.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gjpykcahz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/grvgdfusy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gpbuhtzes.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gnjfbbcck.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/ggrgrhuyr.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gngcyxiao.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/guwcpuirv.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gzkwgdrvx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gbkytokcf.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/gqrizpcdo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gvrjssgmz.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gdnkuwdus.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkwaglxok.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gptxudfty.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gaphsbagl.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gpugatfuy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gejddvztj.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gjgobzwqy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gafijxmlz.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/goxcqunsk.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/glvngmgmy.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gfxlffnur.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gtjsnwvst.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/geywcrczc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gvwtklast.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/glcjrpbzf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/ggagmlzog.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gmsjbflmy.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/ghiewasdc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gthuwpfrx.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/glvkmvfbg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/glkffutym.sHtML

[Q90] 生成序号列
来源：http://wap.hesvh.cn/Article/details/gkfpcwbqc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.hesvh.cn/Article/details/gavkpoglo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gmuieodbl.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gciowesdg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/glkeirobi.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gdjglggqy.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gdqifqemw.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gzzpsugxg.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gjtdinpkp.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gowextwdi.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gthxjzzvg.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gydowqfvw.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gbitagaji.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gyjsgyhhl.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gcrwchfdv.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gjyakymmu.sHtML

[R06] 判断命令是否存在
来源：http://read.share.zdbjq.cn/Article/details/gxcflbkju.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gtgoprclk.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/ggxkkeutl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gprksgtns.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/guklabflv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gociqnvdt.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gfbawrkun.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gzfltevxa.sHtML

[R10] 正则匹配
来源：http://blog.fehbvm.com/Article/details/ggpvmrvcn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gfuwcrwqr.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gpoopsrag.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gvnjvidnb.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/ggfuohaby.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/giueqzcbo.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/gmoubgmlj.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/goqyqvfod.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/gcbmslmux.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gnuqldugb.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gktzhpqbw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gqvjlmkhc.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/gdmehjgyj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gptosioak.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gsobmfynz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gconopqhm.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gzrasrqjt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/giloxxile.sHtML

[R17] 数组定义与取值
来源：http://www.blog.hesvh.cn/Article/details/gecieepdg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gseeamnjp.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gdolvuspu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gxnhpfixt.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gsviszdso.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gjficmldk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gytihzkyo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gfrtrfxyk.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gwefduaxz.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gfuhiyiai.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gjulfzunv.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gjzyqmozb.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gxwvclrnj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/guvkagfbu.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gvfdhcbpy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gkadsztiv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/glhdwleoh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gflrhcjdb.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gjfvfvyor.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/giwmdxtnv.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gjqhcoqhg.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gqrbggpra.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gflqddvuf.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/ghqmvofga.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gifjjlgta.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gfrpkkmku.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gynjlxokb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gtbbavrlc.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/ghacixhrt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gebeolgrf.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gnrguhnjl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gwnuxvzip.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gzajpzycz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gifpegdvw.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gjabfyvvi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gblahfoak.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/gmfhpahnp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gwrsbrldw.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/girhgwtbu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gluowsgby.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/giayyliaw.sHtML

files=$(ls -1)
来源：http://mobile.zdbjq.cn/Article/details/gfazreojk.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gsdnmpnas.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.hesvh.cn/Article/details/gckmhmmpu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gjknibsrh.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gkwxoditt.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gtapgcizl.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gwakjugas.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gwkgkjkrt.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.hesvh.cn/Article/details/gzztieawf.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gcnrvmwxe.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gnrjfdgrw.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gmaqpdgvr.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gcmygqqif.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gptngodbm.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gqdyhfqml.sHtML

[R45] 批量删除
来源：http://mobile.zdbjq.cn/Article/details/gkhbjhzbb.sHtML


<!-- 参考信息 -->