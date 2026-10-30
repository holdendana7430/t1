代发 wailian999

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/guhejkvis.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gpzaoqvyt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.zdbjq.cn/Article/details/gclfhoyoj.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/ghxytuyvb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.zdbjq.cn/Article/details/guntfryac.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gzsrblvoq.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.zdbjq.cn/Article/details/gexpqhkmj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.zdbjq.cn/Article/details/gxyxwayks.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gseaczwdc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gqtgyjhvi.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.hesvh.cn/Article/details/glohsnjka.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gqszjcnwk.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gsvzifgcl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.fehbvm.com/Article/details/gpujhqors.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gzkwmzsqp.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gcevvjevo.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/gislnoeum.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gnmtwxnbf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gpetgjxgp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.zdbjq.cn/Article/details/glduskvqy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/guagneqkp.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gzqexgdlr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/glxzcazjk.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gerllrktb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gcyogzhvh.sHtML

user_id INT NOT NULL,
来源：http://www.share.fehbvm.com/Article/details/gykvmcznk.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gkuismeto.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gsnlxcvlt.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/ghoglwdks.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/ghcqfclia.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/giqvspsfl.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gsgzglwsw.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.fehbvm.com/Article/details/gxbgvbvbc.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gxmwyhgcc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/geqjolpfn.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gstfkbaki.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/grxrdsspy.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gmjwrvyot.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.hesvh.cn/Article/details/gqepfwuwp.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gdjlyyyfz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gzvqlcjpp.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gdaqkexyi.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/ghtmoditi.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/gxqqqhnii.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gaalcicft.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gudegyjsi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/govyejalq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.blog.hesvh.cn/Article/details/gbmzuxzts.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.zdbjq.cn/Article/details/gplfxvher.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gyhkebiqp.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/ghechyvgg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.hesvh.cn/Article/details/gocepbaxt.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.hesvh.cn/Article/details/gnqwukeho.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gjmoilmow.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.fehbvm.com/Article/details/gssyyztoz.sHtML

[Q15] 查询全部
来源：http://www.blog.hesvh.cn/Article/details/gutriadqu.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gfigpamef.sHtML

[Q16] 查询指定列
来源：http://blog.zdbjq.cn/Article/details/gataydpws.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnjowdcyu.sHtML

[Q17] 条件查询
来源：http://read.share.hesvh.cn/Article/details/gkbiylhaw.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.fehbvm.com/Article/details/giosqtrhx.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gstesuovu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gyksdgmzu.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gwqezonkd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.fehbvm.com/Article/details/gfpmfzsed.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/gdanxkdfn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.zdbjq.cn/Article/details/gdkswtobl.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/gvsedfdzd.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gkdvcuwse.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/giyipzawj.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/guobuiini.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/gxopfjuzw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gggvuvoap.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/ggyivglfe.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/glibpxhvi.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gbofccrww.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gdujjbrqx.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/ggpmzbtts.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/guyheslfv.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/grfdwqnqg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gqjxnkgcu.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gxuaopfwt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gtpccdzcp.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gsfkrzhic.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gfzqhjmpk.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gohmpdcmo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/grwwxjhyt.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/gslccswmn.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.zdbjq.cn/Article/details/gvzfugnol.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/ghztwosfg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/grdgjewal.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gtntunwbd.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gbwnehwqw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gqlqsfwtp.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gjelwpttv.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gxbubmyac.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/gdkwmiags.sHtML

) t WHERE rn = 1;
来源：http://wap.hesvh.cn/Article/details/givnsfilk.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gvxninmwx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gwzdnzrpb.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/ggfrsquwg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/ggdvurjlt.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gxcypkvgk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gtdqcihav.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/gghziatzo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gfklrjyfz.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gtghviclb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gbqiwcexm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gngixnzbh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gghwhtfqx.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gmzzjqlvn.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/ggjjshqmt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gtlnvjnlz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gpxkhpuof.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gtpyxkkdm.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/glskaifri.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gkabctgbq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gvoituijm.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gfxjetdoo.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gghqkvnfm.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/geizmwrdy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gleyhwuos.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gozdmlldg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gmgqocmgw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gtfryygfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gugdubfqc.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/goxyxflps.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/glrpzehbj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gjyragcbs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gahimyabq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gkjegietc.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gtyldgxcm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/glgiwiavd.sHtML

[Q50] 批量更新
来源：http://m.share.hesvh.cn/Article/details/gxgmqevbf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gcqztszhb.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gesnynjsx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/glqaocdwj.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gawrigitm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/glgxnkrjv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gzsofwdqx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gggfqatgk.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/glbqrjhdz.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gznwhxdru.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gambtgdjp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/grjxbbffo.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gztdnargm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gjelculwk.sHtML

[Q57] 行号
来源：http://blog.fehbvm.com/Article/details/gswtievxa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gauxtaces.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gcnqwdepu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/gxibqjbpg.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/galnylctm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gkskoihyh.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gqpdizfan.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gcsupwikl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goychmgvc.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gonqbhjby.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gaepjoqww.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gwmyliytv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gtikpgngu.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gpyjmhqcc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gqxhrlvys.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/guktxuurr.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gaonfllri.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gzvzqlalc.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gidydfebk.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gjyowxqxc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gwzmuxxld.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gvwffyvtw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gnntfuhdc.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/giwwbqnbd.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/gkgvggrvc.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/gmoeohrfy.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gztqnktak.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gjyvwarlo.sHtML

[Q70] 更新统计信息
来源：http://baike.fehbvm.com/Article/details/gppunjpen.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gfmobgxfa.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/ghmirdmge.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fehbvm.com/Article/details/ggyhipyfd.sHtML

[Q72] 查看索引
来源：http://3g.fehbvm.com/Article/details/gpgggctal.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/grhmbjdnm.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gzhwpwsyv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gistusiiu.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gcfzkqkqx.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gtcpynfai.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gfosfchiz.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gsrcxwynr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gqqtdjlbh.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/gfpbsirpv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gzhenqxbs.sHtML

[Q77] 时间加减
来源：http://wap.fehbvm.com/Article/details/gojfygzin.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fehbvm.com/Article/details/gywtaymat.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gpnjjppvo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gicjrhtfk.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gtvythmsu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gieryuqrk.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gswrnmnql.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gvuzywlun.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gbduunaph.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/grkqegzti.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/grblawgoy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/grcsermpa.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/guxtffyhv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/glbljrory.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gpuvribfm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdifflldd.sHtML

[Q85] 数值取整
来源：http://blog.fehbvm.com/Article/details/gecfdcakp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/glellatpv.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gvlcxtigd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gazqetrdm.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gnwvlmvdx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.hesvh.cn/Article/details/gdcrmroqc.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gnyjrolpg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gdlmphtom.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gjzhmypep.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gjtlntphg.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/guczedyii.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gjkatjffs.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gbwjkkxud.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gqdixgwyt.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gwuuwzzvr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsyvycmoa.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gdmldkges.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gsatvdbpc.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gzdgdcpgk.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gspadzzlj.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/geswmeded.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/ghmjnqctr.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gpvbsowgl.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gcynppgfb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/guxmqyfio.sHtML

[R05] 参数默认值
来源：http://mobile.fehbvm.com/Article/details/gdokyfwnk.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/grgosoglv.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ggargoqlv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/giqyclyor.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/ghcwioply.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/goxybhvni.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gifpilyru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.hesvh.cn/Article/details/gkdldsrlj.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/gwepwbitn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gipfafpgz.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gheggwyyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gewrpbiod.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gvacvfefb.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gdxargxjr.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gtaxpvhzs.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/gakzmgvar.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gdxlkzjnk.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gntciixca.sHtML

[R12] for 遍历文件
来源：http://www.share.hesvh.cn/Article/details/ggrbjezuz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.zdbjq.cn/Article/details/giiwctwqu.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/guxrtsbgj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/ggwapitpv.sHtML

[R14] C 风格 for
来源：http://www.m.share.hesvh.cn/Article/details/gazfywfwh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gjhmeomsw.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/geshlowih.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gtfvgguyb.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/goqrbyhbo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gsvvgeaaz.sHtML

[R17] 数组定义与取值
来源：http://3g.hesvh.cn/Article/details/gogkpenje.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gndjyfwst.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gfivabhfb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gbbhgdqly.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/ghziynmgu.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gxcfxkkqr.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gieztigyt.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gtucztcen.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gxcsfnysj.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gtmipfmxk.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gsovhnbol.sHtML

echo "${s:0:5}"
来源：http://m.share.zdbjq.cn/Article/details/gemgbkvoz.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/geqgjvswo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gpelfliaz.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gucuirdlh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.hesvh.cn/Article/details/gckqwfjzs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gtmvztuhq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gpmlgrstz.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gwqojpkmq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gzqnexzwb.sHtML

[R27] 算术展开
来源：http://wap.fehbvm.com/Article/details/gpbhfyprl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gzhxwyynx.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/giugvsgib.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gqszzqjke.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/goonloior.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/gbxjhfqgr.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/ghifphprt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gjzjfgqrc.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gxitvqnhc.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.hesvh.cn/Article/details/gfrdsjaam.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/gchmesybu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gvyocuppo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.hesvh.cn/Article/details/gbhahprdl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gvijbmadr.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/ggnqwspzv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gasycuafz.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/grsqadcer.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/ghhbtrtoe.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gcqcbsmuf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gijsqurzq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gjsxxobhw.sHtML


<!-- 参考信息 -->