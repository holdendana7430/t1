代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gtijixypa.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gjhpwhqzb.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gjwlyqdog.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gqdsthmqm.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gaauxrymz.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gkumlvoxe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.hesvh.cn/Article/details/gkfvygkih.sHtML

[Q04] 修改列类型
来源：http://read.share.hesvh.cn/Article/details/gdkivqkgx.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.hesvh.cn/Article/details/gbnewrqwi.sHtML

[Q05] 重命名列
来源：http://mobile.hesvh.cn/Article/details/gddviyhwi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/giatjdbxr.sHtML

[Q06] 删除列
来源：http://www.share.hesvh.cn/Article/details/gjhfzvsaa.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.zdbjq.cn/Article/details/glbzhzxut.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gzgwwongy.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gilvxfcwq.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gflqhghqf.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gefglneaz.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/ghilyziob.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gbaycbncu.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/gyapubhcd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gigorqfmn.sHtML

[Q11] 一次插入多行
来源：http://blog.zdbjq.cn/Article/details/gvtkanflj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/gecvvdnhe.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.hesvh.cn/Article/details/gwcjalirl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gorgusjce.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/gjbbbkufv.sHtML

[Q13] 忽略重复插入
来源：http://baike.fehbvm.com/Article/details/grlgosjza.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gauewfmms.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.zdbjq.cn/Article/details/gsptkeocl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/geuanopte.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gvtjbdqqc.sHtML

[Q15] 查询全部
来源：http://read.share.zdbjq.cn/Article/details/gqszzuxly.sHtML

SELECT * FROM users;
来源：http://baike.fehbvm.com/Article/details/gclfbolpu.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gvtgjuirx.sHtML

SELECT id, name FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcrimlhfz.sHtML

[Q17] 条件查询
来源：http://blog.zdbjq.cn/Article/details/gqwhvgxtw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gptajpmqq.sHtML

[Q18] 模糊匹配
来源：http://www.blog.zdbjq.cn/Article/details/gkvfmvhpc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gxiowdpmq.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gshosxbni.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gryjoxijx.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gsessaraf.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/ggrnxgpix.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gcczmszhw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.hesvh.cn/Article/details/gpoacytur.sHtML

[Q22] 排序
来源：http://baike.hesvh.cn/Article/details/gvvlquxju.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/grjldwtht.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gxhahirhl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/geyukfywj.sHtML

[Q24] 去重
来源：http://baike.hesvh.cn/Article/details/gzjemahfu.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gclgrsrvv.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gpfjignli.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gaeleqanh.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gkqmylojw.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcemtnykh.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gjnqwxzvf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gdprrecuk.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gfxcpuymn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gzzdbbxbr.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gaibzzdib.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gttcvoebg.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gmygffjck.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gfnptthck.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gpjywxljw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gyddqjeiv.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gytoffsiq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gxwzdwizf.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/geazzgant.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gcghavqkp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/gtmqnzmvx.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/glqwfcvai.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/grqvlgwvt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gumeyygxs.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmcksuqqh.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gpbkdadko.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/gmsmgcrzd.sHtML

[Q36] 左连接
来源：http://baike.zdbjq.cn/Article/details/guaabgdzp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gtemmgsqe.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/gfpibzwug.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gvkioigxs.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gxbekkbnk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gfptjsetg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gxjalqvty.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gukfsbczp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gmkgcpqqq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gnielwexu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gxnufisur.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gpukswldm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/ggztabfsg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/gqkvhggvi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfqitzhn.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gdzvzkxzv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gabimggax.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gjcxheapg.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gwxmynwgx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/glwdnmwxz.sHtML

[Q44] IN 子查询
来源：http://m.share.fehbvm.com/Article/details/gbatjzvak.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gnmykwxsw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gijyykcla.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gugsmxxvp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/glrlctgdg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/glzkijogn.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gbqrwvhoq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/gtbmqzokq.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gzguctpvk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/gyhomccwl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.hesvh.cn/Article/details/gnvzohgbf.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gywrgcbmq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/ggbryblhk.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gmktuftsa.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gnvlgagng.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/gcflwhqwy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gugleedkn.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gzpvrjpjt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gppourtwm.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/ghihcoqil.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gpcdzvhvt.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gsjncelxr.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gbiiknihg.sHtML

[Q55] 排名（并列占位）
来源：http://baike.zdbjq.cn/Article/details/gbesihyit.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gpqoadhyw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gwzvvzwsr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gfubigaae.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gwyzqtyhx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gcbuxkxxp.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gdkziiqks.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gagczsgjp.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gwxbtjevf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gfqxdilcj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gkkrkdzie.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gtpqgmagf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gdmlhmsdw.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gsshqnsag.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpjblsdgi.sHtML

[Q62] 分组占比
来源：http://www.m.share.fehbvm.com/Article/details/gliskixlg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/geedrdiiw.sHtML

[Q63] 开启事务
来源：http://baike.zdbjq.cn/Article/details/gqorrmnhd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gvlyffogw.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gyyrbcwkf.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gqiwoqjoe.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gkcgqfyne.sHtML

ROLLBACK;
来源：http://3g.hesvh.cn/Article/details/gmtjmnddq.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gymizaqqc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gxougoffn.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gybrlcwqv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/ggblrasdm.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gdjcgbnde.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gbnmboajx.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/glbcxzehd.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gqscssgtj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gijgbfnje.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gbjajdccy.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/geckznfpt.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gwbxubuok.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gixrkdjqf.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gxpkxnayb.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gomtkkyjf.sHtML

[Q73] 查看表状态
来源：http://wap.fehbvm.com/Article/details/gctqcblwq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gkgpahafj.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gfelgqfai.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gqiqhsiqf.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/ggtrvrcli.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdgzzoycr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gkjqtjpvs.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gsithsjvq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gdhwtunpb.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/grpkcibcd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gfaxroara.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gcxpzlaki.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gtycrngbw.sHtML

[Q79] 字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gqbuvemlb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fehbvm.com/Article/details/gqvjzepim.sHtML

[Q80] 字符串截取
来源：http://wap.hesvh.cn/Article/details/gcemkusqi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gukhwbckf.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gyzibhigk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbtnimtgt.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gfflonnov.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnkpmkmdv.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gqqexqgtu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/goafdizvz.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gfhnjbejq.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gdomgcijn.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gohjgophf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gvasjmlda.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gcjimiilo.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gqgixcbsl.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gjodfagnr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gbayvmahh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gdwsbwtrf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gqsklrscj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gohztbxsq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gkhqptwup.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/gmhcyveut.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/glqdmyqli.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gwfslkyvr.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gdghbnuak.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gkadsdxgn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gfdlvzwta.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gcyhrmfiv.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/golfqzdbx.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gkfrjatsg.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gaherdinf.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gftxgttpd.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/ghmlzuhbo.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gfdsfdjwq.sHtML

[R04] 位置参数
来源：http://mobile.fehbvm.com/Article/details/gtzjimath.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gjtnxqkcn.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gpziruswu.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gqfxozhez.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gdiieuuhw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/grwnapmiz.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/glzyopqgt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gsraicvlp.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/ghupmykzl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gomeqfbhm.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/glxnflqdk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/gmygildvv.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gmbhuwaff.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gmovcbpdw.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gpxyhnvxl.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gsvixzdrp.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gujilkdhv.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gazliapwo.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/ginkuahig.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gweadtnzw.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gortioodt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gcqofcspn.sHtML

[R13] for 计数循环
来源：http://read.share.zdbjq.cn/Article/details/gymjswlzp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gmeqgpgix.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gwtfsaujd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/giexhfyys.sHtML

[R15] while 逐行读文件
来源：http://wap.fehbvm.com/Article/details/guozkzgig.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/ghljlkjje.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gwlhjadql.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gqcjnjytn.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gsytfqexc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gafmnktch.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/gqztyzgwl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/ghxesbdka.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/ghnchonjx.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gaccscwua.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gijsaqnpz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.zdbjq.cn/Article/details/gbdgykmgm.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gdubegsuu.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gtdzssgio.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gzsxaniod.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gxerbypuj.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gyncnrdjw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gjejcxvmb.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gvjhhnfrr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gahzjgfid.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gfitpmwrs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/grcjftrhn.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/glufajigg.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.hesvh.cn/Article/details/gpdaclmsl.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gjejmdtgv.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/guxktjhtr.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gtdtatiee.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/geymdkhgz.sHtML

[R29] 定义函数
来源：http://3g.hesvh.cn/Article/details/gbowhmorw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gavzttjaf.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gctgpfiwo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gxpjarxop.sHtML

[R31] 局部变量
来源：http://www.m.share.hesvh.cn/Article/details/gojfeyupn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/ggvmwuupb.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gpnwvykbt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/glswlfqtt.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gwxtquqjy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gzapknjnw.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gurxnvrqg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gbwgomlyx.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gjqjmwsdp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/guwpxsrzf.sHtML

[R36] 并发执行多个任务
来源：http://3g.hesvh.cn/Article/details/gygayjfxi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gmgiexaoa.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gdpbxadfq.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gjtkvtbdv.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gakmwvmpx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gigytgmwb.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/ggtdxiebq.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gurbjxcca.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gqnhxaioe.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gykkdquut.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/giusetrsv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fehbvm.com/Article/details/gpmgsfqwr.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gistrkpcz.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/ghzvatqxn.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gnfkjmujm.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/ginkiemrj.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/ggqmiddol.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gduqbfbdl.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gsbuuceqf.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/ghrkskgzx.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gqviwyjxk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gizsrqvvm.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/glhytgqmz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gajvvpnsc.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gzsfpjjuh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gckdqmnhg.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/grumfngdo.sHtML


<!-- 参考信息 -->