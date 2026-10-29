代发 wailian999

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gomevvulb.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/glvlnedno.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gmhduxzbq.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/goesrjuxq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxtggmcoy.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gnynjqewc.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gudlkprwi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gmgpejizo.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gzlznkfyd.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gbikizfqx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.fehbvm.com/Article/details/gmkglxler.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbudyqebd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gtdcryeoc.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/geimkwlgg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.hesvh.cn/Article/details/ggeyivtwq.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/ghcfmlmcf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/gcagwrpez.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gvfqiaioo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gugxdtgdf.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/goqmsjlhl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/grkieourk.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gwybmdkry.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://m.share.zdbjq.cn/Article/details/gczqizhbv.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gazfblouq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.fehbvm.com/Article/details/gcaxxdyxc.sHtML

[Q11] 一次插入多行
来源：http://3g.hesvh.cn/Article/details/gkvaleybv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gbsixoelj.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gxqwbgwtd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.hesvh.cn/Article/details/gbiiavfrl.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.hesvh.cn/Article/details/gpszdewpg.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/getiwupxe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.zdbjq.cn/Article/details/gzgqfposq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gvxsdeuzc.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gczrkefzo.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gzxsowphd.sHtML

[Q15] 查询全部
来源：http://wap.fehbvm.com/Article/details/gmacfnqnx.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/ghldncbxf.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gxbftegax.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/glqlrcbth.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gllqyibkv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/ghvxzaawg.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/ggbmzljke.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gpnyymved.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gzgfevmji.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/grsfgqahd.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gbbalzabx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.fehbvm.com/Article/details/gghzaqojh.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/gezywsbdo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gecvuphhj.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gwcerkjkw.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gqfsysirk.sHtML

[Q23] 分页
来源：http://blog.hesvh.cn/Article/details/gwtcbjrrn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.zdbjq.cn/Article/details/gowtysoww.sHtML

[Q24] 去重
来源：http://wap.fehbvm.com/Article/details/gsgsberyn.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.fehbvm.com/Article/details/gfcthuubg.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gwduppapb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/glvhmdozy.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gpvjfajqu.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.hesvh.cn/Article/details/gisxnlwcp.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gkuuhvrdi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gvuxjqwnr.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/goufqqrtb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gtpoxudcz.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gsrzgpyps.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/grpjrbakk.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gjcvcohqu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gvcuhkeff.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gbnnqfygi.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/ghoxofhsx.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gvzbbqjok.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/grgsfeghh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/grdavztkr.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gsjrmjqsn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gpjfqxcco.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/ghmqoqump.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gzervalof.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gmpmhfqln.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrqnqnhy.sHtML

[Q35] 内连接
来源：http://blog.fehbvm.com/Article/details/grnsfpgnh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/grvqfxiea.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/gkudfuclm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gwqywreua.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/ggovpisky.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/grlsyzhwk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gpqoafkru.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/geawdxuhi.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gevloehzx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gqgtlfohy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gwxcdlzix.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gptszcjgz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gcrirbxwz.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gfjsmwudf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gtxewjlja.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gnqocxwcq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gmsnscwox.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/glkkalkfy.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.zdbjq.cn/Article/details/gjzkpovwm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/giwssnath.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/ghafhfhhs.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gtyibchzi.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/geysnvbok.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gfekquccl.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gmsmjtcdy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gscqnwymd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/grwlnvbjj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/guuukspib.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/gjhsekpkn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/glpknohgx.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gkxiobpes.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/grueemkst.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gtbhtsgwk.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gnehxwnmb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gtrtogufo.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/gqzrqrpao.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gqebgxjms.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/gdmsyspow.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fehbvm.com/Article/details/glbpjwisz.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/ggxfwapff.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gxdjkaojc.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gemhxfrdo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gqtxogrwp.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gtglagukw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gkrbslowy.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gasdzyuuz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/glqbpeltd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gpcgpnvcj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.zdbjq.cn/Article/details/gpksojmlz.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gnozkolrq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.hesvh.cn/Article/details/gfldhvznv.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gaaifniqe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gowlorhas.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gmvuslcbq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gywqfuzsy.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fehbvm.com/Article/details/gwgzwwsov.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/gmyygekhh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gflcyltek.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gilpvxuqp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/groizjsoq.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gvtjtfrxn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gzronqkgp.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gycbxsmpk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gbduqkayi.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gsxyaoftu.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gviltumos.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/guybzaqiz.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gvytbriyn.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/grymnqcle.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gozzpbdtk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gedfximax.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gocffdnsb.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gpmffbvul.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gngeizgog.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gkwjsvjqf.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/ggkvwatiq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gglcbgjqa.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gvyicctfy.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gjkvvydcu.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/ghllehstl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fehbvm.com/Article/details/gohhgxaao.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gvfpabeoo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqnvcyxly.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gwlyeeyqo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gwxijbcvk.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gorfimjly.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/ghphvzmpe.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gavlwugdh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gewwyqonw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/goechixwo.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/gdqdsrysn.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gjdoeyvzn.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gtvpxeshb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gehnnzpio.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gsgulkivh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fehbvm.com/Article/details/gfqeuuagu.sHtML

[Q79] 字符串拼接
来源：http://wap.hesvh.cn/Article/details/gcqsqchoi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gmqgxcskv.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gwdgokdmu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.hesvh.cn/Article/details/gumrjwlsr.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gnzolaylx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gxnqdtgld.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/greyxhten.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gbcfawfbg.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gcojnajjy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvyyoiebv.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gfhekjhpt.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/geayezjfh.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gpmixhgqo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gfdkkecwb.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/guyutitbv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gxaoaijje.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gztcfqkot.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gpwmzrxwk.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/geilfmbkx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.hesvh.cn/Article/details/gnizzrcfz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gidszqobe.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/getdagyjs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gnkwvwvlt.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gxukmhtgq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gfgrqsqxd.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqpkjkfvh.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gwygkuxrp.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggoqgytwk.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gtxwywsth.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gjuxeckvc.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/ghsvdeybm.sHtML

[R02] 变量赋值与使用
来源：http://read.share.zdbjq.cn/Article/details/gfcyajgrv.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/grltrdrur.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gtgnyyscq.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gfihmhqmm.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gzraogatp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gfrweocki.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/grrcmnhdo.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gdnwlvein.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/ggvkrphgj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gqbqabbbu.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gguwbqptu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gjurubuni.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/gaiceyqrr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/grabydupl.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/golazmmfh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/glsjnuakb.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gqvwqyiyi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/gblxwwwem.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/galtdbyof.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gbyfteryh.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gorrzmalb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/ghcmjtytf.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gxckpwthc.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gwlupohtr.sHtML

[R12] for 遍历文件
来源：http://blog.fehbvm.com/Article/details/gybvglbzj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gonknevxo.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gnngackvk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/grbajdrio.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gijtkjohr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gcrflyzxk.sHtML

[R15] while 逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gjbtfrcra.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gfwtxkkmi.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/ghrgqgvgf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/ggyvnuqtr.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gsejwddzn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.zdbjq.cn/Article/details/gxlqbtfje.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gazvicnht.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gxlfhehyl.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/gouizrsbg.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gwugzjstu.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gpnxzzpnt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.hesvh.cn/Article/details/gcnchpgbe.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gvybuqevv.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gzvjjfurl.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gcdcyljtm.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gpqywnfeo.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gmdjjmgel.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gynzujokt.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/gyneutkom.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gwstmvopu.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gtrhdkldf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gouhgbdna.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gsfuvruzm.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/geysqupip.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gkpeadmet.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gztzeafew.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/glvxtdifj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gsrpeicfv.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/glcgiumbc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gpabdvzuc.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gohkukxqm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gvfyhxcju.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gszjvlzya.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/ggbyumnmx.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/gtisbjlit.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gytshrrhh.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gazmphysv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gjlhtiteb.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/gvnagodqh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gxecdjdbv.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gqpbnjceu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fehbvm.com/Article/details/gregcimpz.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/gtodboiqi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/goapquzqs.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gvslqpyfo.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gnyptwntx.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gedelksxv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gayrgholl.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.hesvh.cn/Article/details/goirvxroe.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/girmzdail.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/geflvceel.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gzeyeioij.sHtML

[R41] 丢弃输出
来源：http://www.blog.zdbjq.cn/Article/details/gzzqjrfdh.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/glzwpjbqk.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/grotqggih.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gwnrfnaij.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gndlwjsnu.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gpgwgglwy.sHtML

[R44] 按修改时间查找
来源：http://www.share.zdbjq.cn/Article/details/gyjzobgdo.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/goqypatla.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/ghmzkjzks.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gdwoqkykf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gkatfszct.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gqpmrgyin.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gbnbipuhx.sHtML


<!-- 参考信息 -->