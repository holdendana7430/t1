代发 wailian999

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gzkptjzcz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gwvmwpcvo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gqqgwlwpv.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.fehbvm.com/Article/details/gdyfhdolu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.hesvh.cn/Article/details/gptijukzf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/girjaoabl.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gvgyqyuqx.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/ghcmbiztb.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkuyanijx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.fehbvm.com/Article/details/ghkjocezv.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gydnlfuio.sHtML

[Q01] 创建表
来源：http://3g.fehbvm.com/Article/details/ghsaeyoyh.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gkjurayqp.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gapouijmj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gyyzdyews.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/goocimgsx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.zdbjq.cn/Article/details/grkohkhdj.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gkokfhmhg.sHtML

[Q02] 创建带外键的表
来源：http://wap.hesvh.cn/Article/details/gaefnfwyg.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gywramlmu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gyvsxktph.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/gtqpqilns.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/glidylkii.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gesbbdaug.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gmktchnqj.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/ghadqjebk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gtwcintze.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gqvkmzjyt.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gzjttpbie.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gzevzmpxo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gzalpqucq.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gigvckuxi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gfbjtafed.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/giftdshso.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.hesvh.cn/Article/details/gdwcyugqr.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gcksjmbcc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gfxjzhoup.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/gamrnezcs.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/glztrnbjj.sHtML

[Q10] 插入单行
来源：http://blog.hesvh.cn/Article/details/ggnvzvjzt.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gcvvpmken.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gaetqlcuy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/guziecopu.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/ggaqqqsiz.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/gpwbzrfkg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.hesvh.cn/Article/details/grglatzlr.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gpbwdyqqx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gzybijzct.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gznpqxwid.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gtuyybyfj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/guefbfysb.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gitosrhuc.sHtML

SELECT * FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geqnoyowf.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gzzesqvnq.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcczlncxo.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gpcjmbskx.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gyldnobhh.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/glajxewkk.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gryqszevb.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/goabzcfkl.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/gevzezrxm.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gvybxwlcz.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/gpyrrlteg.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gnnpjdzoh.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gtymnedxp.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gkgzlwcgm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/ghlhqfnns.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gnokhqdry.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gvtltdwxw.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/geylmivlx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/geanbpwtk.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gqzstgjyj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gfcunmzyt.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gfviwaksr.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grpemluvn.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gnyekeect.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gzbeajjti.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gqaxuwyey.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdbhkzkbx.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gehlncmer.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfnziltdk.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gbvaperca.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gddyjcvfi.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gjxzxcxta.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/goclgkncj.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ghxstvjuw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gyasbonqi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gcmqpfrqb.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gwjiiuobs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gxuhgmmou.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gornumpsk.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/goxfzbkkc.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gnmnmgnsf.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gahxcalon.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gboplccho.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/glkirihgl.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gaioddwsw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gfheyzwrh.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gpgaicgaz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gxewlneav.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gjbsrlfgf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gvyuvmogt.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gxwhpnzln.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gfiptfsle.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gpvojhswz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gobnwsuyg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/glvrsaogf.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/geqjugidr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gbwtejksq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/gfoowubwj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gxpcyisse.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gwuqwgmbk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gkjvmclfh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/gaknyjedl.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gkivxctjl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gyukccurz.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gecffboov.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/geebgjemp.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gqhiemzjw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gndaqlmwl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gxwtegzms.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gtgupxrdm.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gjfzxfwux.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gmlpsgvjr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gbipohxjp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gdplvahik.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.fehbvm.com/Article/details/gnuzsypqe.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gwcemadtr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gtxjmkhpe.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gmmftcwcs.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gpvdhybia.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/guxuecjsz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/ghduxspre.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gapvyxdsg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gnjgicuoj.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gipxprdxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/gaudrcklr.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gaxtywyvu.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gljvthcea.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gvupvyqph.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gwwuczjod.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/grhvpwmkf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gjawjmwmi.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gpvedthmi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/grswebpzk.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gnpuqqbse.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ggzlyslpl.sHtML

[Q59] 分组内累计
来源：http://read.share.fehbvm.com/Article/details/ghyhitltq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggfilpeju.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gceqcyzqx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gnnjiezud.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggcbkbfdi.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/galfefakj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gnapozcer.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gbmzndudy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gboynpspc.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gxkhdnfbm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gpuxjohxp.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gfzzxmtxo.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/ghrvyufyi.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gvgtrftmy.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gabipkdct.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gmzjttcpb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gbuadxbwy.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/ggonuctxw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gysoctjnj.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/grmkjxzgq.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gsmyahnwz.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fehbvm.com/Article/details/gjbdwveif.sHtML

[Q69] 查看执行计划
来源：http://m.share.fehbvm.com/Article/details/gxafzcafg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gmbkfqwvp.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gmsnruyae.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/ggducfuhq.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gibpemwuq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.hesvh.cn/Article/details/gfpyhdykv.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gdpidwger.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjfbtegen.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gbvazhxpm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gzcjpotun.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gdwuceiuf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gehvjzfio.sHtML

[Q75] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/goayjlrvn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/glnpnmdid.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gguvtwczr.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gueqfpekv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.hesvh.cn/Article/details/grqbyckhk.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gsuzgtkwv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gxrervdrn.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gmphljnpq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fehbvm.com/Article/details/grrjdvtef.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gsldxihxm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/gdkazztpo.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gmgdpqptq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxgszqtbo.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gftuaqksu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gdscstmly.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gyvxoowaw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdxayifqd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gnfktxaec.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gceedfztt.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/guacuwswz.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gswzjjsaa.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gcealjoil.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/griwdgnvg.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/guyngfjtf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gqfeavuwj.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/ggggsyfuh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/gihkijcvo.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fehbvm.com/Article/details/gclcpgqfq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/guuqwmcpt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/giimiayun.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gjxgczczo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gjyeocudi.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gvctzhjem.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gokphvnku.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggfzotcfj.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/grxsifiaj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdtdgkakv.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gzkzcjoqw.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gqspkwqdj.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gidfuxqul.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/gjmrbiasj.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gicgkixvo.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gmjyadfva.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/gjqplcetm.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gfnunyzaa.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gcremjuua.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gorvkmlxm.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gxnbrltyd.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/ghlfuerbj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gyxkrvhoj.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/goednjkfh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/gbwobfiut.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/gvnbyhywp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gtecyvugk.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/ggibhcxuu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gpofhrccj.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gmpfsgcou.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/girdaexge.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gpihtsahs.sHtML

case "$1" in
来源：http://wap.hesvh.cn/Article/details/gwpkuleyl.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gfpcaishh.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gzdilfzbc.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/gzdzvplnb.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gwxcbgowz.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gcdjwufod.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gjnstcixq.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/gfqzppsev.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gntzflgba.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gqfivztwu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gbuxmibds.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/guqzwlwni.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gdwgcpqnj.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gjvyajlrt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gfbiilsvt.sHtML

[R17] 数组定义与取值
来源：http://www.share.fehbvm.com/Article/details/gkrmhcukq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gyctwycfp.sHtML

[R18] 遍历数组
来源：http://3g.fehbvm.com/Article/details/gewggmekr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/ghoxmlhio.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gcduqbffu.sHtML

echo "${#arr[@]}"
来源：http://m.share.fehbvm.com/Article/details/gkpvsobvo.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gpphntqvd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/giwjnpuro.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gmudbwjsv.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gfaefmnxd.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/grnsqmpsb.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gdgyivzul.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gvexdqizf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gynpzpilq.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gvqbjntzt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gwmnjjkzn.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gjqghctin.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.zdbjq.cn/Article/details/gjbpcxrzi.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gdpcztxlj.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gwrskdwbm.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gkhumslth.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gakpctkgz.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/gofgvfjsh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gjkgypenz.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gcnorweix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gcvzdtiqh.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gqtufbgap.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gmcxlnxrl.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gavdixbwu.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gzlhvtiah.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/glclvhvrc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gpalkafut.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gkbmrjlit.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/ghzxhkmus.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gytzytlos.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gdhotgdal.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gzaswyesb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/glukafyxb.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fehbvm.com/Article/details/gfmbhzwaw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fehbvm.com/Article/details/gynuomwsd.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gvsjqwkro.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gzslygcfc.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/ggxjdyyrr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gqecazkai.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gphgqohpk.sHtML


<!-- 参考信息 -->