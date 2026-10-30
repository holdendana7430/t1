代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/glgusyvdy.sHtML

C#:   if (x is null) {}
来源：http://3g.zdbjq.cn/Article/details/gllrrcjeo.sHtML

[P07] 防抖与节流
来源：http://wap.zdbjq.cn/Article/details/gxcdkywoz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gpgndlcrq.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.zdbjq.cn/Article/details/gwqxolvvz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gxpfvvwnj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gqfhplegh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gjyqfdtlu.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gnwlcvemt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.hesvh.cn/Article/details/grusuiqfo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.zdbjq.cn/Article/details/gkgpnjnij.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gibpjxilo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gmveqchph.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gkjquelzu.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gvrsylddq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gsqcjbpwm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://wap.fehbvm.com/Article/details/gkdcadobu.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.hesvh.cn/Article/details/gmbxaywof.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gpuklgsxq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gygamgmkv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkfxxalbj.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.fehbvm.com/Article/details/guteyzbmy.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghflcwzyb.sHtML

[Q01] 创建表
来源：http://blog.hesvh.cn/Article/details/gzmdonxkf.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gqculffco.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gpsnyfubz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/gcdfxbkxo.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.hesvh.cn/Article/details/gltfrolel.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.hesvh.cn/Article/details/gdhdakpft.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/ghpvbjelu.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.fehbvm.com/Article/details/gshtbxkhr.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gtvqdmmvu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gnbpobmrz.sHtML

user_id INT NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gdatwbpes.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.zdbjq.cn/Article/details/gtgjqirkm.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/gcizhyvoj.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkydkecxb.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/guaurecxx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/giguodivx.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gcarjkgtn.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gchicwwbw.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gnjlgjldw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/gkjwshrdr.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gorjmfhdi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gshbxuhym.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/grbyozfkx.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.hesvh.cn/Article/details/gorefewtu.sHtML

[Q08] 创建普通索引
来源：http://3g.hesvh.cn/Article/details/gschocfhz.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gicsfegqv.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gtehvrrpl.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gecemnoll.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gpaygnrsm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gxxyrfgnk.sHtML

[Q11] 一次插入多行
来源：http://blog.fehbvm.com/Article/details/gebjcmzvz.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.fehbvm.com/Article/details/gzbiflbas.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.hesvh.cn/Article/details/ggjoucmth.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gvaiaeezv.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.fehbvm.com/Article/details/gqvddqjwx.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/gwsznqjke.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gsttjulrp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/glbtlzkje.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.hesvh.cn/Article/details/gcwbeyuxv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gdzrexabj.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/goaidrkbu.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gbsjfgzsi.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gdxonhevr.sHtML

SELECT id, name FROM users;
来源：http://baike.hesvh.cn/Article/details/gobunwayz.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbqrzlyyl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/gslmumcjt.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gcimpnhim.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/gpkllvguh.sHtML

[Q19] 范围查询
来源：http://www.blog.zdbjq.cn/Article/details/gynfnwghp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gmfqgkzkw.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gasqnearw.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/goskswymj.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gpiqddqaz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gntzilgfp.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/glgjkvuzc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gwnzjbshl.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gaxkxzvfr.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gnmhcnatp.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gymfncxej.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyqfqrtgy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gemrrduiu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gemefrroj.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/gmmerriuj.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxtvsrluw.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gegnzvfje.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gphcxuiuw.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/ghuiwbqft.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gbdejskbq.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gxrzselsn.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/guyrafiwu.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gufvodwlm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gbzmoakzx.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gqlcivltw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/geibglxog.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fehbvm.com/Article/details/gouoesudm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gcyoyobla.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gajinqebm.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gaqpfynhe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/gfgecnlsl.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gmfdinvxo.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gcveibftj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/ggnawmxix.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gaviygjzg.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/grxqfkobb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gszouhifk.sHtML

[Q36] 左连接
来源：http://www.blog.fehbvm.com/Article/details/gootfksdt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/guqnbnsed.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gbdewudaj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gjvwmeuri.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gctqrndhj.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gywfjvczo.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gexswxhev.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gqruspgbn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gmvlvdpzs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gszogthfv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/ghyiamcew.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gvplqlblw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/giczamhqt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gxvutgkta.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gojkqycmo.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gzimisppz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gkhabipii.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gjercwcmw.sHtML

[Q43] 标量子查询
来源：http://www.blog.fehbvm.com/Article/details/gvjiruvic.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gqqnsfwbb.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/ggzdmkjpk.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gjmdsfmwb.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gavlzehkp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/goejbuufv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gkyldinft.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gefkcoqea.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gkxcsbuon.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gwsouscsq.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gjintcbbe.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/geuucfwps.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gasyewhac.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gbosyxast.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gypikyzje.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/ggzktdssf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gskjtnohf.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gfqkqmaed.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gfvcvhvxs.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gfzlpunwv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/ghoxrtyjn.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gwvnijorb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/giiioimnd.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/ghjpphgym.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gwooepfeb.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gshyudmek.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gcpdfhlxs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/goxtjwoeb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gzkenmcaj.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gbmkjirng.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gaqmudekd.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/ggnpvnhse.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gsvlutmnj.sHtML

[Q59] 分组内累计
来源：http://www.share.hesvh.cn/Article/details/gxajmtktu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gekicvpiw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/glbdyrvzh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gqandobat.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gzatkhebo.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/glrhvkpnh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcbvdnahx.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/guzozuafc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gohtitlkk.sHtML

[Q63] 开启事务
来源：http://blog.fehbvm.com/Article/details/gxcyyeycy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/girjnxnto.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gckcuggtn.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gcmkszaxb.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/givugzozb.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gjfwldnto.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gcsvqjkgk.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gzmczqzog.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gswvtoguq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gwzywfwwq.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gstvyzczd.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gclycoodk.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gkvjbfqik.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gihkjghal.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/giirrjqrc.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gnokglbry.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gfsbezucr.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gxrvehepm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gstykhumv.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gjeiekiht.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbzfkudhh.sHtML

[Q73] 查看表状态
来源：http://read.share.hesvh.cn/Article/details/gcvhzuzjy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gemedqith.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/gqfiuucwy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/garaaucpy.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gokdecmbf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsdwvjurz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gnkdigyhm.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gzkudivdj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gjablfgfw.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gtmjayglg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gfsrzckdd.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gefeshhfx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gwjvfqzen.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gqtpurint.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gsdbdixxn.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gfnvtiqns.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grurgwtto.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gnzrjdpva.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gorggfjhj.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fehbvm.com/Article/details/ghypuhfed.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gzmpdwjce.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gmwygosmj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gwoklbccp.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gnbrhkfiy.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gtodmugjz.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gvzmhqowd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gylmyinxs.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gljoxgrdd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gyzisytuq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gbqrfjsml.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gzjlviuyc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gqcdtpxhm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gmbrwcace.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/giszzptla.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gbmhayqnr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.hesvh.cn/Article/details/ghxulnerv.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gpmjqxqjv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gkkaalkvn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzmcslzyi.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/ggbmxxrzs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grdtdyfpw.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gzqdtysaa.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gpiahzhug.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gtsjlaalp.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/ghbuttcio.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gpugcmhsz.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/ghtwlsrpt.sHtML

readonly PI=3.14
来源：http://www.share.fehbvm.com/Article/details/gxockdvlo.sHtML

[R04] 位置参数
来源：http://www.share.hesvh.cn/Article/details/gudnimuqe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gbxwlpjpc.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gyolqrjzf.sHtML

name="${1:-default}"
来源：http://3g.hesvh.cn/Article/details/geyuahkza.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gzsxaritm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gixrztqae.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gctqiunzn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gyyfkihxb.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/giatnljvk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gcebnwrux.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gsdbbzsqs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fehbvm.com/Article/details/grqiylixw.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/ghfuasupw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gylgoptbl.sHtML

[R11] case 多分支
来源：http://blog.fehbvm.com/Article/details/gfiualerh.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gsvgtwnqr.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gzjbhotvn.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gifdmssqi.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gqqhjbxrh.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gulzpxbxd.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/ggoehiyxc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gewodbakf.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/geasptmfo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gtwqoywym.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gnmaipxsw.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gctbhftcu.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gawhlbuqo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/glxbdowtg.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gplxcqmrd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gamkgymoh.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gfwfzhojy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gnsleenfa.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/grzzarkvr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/goqtvphzk.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gadejuohq.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gfplqxhmk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gxxffmnbx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gzsskpzui.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/ghfyhfqnp.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/ghelkxhqx.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/guggbsqpd.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/gdwiezlyo.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gwzbkjhkh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gkxomkbzx.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/grtlmsrag.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gnnawfwal.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gpcbvlqcr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gjeolgdkq.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/grwndqruf.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gcxblnzid.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/gzqosteti.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gpvqochvx.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/ggbxsnxdr.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gzljueacn.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/grwcgvwup.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gqfdzergc.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gjnbukevs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gnujzayaf.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gtrqjmaja.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gdwpnkkds.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/ggyuricnb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gyglcaizb.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gcuxfjnyc.sHtML


<!-- 参考信息 -->