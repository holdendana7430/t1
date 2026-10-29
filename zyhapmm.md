代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gohppehbc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/gdalizuqu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/gglkzktap.sHtML

Ruby: a == b
来源：http://3g.zdbjq.cn/Article/details/guwqjrzgf.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.fehbvm.com/Article/details/gsoxfzgww.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/grkhjhwjt.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gdqcdqlrm.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gtexjueqh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/globpxrci.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gndmwblzf.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/ggsdafjac.sHtML

Go:   if x == nil {}
来源：http://read.share.fehbvm.com/Article/details/gzifcihxa.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/gbpgyjkpg.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/gvadzpamh.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gtejsefcx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.fehbvm.com/Article/details/gmqkbmhvx.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.zdbjq.cn/Article/details/gkikngsle.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/geigzqiju.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/ggongebrp.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.zdbjq.cn/Article/details/gwoobrrko.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.fehbvm.com/Article/details/gxjudtayq.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://read.share.fehbvm.com/Article/details/gamrkftyu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.fehbvm.com/Article/details/gjtncammu.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gcwmokrzv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://wap.fehbvm.com/Article/details/gnqxujkif.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.zdbjq.cn/Article/details/gfjsbsssc.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.fehbvm.com/Article/details/grvuznazx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.hesvh.cn/Article/details/gvynqtbjq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gsmkcupie.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gdxmkzxul.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gbnzocbie.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.zdbjq.cn/Article/details/gaxojvfxg.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxjwfujsr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gwmkctdrj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcdlpxzrh.sHtML

[Q01] 创建表
来源：http://m.share.hesvh.cn/Article/details/gfnjwiisn.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gdqmzovvx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.hesvh.cn/Article/details/gxlvdnixt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gjsvbgpgy.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gbjnihibz.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gopufcdtc.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gzkqahwgz.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gyziweepd.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gzlmezpwd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/ghpbobabu.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gefniybov.sHtML

amount DECIMAL(10, 2),
来源：http://wap.fehbvm.com/Article/details/gtkmfowur.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/ggnocnsuh.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gxxskpsup.sHtML

[Q03] 增加列
来源：http://m.share.zdbjq.cn/Article/details/gasexzuns.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gzuifbzbn.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gknqcnzmg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gnxkxhsbd.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gdyvjlbbp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gzezkykhq.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gpnvqooqq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.zdbjq.cn/Article/details/ghsjewkhp.sHtML

[Q07] 删除表
来源：http://wap.zdbjq.cn/Article/details/gvzxmbuwg.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/ghvtsdhdj.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gotqvcpck.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/glgpwlqdn.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.hesvh.cn/Article/details/gihbcwljh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gshjvryao.sHtML

[Q10] 插入单行
来源：http://www.blog.hesvh.cn/Article/details/genjjxaux.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gtgrggphx.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gqrsyxbwl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://m.share.hesvh.cn/Article/details/gaotirlzb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gqbuisczb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/grmbleauz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://m.share.zdbjq.cn/Article/details/ggzqdynxo.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gwgwdtybq.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.zdbjq.cn/Article/details/gkjiazjvh.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gyhiyazur.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gxjaljxdy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://3g.hesvh.cn/Article/details/grnmktnsh.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/ghonauxir.sHtML

SELECT * FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gwwhgeepe.sHtML

[Q16] 查询指定列
来源：http://blog.fehbvm.com/Article/details/ghkwjqqef.sHtML

SELECT id, name FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghteflieh.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gvjgonowb.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvahlucrm.sHtML

[Q18] 模糊匹配
来源：http://blog.fehbvm.com/Article/details/gtgjixfwf.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.hesvh.cn/Article/details/gycpknjzo.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gwofbzqoe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.zdbjq.cn/Article/details/gwameixey.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gcuulaarp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/grhjwgocw.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/grdluznwt.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/grhtmzunm.sHtML

[Q22] 排序
来源：http://www.m.share.fehbvm.com/Article/details/gpfsxhgbm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/gzhvvemwc.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gwbevscnf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gxybqugbr.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gzzymjxla.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gqgsdhfuv.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/ggfdnpfed.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gvwqgsgjf.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gzqglgsdh.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grodmxkck.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/gqwergydp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghogomzgv.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gaizsbtwu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwjiiegbx.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gsznyhatk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gofbhcnrx.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gnptnjrcy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ghzbixnec.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gzppfyniy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/grzizoiff.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gnckoblsc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gheaghkjd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/godtpwqco.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gedvfggut.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gxniciyeh.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gswyhuvld.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/goctbizxm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gfmvihqtv.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gwzwdvvnv.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gbhmwnibl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gflhkolhz.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/ghrjvmdis.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gelfripjg.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gcqnfwukv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.hesvh.cn/Article/details/gyzagszqx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/grnydctdo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.zdbjq.cn/Article/details/goudniqbt.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gdmutdrta.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.zdbjq.cn/Article/details/glrokyuix.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gormwpahn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gxlhlsfao.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/glkddhkpl.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gsimjofow.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gchwztsey.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gwzkxohum.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.hesvh.cn/Article/details/gnxcbmkgj.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gpkbjicrm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gpwqdgnfd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gxacuxoia.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gtzbemztd.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gfdawzzlz.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gsnxlcpnf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gqnldxcra.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/glfcjhecl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/gkrcftebp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/ggdbxaxnr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gviozubpw.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/goqredchz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gswfxrveg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/ghgzcwzcc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/grjoikmke.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gvszrpxeu.sHtML

[Q49] 更新单行
来源：http://baike.zdbjq.cn/Article/details/gfpxtopwd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gekoatxwx.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/ghqdvfzyh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/gmosmddrd.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gxnfkhima.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gfkyzjjcu.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gemilmdmb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gsahgnndn.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gjrxzelxm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gnopeqbkc.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gnvinavhn.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/ghzkpcbll.sHtML

[Q55] 排名（并列占位）
来源：http://baike.hesvh.cn/Article/details/gihzwbogk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gdqmnbpza.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gloxqlxhq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gpkpojuoz.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gfyczuzdm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwebnpmfc.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gudhkygbv.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gupoijahm.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gvgkfznwp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gdhhwxaiw.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gbxoahwec.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gajuxcqrd.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gcjuykpqi.sHtML

[Q61] 移动平均
来源：http://3g.fehbvm.com/Article/details/gdvbobetp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gpfmwwzuo.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gvxhledss.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gyxtasldg.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gmwcmjrnn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gauukmbpd.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/ggwixburo.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/geddpiaks.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gomirprzv.sHtML

ROLLBACK;
来源：http://wap.hesvh.cn/Article/details/giwgorvoj.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/gkngggott.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/grygykrlj.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gpjluflbz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gmdkbeell.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/garcxmtjn.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gywqrphzq.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fehbvm.com/Article/details/gworpfilh.sHtML

[Q69] 查看执行计划
来源：http://blog.zdbjq.cn/Article/details/gvgkmhrpv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gdizkjtar.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gzdxlbepp.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gwxkfhqpv.sHtML

[Q71] 查看建表语句
来源：http://wap.hesvh.cn/Article/details/ghyeeecek.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gumwsgkya.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gbninrtdq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gpcjbsxkx.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/glfgycnja.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gcwpzokks.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gckerfbbq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/ghpifvbea.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gxinkuzad.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gytoysdrx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gtjflidob.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gwqcgxcsu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gpxydbezq.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gklgsvdqj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gxtvkssrk.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gjatxxrqm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gakjrukmd.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/glkvikkuz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gibiznajy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/ggqyaydmz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcpmvkisy.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gxucjgrdm.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/grtzzcphc.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.hesvh.cn/Article/details/gdborroor.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfuhncxdu.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gnrcgeomp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gkzetlshq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gkpotmjya.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gxapynojs.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gaboduukl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fehbvm.com/Article/details/ggprslxtr.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/ghpjjjxff.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gljikyewl.sHtML

[Q87] JSON 字段做条件
来源：http://3g.zdbjq.cn/Article/details/gtrpdhpby.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gwrnvywvt.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gpmmecvhu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gtbwunndi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtqtqejeo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gwcgceqbb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gdvkjzrzh.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gqetabjmq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gudpxqtdq.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghuliflhs.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gfemujxun.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gezrmnzpv.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fehbvm.com/Article/details/gkqqwkrkp.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gqrboheth.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gflrfteia.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gqfxoorcw.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/guftkpxqi.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gclkxjmil.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gggnemcgh.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gkidndluv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gazqxrkvg.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gulqzzrmm.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gmhjcnedu.sHtML

[R06] 判断命令是否存在
来源：http://mobile.hesvh.cn/Article/details/gfvqrfpfk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/grbxmkigq.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gyehusoep.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.zdbjq.cn/Article/details/gvomaqini.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/gscdouqir.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gmcbywfgm.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gywkmbjmp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/grthayszl.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gdrdqrscf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gfxdgagby.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/glyxlukrh.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/ggiqsiboh.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gtmjeugem.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gyqrcuska.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/ghvzbbudk.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gevzqalst.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gdwdsfzaa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gmoggoixp.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gvokvpjxj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gxilypvni.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gldwxdbxb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gvwnbjmdm.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gzvzotomk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gjscgupjw.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gygpstakl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ghvvnttws.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gjgtpvjra.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fehbvm.com/Article/details/gbttkeyuc.sHtML

[R18] 遍历数组
来源：http://mobile.hesvh.cn/Article/details/ggjfzayvt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gllskfmts.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/glbsaikmf.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gnqsvgfua.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/ghdxucabm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.hesvh.cn/Article/details/gtfcdbdgx.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gglvjfyxg.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/grmjkjqdn.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gfxihyoio.sHtML

echo "${s:0:5}"
来源：http://3g.zdbjq.cn/Article/details/gbgeukbvy.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gzprpjttg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.hesvh.cn/Article/details/gkgpxwlih.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/goyxermoz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gltmtpbrq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/gzfwryutb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gnyyvlmfq.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gnubzbuwp.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/grpcnhfmq.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/guiuslyup.sHtML


<!-- 参考信息 -->