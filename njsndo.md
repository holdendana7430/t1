代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3wsjetlxo.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3njtpswps.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ppgxefhq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fyxqzjlj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3juqofkgg.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prufbfpk.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fnelxhfv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3wjtvrjhj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3nthqasmy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3pjyvnpxq.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3hmajgrcc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3ixradaou.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3wzkifwxs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gxfmmtkm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3auctumoo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jkvlmcfp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3fnymzqoz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3joothlrk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3hxrawpsl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3xgunupgf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3kqspthms.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3knxmilsj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3yawtbdvv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3rgxrblcr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xrkihfof.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3llueudta.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ekterijn.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3soyrngul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yfkxksrb.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ejykwmfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ozlwnxiz.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gwswmjrb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3nhromyem.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ulomxgwi.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nlnfbaka.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3whonwtpv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3lrphijzz.html

);
来源：http://www.52xcode.cn/Article/details/gt3nopmugfx.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3clephwoc.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3rrnpazmf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ligvhmvy.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xjqtivjq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3iplcggcw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ikakgsmg.html

);
来源：http://www.52xcode.cn/Article/details/gt3ebyzpdak.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kssbwvuv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ihbvortu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3epccmjke.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tjtmemjy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3mxjynnnw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3kpeitfvs.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3emvaqvbb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3pvzotypy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3hdbxohnd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3wzxzengf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3sqvutcms.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jjzdebwq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3vkepkdbg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3vwwankum.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3jskuwrwt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3kksoxtyc.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3qewvmgpq.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dzsbzhyi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xppfdbyy.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nnrygwwj.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3pvxsmjmm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3rgqdzbab.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3syqsrrck.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3nnnyatfy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3hltvvskk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ilspxsdj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rbctywra.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sbjwyzob.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3aycbiewt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gyzefdcp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ptigutxq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zteuhdmh.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gqhvadrv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3utvcpwjl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yhveuqjt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3oiqpgyxw.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3elvibtri.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hccmugtp.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tuvicfpi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3fbzucbat.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3djvdhfst.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3ewbfktgo.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3txtdoqsq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ltanyerv.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3oxjfnwsz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwvlkmbo.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3rzmbavdp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hcquggdt.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3hgtdalzi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ccbvscem.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3zmktgwts.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gjmccngi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3lkxbdiei.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dusfltwh.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xbjlzygv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3knzpacmw.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3djkvlkjs.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zfjxjmeo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wtmypakx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3pemameuz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cxlsdoah.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3efixqygi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zwiyoazo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fxoctgdq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3fkekbxto.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3qtryktvk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3tkwjfoxl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3mhxmkhja.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pwykcisx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3dsbimchp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fxtlwpfj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gybdnrer.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3koryhdez.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3cmzfbzxz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3uwghjdjb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dlyccjvb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sewjmoot.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3aijjrrfb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qdbslgux.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3admgdxen.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3amjsluhb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3gxwbtxjl.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vhryhwke.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3glmzaljq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3koelfdzp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3iybzmoco.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xganxnek.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3davrysdc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ynogqypo.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uzugeynj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3sdgqffaw.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vnlbzjpk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ypqpcxqe.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3seezndvd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ddqujzly.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mrarhkfz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iairqbgr.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ryjguutm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3cbypcioi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gdmrajqk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vacdujow.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jqnuzfyx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3zalrfvbq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vuvscyno.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3trbqmdus.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3wsuqagfk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3xgruajtj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ettpofic.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3xvxbmtdp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kvwoyggl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ibkekgbw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3oulhvkvd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hrabayof.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xibbqkpm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3szplsfey.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mzrguday.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tbyqvpwf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3modllntz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pzpauyez.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3egaaxvei.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3rslctqdc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rpsgoxtk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3juiuqkwx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xesbaimp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ktqtgvnk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nwlqornj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jyorxjhs.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3zgycwwhw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bkxrsfce.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mrgzuvco.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3banzbycn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3wmxzhsti.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ewasujnn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3msiavtho.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3rkrixwnn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3uzlxkmsa.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tbonykbs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3idacvsoj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jplgmskj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3vzujcsde.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3jznxtepm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3wuxvtpxo.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3emusocnw.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3oavsdcsr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ppojoosb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3punrkvdt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3fwaxipxz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rruwqzrh.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ywwypots.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3kzklasnm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3qnpdcpru.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gwcstinp.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rlzyzjrx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jswbhthw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xktupmxm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pimioupp.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3iczbvdza.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3inbpbkyy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3cdekxetr.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vxmyenvb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3disdqwpy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3qsyvfvwi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3autijfdc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3whpitajr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3dblbqlhm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lidtovir.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3pamicama.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3acwmcpft.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vpgaulyp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3mvaoymck.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3npyrfhit.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3zpdwmkre.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mdzqkxsp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3scpnkvun.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3imacbjob.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3sehkdrwc.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dymdapgc.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rxisyxaj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3uyqrbkiz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3svaxjqdx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3favzupke.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3lqknnnzn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fqyfjgka.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3qetoltbs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wlovimlo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdraulzi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xhotqlqx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3ewzyupwo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3gerjexfn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rvyfxmcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izdnccyt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zrpksowd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kzbjbwdo.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vhfgarqh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3mdieswql.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wptemucx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cneeicyb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3rhgernhf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hhekbcvh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3uecdzfid.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3qoflaveu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gifhhxut.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mqjvdkbq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3aktimslr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jpkfugqm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ywxkzfrv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3hmepslzz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3swlrzsjw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ovjwjfdt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3nzoxtweb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3jiatjiiy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jarpmblz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wjrsiqxx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3psnuhxkv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ulwdtzxs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3tbcirmdn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3qignmosp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vpwmwtvf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uekwkxmb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ybxkjxic.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxqahcsn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqhbkqmm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3aknbvuxl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mwoldpra.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bzzzgkrr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gknsbcxi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xgcrykbg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nuipvxwh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dslaspaq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mtywocda.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vapwmdyf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgrjwybv.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pyoxaeox.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3gwwlskww.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fvninvkw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ghpbrhxy.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3abcvarlq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rkxqdwrg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dyfryoec.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xdezgpbl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fpdsljbt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rwkvsdjr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3dubyzokt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3xcvxcbcw.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zcahbuia.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hxxeyape.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3lgnumhfo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3gedflvhc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3lmutrdwk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3usufwbrp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jgtmxtch.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3uimcdldb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3esdwhnbs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3byfpihnq.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3knyqpwaj.html


<!-- 参考信息 -->