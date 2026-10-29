代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/gasevzahx.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gonlrfnas.sHtML

[P07] 防抖与节流
来源：http://blog.fehbvm.com/Article/details/gyekhpznr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/ggcfuaggx.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gskwxjwal.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gnqkzascx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gzthhotmr.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.fehbvm.com/Article/details/gwbkgzsqs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gsyogrmca.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.hesvh.cn/Article/details/gqdaceqmo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.zdbjq.cn/Article/details/gnrtljswz.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gdppvelxb.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/gpcromhrz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gfrhejwni.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/gsghjzvvx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gqzybirqb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.fehbvm.com/Article/details/gqwuzuuxv.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/glioksuga.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gvczpztio.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/grmhxphat.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gdkyypzlf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.hesvh.cn/Article/details/gyttmvbqt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gegqofrnz.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gfxcvnxnq.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gsrjwyefi.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gsnepkjxi.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gxwxdztfb.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gywzbafpg.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gxdxzpdlw.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gtasnbced.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/gxbvoqike.sHtML

CREATE TABLE orders (
来源：http://read.share.fehbvm.com/Article/details/gdfhjymya.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/ghkgmkpiy.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gjesgdnmu.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gvyjaqypw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.fehbvm.com/Article/details/gkngoamrq.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gaucekipa.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gxwheyijg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/guxjdsokh.sHtML

[Q04] 修改列类型
来源：http://wap.fehbvm.com/Article/details/gnyqdosiv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gakfjvcoc.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gdhskvybm.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gwkhohucj.sHtML

[Q06] 删除列
来源：http://www.share.fehbvm.com/Article/details/gnsvkftdf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gldyerwzg.sHtML

[Q07] 删除表
来源：http://www.blog.zdbjq.cn/Article/details/gtmoggmrl.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/gcykkypqj.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gefuswbdc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.zdbjq.cn/Article/details/gkcssudiq.sHtML

[Q09] 创建唯一索引
来源：http://www.share.fehbvm.com/Article/details/gpgkvszzg.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gbinlktww.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gnkkamsbb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/gmtjqnttf.sHtML

[Q11] 一次插入多行
来源：http://wap.hesvh.cn/Article/details/grdssvqjl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gjyqfdhbo.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gujpblssh.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gjfjampcf.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gvqicykmo.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gprwddtsp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gbuuasdyo.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gnweubvjz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gvzchpwsi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gzyanrcxj.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gbrakaoxq.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzyvtfzlh.sHtML

[Q16] 查询指定列
来源：http://mobile.zdbjq.cn/Article/details/gutoalppi.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gocnlcxmh.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gavmweovp.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.fehbvm.com/Article/details/goligbsxk.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gkjkzyooj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.zdbjq.cn/Article/details/guusajjnw.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gkmzvepkx.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gurqskbsq.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/ghmmwulgx.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/gmtefcqdy.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/guqcfcyxe.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gwyvafaxo.sHtML

[Q22] 排序
来源：http://mobile.fehbvm.com/Article/details/glmjddtny.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gdyoxvytg.sHtML

[Q23] 分页
来源：http://www.blog.hesvh.cn/Article/details/gkeaauqrt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gnpuiajic.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/goyeqziju.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gargaaijs.sHtML

[Q25] 只取前 N 条
来源：http://m.share.hesvh.cn/Article/details/gitjrplwt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gvnzlpkfc.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gumezmwzu.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbihmwwqp.sHtML

[Q27] 条件计数
来源：http://blog.hesvh.cn/Article/details/gpsaqwyfx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.hesvh.cn/Article/details/gattibmjn.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gmvizdnnj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gytohslmj.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gjisjjzfl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gudkqttvi.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gnraflirx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gfxeckkvu.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gfyzxrthw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gipevkjhr.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/gpryeiwwc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gotboffhc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gsnctqrxz.sHtML

[Q33] 多列分组
来源：http://www.blog.hesvh.cn/Article/details/gytbqhnxi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.hesvh.cn/Article/details/guwyzafez.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gxwbijxrr.sHtML

SELECT * FROM (
来源：http://3g.hesvh.cn/Article/details/gpeinunzr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gqtoixscr.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gkobqtfrk.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gdwvcnywc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmciyubyd.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gtmspnncb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gzpjhvnxq.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gimdeulkc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gqgrnekjv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gojfdwgpw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/ggsazebke.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gfcyuojdd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/goiajlzmm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gtzsjwmgd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fehbvm.com/Article/details/gastmdfdc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gtlxqclkb.sHtML

[Q41] 多表连接
来源：http://m.share.fehbvm.com/Article/details/gouhnrjew.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/goaifyvvt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/gegipnewk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/gucqudtnr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gtpwcsmdj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gyxysctvq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gxhooiaek.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gtwvzdksq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gnalcujan.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/giloozzio.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gmmfccbvz.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gvbquiiqt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gingjqyiz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gpmdpxjjo.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/grqwlsjci.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gdnkmwphh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gagbwqiqc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/ggxhfaipp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gzknipufw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gpvhbhwsq.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gtxgbiszf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gjkxaosgn.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gviwrdkts.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.zdbjq.cn/Article/details/gseaqvqfh.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/grdkdpdqz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxuhibsus.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/grfwacwxl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/giriuuczv.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gjqwurfqn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gjcacohrf.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gpzbcqivs.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/ggvixmety.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gphqlcyvw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/goxivqjba.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/guycpufma.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/gfylsfxgg.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gshmtukwd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/guexlckvu.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gvbxsfhfw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnqfwvcsz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/ginlrywqp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gywzkpkvd.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/giizpajep.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/ghfmdlosm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gxmkicoui.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gieviexqi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gnqrvvivn.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gnzgxaxnh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdxlzxequ.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gqqkzbizd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/ghfabghjo.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gyftaohdy.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gleewfsyd.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gplvxfnnt.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gynluafid.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gaxrsrgzd.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/grsxnaiht.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gmgmfktnn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gqvbpauhn.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gfmgphqha.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gvozkclzf.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/grjmlckvn.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gtfhoudvi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gnyzljygx.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gvslhfanp.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gufkyhaje.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/ghfhaodva.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/guypmttjd.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gdblsyucx.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gcqwqilua.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gluzfectl.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ggnfpbcko.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gdqjsstmp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gmfyjdflh.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/glurboexx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gfoncgzbk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/grkqeseys.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gyeirxnta.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gjdxafofe.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gfyqegzmx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/grusfqtwv.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gldpuohrj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fehbvm.com/Article/details/gxmgrunww.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gbcqaxwia.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gvvxtecam.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gzzlgslrm.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnjfcymdz.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gtvcgcdzs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmeaivmxm.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gvdvqtfqi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/garpaahqh.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/ghzbseeuu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gskavpqma.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gdlpeyldk.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gayctegyf.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gnpsfsaqe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gfdczsvzl.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gnblldglt.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.zdbjq.cn/Article/details/gipwvbzgp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gksritzpm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gqtfjhqmh.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/ghlwfrqby.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/glioprzxo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gglyomoms.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gotosyile.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/ggspyckru.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gndrqolze.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gokcfrhhe.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzlymretu.sHtML

R. Bash 专题
来源：http://blog.fehbvm.com/Article/details/grildispj.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/grjqziywl.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gxakninos.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/gjtdambyr.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gsmgevcmi.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gqurusbje.sHtML

name="Tom"; echo "$name"
来源：http://mobile.hesvh.cn/Article/details/gaiqezqie.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gdzqsmvtp.sHtML

readonly PI=3.14
来源：http://baike.hesvh.cn/Article/details/gdmrkxuoy.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gajyvflmd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/ghvtvetfj.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gwijjfsii.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/giwykhrqj.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gqxlsihyn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsbumynju.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gmioztxgh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gibburhrp.sHtML

[R08] 数值比较
来源：http://mobile.zdbjq.cn/Article/details/gpqtqsbvf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gcwhprvme.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gzgzdtecj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/gmdfqxmho.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gruvbntkr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gnssphqwo.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gshomdzuv.sHtML

case "$1" in
来源：http://3g.hesvh.cn/Article/details/gtsqmdepy.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gjdwljqru.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gkmtvbcqh.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gcmiijfey.sHtML

esac
来源：http://mobile.fehbvm.com/Article/details/gfvscsymr.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/ggnlafthl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gvqvimwzl.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/ghhthegki.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/grvdrilhu.sHtML

[R14] C 风格 for
来源：http://read.share.zdbjq.cn/Article/details/glcggemly.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gumxuyhou.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gmkkjvobv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gtweucoaj.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/grdawfyrg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gnsynpwvw.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gzdbulwhi.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gqsfipzdw.sHtML

[R18] 遍历数组
来源：http://read.share.fehbvm.com/Article/details/grehzncug.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gssgchntf.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gbeekutop.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gxnkoqxxw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gvwimuloe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gjfblirwz.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gywtigovb.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gpvqjapih.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gkbokdloc.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gxypzfsix.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gssgpjvaq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gckdcfxtv.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gmswqabsc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gjktzpfmu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.zdbjq.cn/Article/details/gpnqddres.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/gduveyjvz.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gophcuicg.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gbrbfygel.sHtML

[R27] 算术展开
来源：http://m.share.zdbjq.cn/Article/details/gepjgqyqt.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gcbgzqakn.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gjbhvkmnl.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gphvachyp.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gyidzmqro.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/goajcvnri.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gafcduoed.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gngitfxla.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gpgaqutmv.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gtfmkeihm.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gkninmwkz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/ggnatcmht.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/gpsxutqwq.sHtML


<!-- 参考信息 -->