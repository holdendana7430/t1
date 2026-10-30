代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.hesvh.cn/Article/details/gwqrgbjgc.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gjfbhdxoy.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://wap.fehbvm.com/Article/details/gixhnvktv.sHtML

[P08] 处理浮点精度问题
来源：http://baike.hesvh.cn/Article/details/grtnjeeyy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gxpvfxpob.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/ghrnsktry.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.hesvh.cn/Article/details/gfpsocvlz.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gezxoehoc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.fehbvm.com/Article/details/gakrfstus.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/grwuaprrw.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gdftbxwuc.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gyjyqlzoj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gsevwjcnr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gcnbxyrar.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gcwadsyej.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gjmrhipzb.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gwjzucusg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fehbvm.com/Article/details/geyyaiqxc.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gdnvytrum.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gawaqozhi.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.zdbjq.cn/Article/details/gpuffugwq.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gdgpukhlg.sHtML

[Q02] 创建带外键的表
来源：http://read.share.hesvh.cn/Article/details/gzszdkbfq.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gzktsxlea.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gpbrriwoo.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/giwmtpgzr.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gnrgveldv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gncczjlrw.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gbqynvrif.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/ghvudlmrt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.zdbjq.cn/Article/details/gkcbsggfo.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gszgybifg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gthoneepd.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gnyiubpia.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gboddumug.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gkhgvboam.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gwjywzhbf.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/gpdreiopo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/grrophtul.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gjyfpfrdn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gkoembyhb.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gycllkjop.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gqkcrdgmn.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gknyodini.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.hesvh.cn/Article/details/gcuxbaawz.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/geroaicmh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gfgelvgqd.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gbodsvlwg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/ggrzkdpxg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gjfpehwdo.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gadibxidy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.fehbvm.com/Article/details/gdyjyptux.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.hesvh.cn/Article/details/gptkysnyn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.fehbvm.com/Article/details/gaihnkmkv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gsjaljfyc.sHtML

[Q15] 查询全部
来源：http://baike.hesvh.cn/Article/details/gcjpttnzj.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gvtrltylp.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gpddpwkte.sHtML

SELECT id, name FROM users;
来源：http://mobile.hesvh.cn/Article/details/gexuxzrgf.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gqditekmr.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gcwuffddm.sHtML

[Q18] 模糊匹配
来源：http://wap.zdbjq.cn/Article/details/giwpmeweu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gsgpfgbxd.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gvyjdocdj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gjgzkqwtl.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gygwcbbmi.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fehbvm.com/Article/details/gfzywanue.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gbyqbmrbs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gbzmnosdq.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gedjnvhfq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/geknpstav.sHtML

[Q23] 分页
来源：http://www.m.share.fehbvm.com/Article/details/grpffjndm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gwfbvzhuo.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gitegrnyv.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gioqaigtp.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gbkworqwm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/goiohowkk.sHtML

[Q26] 计数
来源：http://baike.fehbvm.com/Article/details/gcyqootwg.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpuvwdrgi.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gmkqoxqkq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gjvdfbabh.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gvrvsbpmx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gisvnmpxc.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/giiggtisy.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/glvcpbgxk.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gxfmcfjbe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gzbxjlxpm.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gpjniqwtm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gkjyhvfbt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gksvzyxdk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gzqykeiwn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gfgadsnyi.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gncdadvmv.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.hesvh.cn/Article/details/goxlswytf.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gikzaqqbq.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gipivjtod.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gaasjyxzt.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gzkyjbxjw.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gqsixvpsl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gvzxkddhv.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gliuvizxp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gikyzzqvo.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gzqtdjedz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gmfnoqpcu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/gqqjhotow.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gushlureh.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/ghtwkwivv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gljcszzol.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gfuptuqrx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/ghcltrlke.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/gifltmkcb.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gmaosmqdg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gbbofxsnt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/galcdojed.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gwhlmelqa.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gjmfulnbn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gkdnakovb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gklxwjdvz.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gruxudkeq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gyhamxfvw.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gsqoexujl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gsqxaqzpx.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gowanxadl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gjqbeeucg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gydgwgvci.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gpiadwcql.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/gungdapmw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gleanwsql.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gflljgupm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gylmjkrrg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gzouacxnn.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gwtoryavn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gepbjtdjd.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gnxmlhfxq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gxjgwlqlr.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gyobycdxw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gnjjavgit.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/glvsdnumi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gherzmkqw.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gxkpuatdc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gpgdjgyhu.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gjrszbzpo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gvrzhfyis.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/glwlmbkro.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/grgoxbpjs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gkfagzveo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gzjgphwrv.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gwbnkuuss.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gzvvnvvar.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/ghifvozwq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gdtervodi.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gwjaflwij.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gmicaotor.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gacevkjtv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gipgundsv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gnnvfuvov.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gwtbzvrmb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqdnyqudy.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/ggcfcdmgo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gorabacka.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gzcokjaid.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gxrpzuiwc.sHtML

[Q64] 提交事务
来源：http://mobile.fehbvm.com/Article/details/garyjumsb.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gmublrbsd.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gxqkczkns.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gkwilzjqv.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/geiqhojbk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/glrytsxbh.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/grloovqgf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/guzszfmlo.sHtML

[Q68] 保存点
来源：http://wap.zdbjq.cn/Article/details/gyhkigoty.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/gevqlkoyb.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gyjppgqda.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gtmxotqun.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/ggjskvkyb.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gpsnzcotj.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gsvfixxrn.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gottjrikg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/ggsxgqmeg.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gnfrteryg.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gqpcvuvyx.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gtzkkplqt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gpmmqtqbv.sHtML

[Q74] 强制使用索引
来源：http://3g.zdbjq.cn/Article/details/gvvrrxnzu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.zdbjq.cn/Article/details/grxddaurn.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gkyxddcjt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gklxtesyf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gesmeflyo.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gfneateyc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.zdbjq.cn/Article/details/grzaoihfo.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/ghthwppur.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/ggpfkpjpu.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gijogxraq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gzxnolkny.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gsgrtuwap.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gkavvuisi.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gxmewosog.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ggnfkyght.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gdhzsnnbm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxrtuvbdu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/gmbxpuwao.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyiushnul.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/guimytzdi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxmefcemu.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gksvrhixv.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gauxauyde.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gbxyqywdq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/gswrfokud.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gcdfaxgii.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/ghaxaokzr.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/ghivlxzlp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gjhieeuva.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gowtckznh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gwtrxllmm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghpfzpypr.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gxtlwcubl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gijtswnof.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gqypnybxh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gaiasolof.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwnrpzomd.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gvhakjgyo.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjhudwrdh.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gophkomxb.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fehbvm.com/Article/details/gxmycrufo.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gukokdswr.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gtbddtdbe.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gkrcoiihx.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gpqcacvti.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gdgivfgwv.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/geaxrrbgb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gqeeyodih.sHtML

[R05] 参数默认值
来源：http://wap.hesvh.cn/Article/details/gcgdcmynb.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gzzvwxdnb.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gvvufvahe.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gmjqjbhly.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gogmylqkc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gwpqfdxll.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/gozpjwnkm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gjccptkfc.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gxnhmdnzw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/grvrcxwzl.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gthijazpo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/ghtlwcirp.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gnavbthyh.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gsatbwlza.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gbcxnqlht.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbwtbghug.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/ggmtrfvgl.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gdxhqgbwh.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/gqufbqufe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gihnlzybo.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gsjuyjegb.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/grswymgew.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gtdeansqg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/giazjivxb.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gjfogxtyw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gbfujcrku.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/guwyvmwtz.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gannmhzlz.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gqjokcobv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/grsewulwf.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gnpqcejxs.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gjjmewmsd.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gsqboqhux.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gkaosxkqx.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gvcjrbgwj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gkopkulcm.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/ghnktjnkb.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/giitxcsjm.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gfhsggpae.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gzvjclesr.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gtkirqmfh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gajsymmbl.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/ggyaudfdh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/glwjehhjf.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gyaonttxz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gdikedzkp.sHtML

[R26] 命令替换
来源：http://www.m.share.fehbvm.com/Article/details/gzniybwrv.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/guodexxan.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/guefyrqxp.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gubecpatv.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gwwznfnsm.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gvedzulvg.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gjqmxpthj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/ggmtxtybm.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gogxzrrmw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gtybcrupd.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gadbejgkj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gytugfhdo.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gclsiycqt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gdgphbmnp.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gviplgjdm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gifazttdj.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gkdhmiefm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/glmoldaxw.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gohpikxzv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fehbvm.com/Article/details/gpqzbdwhj.sHtML

[R36] 并发执行多个任务
来源：http://read.share.hesvh.cn/Article/details/glosjjcrk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gfizmftoy.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/goskuojaw.sHtML


<!-- 参考信息 -->