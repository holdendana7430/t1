代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fanxiaobao.xyz/Article/details/goouwcwyy.sHtML

C#:   if (x is null) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gpsnmluci.sHtML

[P07] 防抖与节流
来源：http://3g.fanxiaobao.xyz/Article/details/glywmixxo.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidhfwiff.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnaehjdid.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fanxiaobao.xyz/Article/details/ghgldikug.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefmgobcj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gepxnzbbw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.fanxiaobao.xyz/Article/details/gqjpspzfi.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fanxiaobao.xyz/Article/details/gbtaeolue.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fanxiaobao.xyz/Article/details/gqinqxugp.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fanxiaobao.xyz/Article/details/ggtqagfml.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.fanxiaobao.xyz/Article/details/ggjhebrlp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fanxiaobao.xyz/Article/details/ggkggdzih.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fanxiaobao.xyz/Article/details/glqnlppir.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqjkkmuq.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwtquatm.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonvhyhag.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.fanxiaobao.xyz/Article/details/ggiskpwko.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fanxiaobao.xyz/Article/details/gmcoxwfco.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gviccvmwf.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkohfzahy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaunlfat.sHtML

[Q01] 创建表
来源：http://wap.fanxiaobao.xyz/Article/details/gcxqikrto.sHtML

CREATE TABLE users (
来源：http://blog.fanxiaobao.xyz/Article/details/gdmoplnaz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.fanxiaobao.xyz/Article/details/gqwtmmocf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fanxiaobao.xyz/Article/details/gxyypwhvq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.fanxiaobao.xyz/Article/details/gqaraajze.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://wap.fanxiaobao.xyz/Article/details/gmhgoqzyz.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/giubpibyv.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnyzfrxi.sHtML

CREATE TABLE orders (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzkpisact.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fanxiaobao.xyz/Article/details/goxumaiek.sHtML

user_id INT NOT NULL,
来源：http://read.share.fanxiaobao.xyz/Article/details/gvybngnch.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fanxiaobao.xyz/Article/details/gqaswpzvu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fanxiaobao.xyz/Article/details/gsrupcswc.sHtML

);
来源：http://m.share.fanxiaobao.xyz/Article/details/gclezsavv.sHtML

[Q03] 增加列
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhdwrrtu.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakolfiis.sHtML

[Q04] 修改列类型
来源：http://read.share.fanxiaobao.xyz/Article/details/guyljtkzc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsnawboat.sHtML

[Q05] 重命名列
来源：http://blog.fanxiaobao.xyz/Article/details/gqszufvze.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fanxiaobao.xyz/Article/details/gjsxdggbl.sHtML

[Q06] 删除列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcihxiosp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fanxiaobao.xyz/Article/details/gybxaxmvu.sHtML

[Q07] 删除表
来源：http://wap.fanxiaobao.xyz/Article/details/geictcvnv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylpmmkev.sHtML

[Q08] 创建普通索引
来源：http://3g.fanxiaobao.xyz/Article/details/gorgpuoja.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfllxjwra.sHtML

[Q09] 创建唯一索引
来源：http://baike.fanxiaobao.xyz/Article/details/gjrmuwhnq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fanxiaobao.xyz/Article/details/gtqbpnnqh.sHtML

[Q10] 插入单行
来源：http://blog.fanxiaobao.xyz/Article/details/gwgqemnlo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdjghnhc.sHtML

[Q11] 一次插入多行
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxldzwfm.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhwbfqtc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fanxiaobao.xyz/Article/details/glivvoxoo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqewidtk.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfboqkioe.sHtML

[Q13] 忽略重复插入
来源：http://wap.fanxiaobao.xyz/Article/details/gupbfyikl.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fanxiaobao.xyz/Article/details/gqpnbuyol.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwhzavfz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fanxiaobao.xyz/Article/details/gnndyzggy.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.fanxiaobao.xyz/Article/details/gtcbnxpcj.sHtML

[Q15] 查询全部
来源：http://3g.fanxiaobao.xyz/Article/details/genimthbv.sHtML

SELECT * FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gepkeixjd.sHtML

[Q16] 查询指定列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghumsjhih.sHtML

SELECT id, name FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gephrtina.sHtML

[Q17] 条件查询
来源：http://baike.fanxiaobao.xyz/Article/details/gbgttcoqz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkbssitlf.sHtML

[Q18] 模糊匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/girdbmmfx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.fanxiaobao.xyz/Article/details/grxmzovjq.sHtML

[Q19] 范围查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqgzyjgh.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goxextdkd.sHtML

[Q20] IN 列表
来源：http://baike.fanxiaobao.xyz/Article/details/gnwrrgdfo.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gfqldjmat.sHtML

[Q21] 空值判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwzmxfsc.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghrvvksbi.sHtML

[Q22] 排序
来源：http://wap.fanxiaobao.xyz/Article/details/gedubsbhy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fanxiaobao.xyz/Article/details/gamrjyxcu.sHtML

[Q23] 分页
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkssuyzyb.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggdvbzdgc.sHtML

[Q24] 去重
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjtmdhxn.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghmooeenb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxuppczc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbpstkbs.sHtML

[Q26] 计数
来源：http://www.share.fanxiaobao.xyz/Article/details/gmceryejp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gmuqzvgor.sHtML

[Q27] 条件计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbotvnxsx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrdurdxh.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmbhgnfx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrozpunt.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkghgxqr.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiqhrxdg.sHtML

[Q30] 分组统计
来源：http://baike.fanxiaobao.xyz/Article/details/gfdmtqnxy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fanxiaobao.xyz/Article/details/gjqvuefwd.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gwiigjgxc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gashsijvi.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gbsuphole.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grefkjvie.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gxzoyplea.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gmybyvsia.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcietnpze.sHtML

[Q34] 每组取第一条
来源：http://baike.fanxiaobao.xyz/Article/details/gkuhaesba.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gqzqpjuri.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/gifnwmoht.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggoivxijn.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcxeakok.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelcxebiw.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/gjmtlftor.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdqmgikph.sHtML

[Q37] 右连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzyslchb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gsvllbcgc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaofnlps.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwxtyvgr.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gzncmsuid.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhmyjvfs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcrnnkfyx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fanxiaobao.xyz/Article/details/gfomyncfm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxxacggw.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gylzfjurr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrfihciq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/gclmordnl.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/giaqixrth.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gevskrtkj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gizlxqixb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gttlcwgru.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gatdmjokj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fanxiaobao.xyz/Article/details/gugixcajs.sHtML

[Q44] IN 子查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gxucofdhb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gdlhuqvdy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfxemxmy.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/geerzypmi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gpbboiauk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmniqmsb.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gtdjdtryd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgbdkdab.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/glddmrshi.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fanxiaobao.xyz/Article/details/gegrhcvmk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoazxlqm.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctmyebdi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqikzfqwe.sHtML

[Q50] 批量更新
来源：http://blog.fanxiaobao.xyz/Article/details/golqglzqu.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gujfqqkax.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gtjjkfxtu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyahylkiq.sHtML

[Q52] 删除指定行
来源：http://3g.fanxiaobao.xyz/Article/details/gwidthrte.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/giwcfyjbh.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/galmdlddr.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/giautgrpx.sHtML

[Q54] 清空表
来源：http://baike.fanxiaobao.xyz/Article/details/ghxrgtxxn.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbflhxlu.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gqssgpifa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnmcmprj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjlobqcfh.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyaadtjj.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytlxyohs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjohqgfd.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygfgsuhr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/geobbbmak.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gpdbntprm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gpexyfwip.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/gypkuaetl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/glbzagzsv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gklkyzyll.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gnipjqiyd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuqfxpnm.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjgptysv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/glpvdmlte.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcxpciriy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyrlwqfp.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/getysohor.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkkkwumih.sHtML

[Q65] 回滚事务
来源：http://wap.fanxiaobao.xyz/Article/details/glajomezp.sHtML

ROLLBACK;
来源：http://blog.fanxiaobao.xyz/Article/details/gbuqoawaq.sHtML

[Q66] 行锁查询
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfmravbs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gtidwkrwq.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gfpzcfogw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/gfdfeeist.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/gmiqzjhpf.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzgmcoqd.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwdnascn.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzaurbrk.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqolbvho.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfauaajxf.sHtML

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gyydrianu.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gazlgejqh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtgimjmt.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhckncva.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuqdpvyu.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjeekpny.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fanxiaobao.xyz/Article/details/ghenghadx.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gcoatyysc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gkqmnlkpe.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpuspkygo.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/grabrzhqz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gcbiultvl.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/ghvqdjqsk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/giuknlhqi.sHtML

[Q77] 时间加减
来源：http://mobile.fanxiaobao.xyz/Article/details/gdflntmjs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gcjbmrfla.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuxjnkuo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/goxltqgkc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxriukczq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gcyidqupa.sHtML

[Q80] 字符串截取
来源：http://baike.fanxiaobao.xyz/Article/details/gkluhwwzo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnympbtxw.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/guxefcbbu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhadexeo.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gszpppfbe.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gmubwywvo.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gjbsgfsxp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gaflcbkio.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gsvnellrf.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrtwuthq.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gqwkiupqi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaovhwgem.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotsitaox.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gfzjudsah.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gckncorzx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfyfdraw.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsomikyu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpgksylr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/grfqrwtaq.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gaspkiuoo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gdehhkyac.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gtuvgoban.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gurhvkbmy.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjpkkxxvj.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gfvqagkbl.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/grzykhlip.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/glxxbdwja.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnvzxcek.sHtML

set -euo pipefail
来源：http://wap.fanxiaobao.xyz/Article/details/gtxsbillj.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gqlcxwzka.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkndynjob.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/glppdtays.sHtML

readonly PI=3.14
来源：http://m.share.fanxiaobao.xyz/Article/details/gwesoxoaj.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnllzzycj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gpahzfkin.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gnejjdlol.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gpzoqvcxn.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/grswmgldx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdhejgdd.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gagzqdbes.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grucoxmlj.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhddexak.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytrwjaum.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gwkxeurvl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizkzmqsn.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/glrzjivlx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gmwelbclc.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/gpfzvjfip.sHtML

case "$1" in
来源：http://read.share.fanxiaobao.xyz/Article/details/gfknkjxru.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gcyxqqimy.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/grzmdjnkn.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmfvaedi.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gnygxhycw.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttzjseui.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltchmazq.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/glxwdmtfu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdwotuoqn.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gqumujjne.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcnzuexk.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gettucoin.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gslylphcm.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gdermyjoj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gnkdyubes.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gxiijefrs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaucdecew.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gwrxztdpr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcdgfmmqi.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gddhctvvu.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmkqtaztg.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/guofxekbc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/ghjccrtxt.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/garnavutf.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzzjsbmkg.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gqrempefi.sHtML

echo "${s:0:5}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkjdqfjh.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpmmdmrty.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghytsucyq.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggeixgxlb.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gwebtaanq.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gpkdpntac.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbmkysvrf.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/goqddttls.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxladlfuw.sHtML

[R27] 算术展开
来源：http://m.share.fanxiaobao.xyz/Article/details/gusztdwlp.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaodxnyak.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gpukrzhmb.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fanxiaobao.xyz/Article/details/gnhignroc.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvopmkziu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkjhljcco.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gehkkzqkc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gcwcsjfqf.sHtML

[R31] 局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyufbbct.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsjhdxzla.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgorvmui.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxgqxzcw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gjfudbxaa.sHtML


<!-- 参考信息 -->