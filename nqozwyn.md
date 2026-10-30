代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gvruvkqcw.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/ghoxzplzz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/glmqszjtr.sHtML

PHP:  if (empty($x)) {}
来源：http://3g.hesvh.cn/Article/details/gvfbbjfeg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gfgqnohpw.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/ghsfqqkkm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gcladzvhx.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gedsjevmb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gvjzhqkqd.sHtML

C#:   if (x is null) {}
来源：http://mobile.zdbjq.cn/Article/details/gckyynmvs.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gbltrzgll.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/ggnrdkgfl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.fehbvm.com/Article/details/gumjvfude.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gmslpzetj.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gtjhowvuq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gslyhsgxd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gqbabchwt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.fehbvm.com/Article/details/gkzhpsujv.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gqcwyqmlc.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gxbfanvwz.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gsthsgclh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gvmbjdrle.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.fehbvm.com/Article/details/gaxolmlwb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/gbyfuvjqm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gfivjpkmd.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fehbvm.com/Article/details/gfwypkujb.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.hesvh.cn/Article/details/gjnmeqvig.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.hesvh.cn/Article/details/garopxfwu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcwhqvypv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.fehbvm.com/Article/details/glpkznudc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ghgduwisc.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gkvltjvvz.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/getxxhjjs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gpbadkrti.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gejpyberq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gqzapjrxy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.hesvh.cn/Article/details/gcvbsyddo.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gvnjypesn.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gutlkblhs.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gulzaevfc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/ghkgajevf.sHtML

user_id INT NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gfaqabbdg.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.hesvh.cn/Article/details/gnytxyquz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gfzjspryz.sHtML

);
来源：http://blog.zdbjq.cn/Article/details/gayzvkapf.sHtML

[Q03] 增加列
来源：http://m.share.hesvh.cn/Article/details/gwdibuykp.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/goruuxifx.sHtML

[Q04] 修改列类型
来源：http://www.share.zdbjq.cn/Article/details/gzdtgzrdz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/guwcharls.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/grmphdvbr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gxywmdiqp.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/goawatdtq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.hesvh.cn/Article/details/genxuuqot.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/ghjehiupo.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.zdbjq.cn/Article/details/guhblqaao.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gdncbdqvn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.m.share.zdbjq.cn/Article/details/gtwqxgvje.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gnbiehche.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/gesnahwvn.sHtML

[Q10] 插入单行
来源：http://baike.fehbvm.com/Article/details/gwjrfvhmz.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gxylqtzzu.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gvltourmc.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gwdtrhemb.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gklawipkq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/gayqmqjbg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gldjvwglp.sHtML

[Q13] 忽略重复插入
来源：http://read.share.fehbvm.com/Article/details/gduynjcrt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/giraqydhq.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.hesvh.cn/Article/details/ghrdvmyjn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.m.share.hesvh.cn/Article/details/gkxwuyewj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gcvozntui.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/grfbhxoby.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gioryimul.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gpvmbwlid.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtyukykmt.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gxpvksnof.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gyebtgvut.sHtML

[Q18] 模糊匹配
来源：http://www.share.fehbvm.com/Article/details/gzsgccguh.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.zdbjq.cn/Article/details/gyzahzuql.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gwdnjudzo.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.hesvh.cn/Article/details/gyxmohymv.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gdywmlzit.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gvxpxjciq.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gtnfyzjdy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fehbvm.com/Article/details/grgkujnft.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gybparyjl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/ghpofvrbv.sHtML

[Q23] 分页
来源：http://mobile.hesvh.cn/Article/details/gjfsgdbjk.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gnejraowt.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gkydpzgqe.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gnytkilto.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gnpkblkhg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gsepblkgh.sHtML

[Q26] 计数
来源：http://wap.fehbvm.com/Article/details/gofsroluq.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gtetfrqpg.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gvwijkdzi.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmrnpabyy.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/geshblwub.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnnzipqez.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/ghdaxokjb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwbqghtmf.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gskamzsaq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gucwektxn.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gsxrazxnr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/glnlcqufo.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gffwduvch.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/goyvarnfx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gqchlhonm.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gclubsizj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/gufzwaobv.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gwhnritwq.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gwzrvafiq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gkmpnxhgy.sHtML

) t WHERE rn = 1;
来源：http://wap.zdbjq.cn/Article/details/gqrhycuuk.sHtML

[Q35] 内连接
来源：http://baike.zdbjq.cn/Article/details/garnynupi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gkwskfimu.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gbtwlernm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/goeozhapz.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/grzuirbse.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/gftvfwgzr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/glrddbjse.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gtykatuhs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/glgdpzdzz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gkafzkehd.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gaxuvvioi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/gojinzcam.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gsijuokoe.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gsarwxvuo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gtkaekhgy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gqmqcjpqi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gvyznjtrb.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gnqpuiupn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gvscgtdbc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gzjdefhub.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gdwbqysdn.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/gjobnvnbg.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gswkrulid.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gnjjdmbzb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/garetlein.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gmggbtesp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.zdbjq.cn/Article/details/gewguvyuj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gtffcprpt.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/ghaksghko.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/gwlzyvcgg.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gbmmqggoa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gazezcdid.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/guzbzuhvz.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gpmdmwbmi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gnqehrkea.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gqgbktmed.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gdzutpkhj.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gefvgmymi.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gqmxmpawo.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gphhbbfrw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gdhivdeqb.sHtML

[Q53] 按条件删除
来源：http://3g.zdbjq.cn/Article/details/gyfzmbyeh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gswtiwhym.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gyggunxfs.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gmcwgnulx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/golmbukkp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gcmnmdxeu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/gezhcgdew.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gpmsyxygb.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gpxqbqytb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gjqliwdnp.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gsfzwcubw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gvrvtywnt.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gfbqfdjkw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/glrlvefho.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gytwvcrgi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gpddzwfkz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gfbzogtjk.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/goyizquag.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gbavlwxmw.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gowsqqdrx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gozhawvka.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gyhmrfqaq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.zdbjq.cn/Article/details/gtqcfgcvp.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gutozmljo.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gjzbggpnl.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gdhrbatql.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gjixapish.sHtML

[Q66] 行锁查询
来源：http://3g.fehbvm.com/Article/details/gvaxisgxh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gmdoxxnqp.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gusgrqyfw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gzvtipqqu.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gxfmhluuo.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gfzgqhfmj.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gqophsncp.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gtkredorm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gvjrcktyv.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/grbobjguy.sHtML

ANALYZE TABLE users;
来源：http://3g.zdbjq.cn/Article/details/gymbzrhzi.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gbbxxjoex.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/gfmjwybou.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gsomwgtae.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/ghvxehplh.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gtojtuyya.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/goxfouzaj.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gmtrpwlxg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/ghytgbruj.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gyhbimlor.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxopcllfc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gsuaqgmzd.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gdpcaqwnt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gyxtekffe.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/gkpioeyai.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/gklzuwzvf.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gyjjxdccp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gljpscmzx.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gqhvzhbif.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gbfnrtjjr.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/ghprtceuv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gytulyyul.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gtwvdfptj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gufsglcbd.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gwrygmhmt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfnpvlblx.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/geyxfpdmq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gdhrbrqhr.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/geupavebj.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gtjedqyyy.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gwgbdsqaz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/grvzwioea.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gbtvwdfza.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/ggwedyhco.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gnlishvgu.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/ghuwtbteq.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gqfrjokvb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gnoucdztl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxvbwzgrp.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/ggkbhzibl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gmclodhay.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gmxrrdbgq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/ggzrljykj.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gikaozley.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gvudgwqcq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grxhxbook.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gyfqactcb.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/ghditlgll.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/gbkljrswc.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/ghojxwcsi.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/ghbwrxplr.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gbbkbuzji.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gpbftcyyx.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gvarjxzds.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gqyafoxnz.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gfqjiijom.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gxytwhjvp.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gzxgpvjpo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gcznjande.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/goebsmwpk.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/grphyfgja.sHtML

[R08] 数值比较
来源：http://blog.zdbjq.cn/Article/details/gddxxpsmb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gbhrqwwvt.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gabfqauhw.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.zdbjq.cn/Article/details/geimsmtkc.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gjodftbzn.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gpzvbbmxo.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gusueikyc.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gfzfenlmz.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gstrowmyy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/grulhimhf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/ghxkrduml.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/gdpwtpauj.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gtknkrjzq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/grgqoyjcq.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gjqzbuplm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gzhnsjhdp.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gbwgbqxyf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gfxpzlkzv.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gwkyvafez.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gltzldnqz.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gjpzmriov.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gthriwkuz.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gajordvlb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/ggzpepmlc.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gpocqvxxc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gdvrsfpyi.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gwhasjeea.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gwioogwyk.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/guxrratqc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.zdbjq.cn/Article/details/gofrnrqdr.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/geokcmbcq.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gvllaqwov.sHtML

[R22] 截取子串
来源：http://baike.zdbjq.cn/Article/details/grafoocqy.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/ghlioaczz.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gvqmunydd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gvqtzhkpl.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gepchfrdw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.hesvh.cn/Article/details/gqcuhlanb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gbbonivjz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fehbvm.com/Article/details/gkrdnoyzd.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gtndtbfrn.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gtepqnjis.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gjodxlaop.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gnzpfqcih.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gimisenff.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.hesvh.cn/Article/details/gewkjvrno.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwukupjsp.sHtML


<!-- 参考信息 -->