代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gfjddvjyy.sHtML

C#:   if (x is null) {}
来源：http://read.share.fehbvm.com/Article/details/gkbscxlzz.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gieisdtsd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gwzejjjwh.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.zdbjq.cn/Article/details/gaoywztxt.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gkrbyoxns.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.fehbvm.com/Article/details/gnsrrvffo.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gvjrvaclf.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gofiwstvk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.hesvh.cn/Article/details/gdovfjujd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/grbtexqbw.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gbnatghlf.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.hesvh.cn/Article/details/gjjatqnqu.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gsuchjfmp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.hesvh.cn/Article/details/gtpaonoxt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gaxzfyzuf.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.zdbjq.cn/Article/details/gsthyghws.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gywnzzafj.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://read.share.zdbjq.cn/Article/details/gmvqhbrie.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/gjanghjlt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gouptovff.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.zdbjq.cn/Article/details/gpliblqqb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpllyajhr.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/gollhgtkt.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/ghumxuwyn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.hesvh.cn/Article/details/gagymygnt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/grckpehwo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gsehujfbs.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.fehbvm.com/Article/details/gxhxidsmq.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gartoxpmz.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.zdbjq.cn/Article/details/gjojquzcj.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gzsgkmlrj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/gyekmetej.sHtML

user_id INT NOT NULL,
来源：http://mobile.zdbjq.cn/Article/details/ggqqdwqxj.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/gfwcblovs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/glzcrkfux.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gejcvszer.sHtML

[Q03] 增加列
来源：http://www.blog.hesvh.cn/Article/details/grysqrwhq.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gyocwkqmc.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/glwuxromv.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gpfujeycu.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gqgkjnyhp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.zdbjq.cn/Article/details/gupgihvfh.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/gbgnlamio.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gfhbwpdtm.sHtML

[Q07] 删除表
来源：http://read.share.hesvh.cn/Article/details/gvgcqfbbg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gzlotwtrd.sHtML

[Q08] 创建普通索引
来源：http://3g.fehbvm.com/Article/details/gynqpyzrt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gconikpdo.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gdfnukpwl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/geivxgvuz.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gzitnmvji.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gmjbsllwp.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gpepeyxae.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.fehbvm.com/Article/details/gkyuucbvv.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gotypoqfr.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.hesvh.cn/Article/details/gnmnkeypq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gosgrekxu.sHtML

[Q13] 忽略重复插入
来源：http://m.share.hesvh.cn/Article/details/guspwtwrz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gfdjjjyfo.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gaecadvkt.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gfknrfotq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gyqswsolk.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gcadmqqtj.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmfdximxu.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gpaosdlcz.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gruppjgpr.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gibchdgcj.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/goseavsnc.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gltdigwmj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gnqtriytp.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/ghhsjnoyg.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/guqdbjvtf.sHtML

[Q20] IN 列表
来源：http://www.blog.hesvh.cn/Article/details/gwrningao.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gucanzhur.sHtML

[Q21] 空值判断
来源：http://baike.fehbvm.com/Article/details/gxmyrobuw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gztjafewc.sHtML

[Q22] 排序
来源：http://www.blog.fehbvm.com/Article/details/grcvmvurq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gghclkrek.sHtML

[Q23] 分页
来源：http://3g.zdbjq.cn/Article/details/gxasuvsbk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gcfrpshda.sHtML

[Q24] 去重
来源：http://blog.hesvh.cn/Article/details/guksmypwf.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfgmmnaao.sHtML

[Q25] 只取前 N 条
来源：http://wap.fehbvm.com/Article/details/gehrzbozg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/grpvnyomy.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gpgkfowut.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gcryozmww.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gnxzcmzwb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/geamjyzlj.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gufoerptr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/grxzhskze.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gfauzbfyl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/grhcbqdhe.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gppqqrejl.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/glycdjgro.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gixrglnfu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/goxcskxmw.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gxvexwdqn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gjvldtvmc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.zdbjq.cn/Article/details/gmoexoxsx.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gykauvpfi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fehbvm.com/Article/details/gzjkkiawl.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/glautqtfd.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gnovocjda.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gejzblqyx.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gwlwssgpy.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/grbbdabph.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/glwleuino.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gephzrqhk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gpklfgrgh.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/guxkojpgl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gdedpesta.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gxcibtgda.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gvpgejkci.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gmayahxcv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gutssnvsz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gsrrcgjqg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gddjfgwrn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gkyxvvfdy.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gfvxuujwt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gutnqjupc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/goklcjjrs.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gqthbmnvd.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gcggrczlb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gcjpsmfxg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gwjzfgnlq.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gfoxhppkx.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.zdbjq.cn/Article/details/gagfpgoqg.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gdlrvnslj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gecxnfgtz.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gjcvapnft.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gavbchgad.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/garrevesr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gxhfyfokt.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gpvrredgh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gqhjbzfat.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gwafzsusz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gkcbjfttj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gkahafcsk.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/ggfkjyuhp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gghbknnvd.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/govybjxga.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/glnfxqxiu.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/gqslusnjw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdgtxanqa.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gxrihaaku.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gxoqcrlmz.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gplmjrvyk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/gwlqyxeuy.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gnowwxkph.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gtrlaavts.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/genwlucxs.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/ghntzqxxy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/ghhoffrqg.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gyalufora.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gyzxvruew.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gxbvmfihq.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gxiwsxlxc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/geomjwhhz.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/ggybiqqtj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gvyemcifg.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gxjrzmfhk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.hesvh.cn/Article/details/gljqydjcs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gjcssdgrt.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gogwszarj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtnzzikgt.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gctzurrcx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gxxuilefb.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gzkszsgwx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/ghjbevdkv.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gldsnbgsu.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/ggqdmjnsd.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gfunaoqlc.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gdidbrjtb.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gyzaityxo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gybuzadle.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gflwfghys.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gywvyuhri.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gdiebboyq.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gikntxrpp.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gjtasofns.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gydjfkkvd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/garluaxre.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gybpdmzry.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gqyaivgyy.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gceovzlya.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gguviesse.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gejfnsfeu.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfcfpxvkh.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gxhkgbotc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gzpquzcnz.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gunkgxkqh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gyuceoldj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/giimjxrib.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gubmiqerg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.zdbjq.cn/Article/details/gbpfxzldl.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gifwqkwtz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/grpgvquna.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/gqglnbutb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gqoqduojh.sHtML

[Q78] 当前时间
来源：http://mobile.hesvh.cn/Article/details/gtogfscgw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gkedlywwp.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gukchflbg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gvhsojcib.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/goppagtgg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gbjwgbact.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gfhsnkoow.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.hesvh.cn/Article/details/giflopbrn.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gfwxuhpgu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjjjbwezk.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gkxhiitib.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gldcmevuh.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gjppizqft.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gshtxhwhy.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gsaimntcb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gurblfmua.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gluigjzic.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gubktpyaa.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/grwwhtvwe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/gffhqayoy.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gvxyowhvb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gmjatrvva.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gofzogllp.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gnpdpxnfn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.zdbjq.cn/Article/details/gtmzaloet.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/ghzmmpocg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gcgkbyomx.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gfabormez.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/ghrptnoqg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gadyfbtbj.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gmisolgbo.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gbnmpmyom.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gisxdbdcs.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gonlzdcvr.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gnlnjiycu.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gaquzneur.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gdztrxrsp.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gnilahibx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gjqkfgwzd.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/gniscvart.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/gchjqpmdy.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gwmdfnqnu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gtmunzckw.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gyudbntnq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gihoxjecy.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gcdzhgjbz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/giicxkjtx.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gjjybhldj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gsvnjzjnn.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/gosgkenym.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gslpxatfy.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gfmcnriqs.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gnawanslm.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/ghqjfahfn.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/grqmmzhap.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gzgwavmyl.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/geosgtoxq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gwgvkinpa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gybjtvbzn.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/ggzarqudl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gmcdgzvqz.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gjlabumsz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gojdphjku.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gltbaljte.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gixtpblze.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gqagjebuw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gtfktxnvv.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gmylgdpkb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/giqswzelc.sHtML

[R18] 遍历数组
来源：http://mobile.zdbjq.cn/Article/details/gwmatvxip.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdgjspmvg.sHtML

[R19] 数组长度
来源：http://www.share.zdbjq.cn/Article/details/gtudiyrjj.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gbalrasuu.sHtML

[R20] 关联数组（字典）
来源：http://wap.zdbjq.cn/Article/details/ggsoourmd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.zdbjq.cn/Article/details/gapsxnpwm.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/glqffcaon.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gnnwxiavf.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gzpbvhxxp.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gcwnqaujb.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gankiwlcj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gkuwkhphf.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/guxtkfzwb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gbblduewc.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/gvfaoudgj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/gljooifaa.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gxbrpkqxv.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gdbhxlzbf.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gitajvjkr.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gpcwvbmsx.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/gquifivfn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gxreqxpjf.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gxrrshjtq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/guhudmawb.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gtonwqgzh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gwdpmgguy.sHtML

[R31] 局部变量
来源：http://www.share.zdbjq.cn/Article/details/gxxijffnl.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gvxgdxumm.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gyrjafxhd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gqrsyyjnz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/grzsxjjnj.sHtML


<!-- 参考信息 -->