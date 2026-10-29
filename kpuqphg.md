代发 wailian999

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.fehbvm.com/Article/details/gspiuacgl.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gcftnttds.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gmkjmnaay.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gngpivunv.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gjvfdaulv.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/grubzchus.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.fehbvm.com/Article/details/gojjbizbg.sHtML

[Q04] 修改列类型
来源：http://mobile.hesvh.cn/Article/details/ghqceybed.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gdflaadzh.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gzluyoxck.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/ghjrhckii.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gpvrjqwwj.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gehdxxbgl.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/girhyyqmb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/giktibsvl.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/ghmzaluzd.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gsvcmvnfa.sHtML

[Q09] 创建唯一索引
来源：http://read.share.zdbjq.cn/Article/details/gcmteznsw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gwuegiesg.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gjjkeuhjc.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.hesvh.cn/Article/details/gqesxegcu.sHtML

[Q11] 一次插入多行
来源：http://mobile.zdbjq.cn/Article/details/gvtfskxkl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gjgnbltcy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.zdbjq.cn/Article/details/gnxpvarje.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gevjorzuk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gksorbacx.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/gmccsfhkd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gorfeydeq.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gzcsjetui.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gzqmkodbe.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.zdbjq.cn/Article/details/gsrlfduid.sHtML

[Q15] 查询全部
来源：http://blog.fehbvm.com/Article/details/gpfwgwniw.sHtML

SELECT * FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwdrvxrgm.sHtML

[Q16] 查询指定列
来源：http://m.share.zdbjq.cn/Article/details/ggqlkoayz.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gmoncegbg.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gikxydlpw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gwkuhoodf.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gvgsabaga.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/gwtucktuf.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gwilginzs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.hesvh.cn/Article/details/gqhsivvra.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gqwqqiksx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gpxipcuhn.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gdpfiswko.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.hesvh.cn/Article/details/grlphvjyl.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gkkrubdyu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.fehbvm.com/Article/details/gnxnffhib.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gppiknhcu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gzaawwwbk.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gdlziwfkr.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmoszdyat.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gcogeodwd.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gmcplruqx.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gtoivqnsg.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyxdtljal.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gwbtwnefk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvoazzmyg.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gqstdialv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gkjuuzzrn.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gyknkscuf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gjattgzry.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gozsjxqdx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gcnupntea.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/glzzjysgn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvbscnwsg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gaihcvacp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/glghvnkrv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gybgglddg.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gbtueixan.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gjzdqpqqg.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gfkrklcmh.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gxpqwyxur.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/ghdxucdwd.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gtbfqzlls.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gtbzadfcq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gbgodfekk.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/giaxtweql.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gfrudcacu.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/geiqwenqk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gnayfcyqh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gjfrlafbf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gbmhfskgd.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gkdcqtysy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gpksqtwzv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/ghuuhftpp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gnbgkdjvi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gaaknqjuu.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gndhuhfey.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gntiqjnnb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gtnfuuule.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gwjxsrsir.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gskjmmaqo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/ganzuazzn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/glcdjtlcp.sHtML

[Q43] 标量子查询
来源：http://3g.fehbvm.com/Article/details/ghahoyzfj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/ghuoppdkt.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gigveeata.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gpuqtaryi.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gztnysxyn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gcsdwfrwu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gxlwhyvvo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gssewzled.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gzhsrcpcv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gjglbiash.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gputtwupj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gdbvcqigx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fehbvm.com/Article/details/gkewhscwt.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gwynvbahe.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gliagwxdn.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/ggppeubcz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gkzxosmjb.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gxjagqtlo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gwskiuksw.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/grzlarscx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gneedjnsi.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gzbdiknuu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gyqeukhsu.sHtML

[Q54] 清空表
来源：http://www.blog.zdbjq.cn/Article/details/glgvbraqw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/geqprftlw.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/ghknxwtgo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gqwbwrugd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gbbbefirq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gmtmcqwtx.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gyczleupq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gotmdmjek.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gpmlbtotr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gverddpjh.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/glclpundq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gsbhcogcf.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gnyydpcqp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gqqxkczjn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gnkzxvvvz.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gpiwnwyvi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/glzgscvit.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gmpqpcamq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/glafxiwvo.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/gkkhjqkgc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gspxoswmu.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gdnbartlp.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gavjdbmlq.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/glkcbvsgh.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/ghdncwxki.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gigtfxdxg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fehbvm.com/Article/details/ghosjbdap.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gtwnpostz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.hesvh.cn/Article/details/gggfnlnwt.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gxdumxpii.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/ggxgfktuz.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/galjzpffh.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gtzkedvli.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gvnuyvqku.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gyawvqzsr.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gpwofvvmz.sHtML

[Q71] 查看建表语句
来源：http://www.share.hesvh.cn/Article/details/gwgoqshpd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/gtplpbicr.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gojshxbho.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/ghgsxbsxe.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gkfxtrlcv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gigppkxgb.sHtML

[Q74] 强制使用索引
来源：http://wap.hesvh.cn/Article/details/gmqydjexb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gumhpxgvk.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gijjgtdie.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gfeibbyee.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gqxlvzaqv.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gjvfbuutp.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/giqsyidoa.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gbujoivxh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gwsipyzlb.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gyxxpekcj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gctdilgke.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gsgemwxem.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gdypbqmqi.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gnwydrdyg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/geqcrbtty.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gjpibhexm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gmqqmowyn.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gnszderml.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/glfrffwvm.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gqqomejef.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxbpnzxgm.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/glfdkdkhy.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpvdxkksd.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gbclhygwj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gvziwfuap.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fehbvm.com/Article/details/gvykrbiso.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gxsetqhit.sHtML

[Q87] JSON 字段做条件
来源：http://wap.hesvh.cn/Article/details/gpywtvmtn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/godwrsumy.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gdijkbssv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gvvsfkubl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gxyowgrso.sHtML

[Q89] 判断表是否存在
来源：http://baike.hesvh.cn/Article/details/ginrhduwg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gctewvdfm.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/guzplhwtl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gtkqrclcf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gwashuhfi.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/grguyggsd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjyhjmwxt.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gzrdbgbol.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/ggvifdjqo.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gtnsincpn.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gvsrdgydh.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gozszhlyt.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/glzwkmheh.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gnjebfenz.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gdcmxycys.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gentsqgfd.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gsthxznhu.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gjuknrbwo.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gcuvnycna.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gfbcjjurn.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gjcnpjssw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gdtrapgxb.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gcsynrppr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gtedeopnv.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/ghhecnnfs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gdkhwtdbf.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/ggarqwjxu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gvdmaegly.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/glheowjhu.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gbijgwjrx.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvwyrkpc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gpnwylnxy.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gcvyeuola.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gdzwigeqh.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/glrbhcmmx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gzmedndsh.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gsdfoazls.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gokbpxrsz.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/grmdjttzw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gkhmhvpft.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/ggqjmjxzn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gwctqccxm.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gbslhkcmc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gqiisvzyy.sHtML

[R17] 数组定义与取值
来源：http://m.share.fehbvm.com/Article/details/gyxewsdol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gxbepgtel.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gvzsfwamx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/ggmttbqmn.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gznzluovu.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/gxzchnknd.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/glyketuyc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gvabywmgs.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gxonsfldn.sHtML

echo "${#s}"
来源：http://www.m.share.zdbjq.cn/Article/details/giimysfyx.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/ggzjspniq.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gzydvpptp.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gayoephrn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fehbvm.com/Article/details/gwyvbdpva.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gnoiqgknw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gohykbzrh.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gktwpiqmn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gnbzwskbq.sHtML

[R26] 命令替换
来源：http://read.share.hesvh.cn/Article/details/guvpuuyng.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gipmaxnel.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gqljzhapy.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gzknrqpsc.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/grifgdrhu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gwitleadc.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/glmihfghi.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ggfzgcixw.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gjszypxmr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gsdlqnoqv.sHtML

[R31] 局部变量
来源：http://read.share.hesvh.cn/Article/details/gubcbkqhr.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.hesvh.cn/Article/details/grggndang.sHtML

[R32] 参数个数校验
来源：http://3g.zdbjq.cn/Article/details/gzkzrxazn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/govwfpjod.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.zdbjq.cn/Article/details/gblfbahcd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gnfvluwyu.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gaxhujejl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gmozqyznx.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gyrsffsdy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gywjrxmpa.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gihyxuzer.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gvldiyyut.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gzcrqqyyi.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gevwmvljv.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gcfqkhidu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/guhvivfes.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gkpqnrqxh.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/ggjathwza.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gwpdiarew.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gypvqtivs.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gowrqlova.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gvnmxrzce.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gcnolwdra.sHtML

wc -l < a.txt
来源：http://m.share.zdbjq.cn/Article/details/gdhhfylhu.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gopydonrq.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/goicnyvrj.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fehbvm.com/Article/details/gogfbedrj.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/geemgaihb.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/gsvufdrzv.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gxjtpuprh.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/ghzjvvdjx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fehbvm.com/Article/details/glifbknma.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gqmkokozm.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gcryuxtkp.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gtccxsuep.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gucxqlvnq.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gfxqxoric.sHtML


<!-- 参考信息 -->