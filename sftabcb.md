代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gxzodreby.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/gwfhijkti.sHtML

[P07] 防抖与节流
来源：http://baike.hesvh.cn/Article/details/gythrutfe.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.zdbjq.cn/Article/details/gepgkpfyg.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/godswlanb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gmgjwaldy.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gqbujpkvh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.zdbjq.cn/Article/details/gcoctzdaw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.fehbvm.com/Article/details/gyfrxkzfj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.fehbvm.com/Article/details/gkgurfhlu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.zdbjq.cn/Article/details/gajrxakcl.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/ganlundvo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gbmtobgma.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.fehbvm.com/Article/details/gvxcwhfyp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/getcbjqcu.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gspatouph.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.m.share.hesvh.cn/Article/details/gerlyuoui.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gokqlnobd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.fehbvm.com/Article/details/gidahhnhf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/gtkjvxhax.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gnkukwcwr.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gnechazru.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gcwfvqcae.sHtML

[Q01] 创建表
来源：http://baike.hesvh.cn/Article/details/gspcdijjo.sHtML

CREATE TABLE users (
来源：http://www.m.share.hesvh.cn/Article/details/gjlxnotqs.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.zdbjq.cn/Article/details/gywlzblxh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gcrbfejgf.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.hesvh.cn/Article/details/gbluetonp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/gvxseyjvw.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gyekytdzf.sHtML

[Q02] 创建带外键的表
来源：http://mobile.hesvh.cn/Article/details/giizqejwd.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gqnfenfbx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gwfmjyjlw.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gcbxqopnk.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gqjfipdlx.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/ggfocatsj.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gqemhmyzk.sHtML

[Q03] 增加列
来源：http://www.blog.fehbvm.com/Article/details/ggbldgmal.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gwgkmfwtk.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gtspxbgou.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gqyeriqpb.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/guvkqwvhi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gqnfrwtsl.sHtML

[Q06] 删除列
来源：http://3g.zdbjq.cn/Article/details/ggncbntig.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/grphesphu.sHtML

[Q07] 删除表
来源：http://blog.zdbjq.cn/Article/details/gbmgviyqp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.fehbvm.com/Article/details/gettkycfh.sHtML

[Q08] 创建普通索引
来源：http://www.share.hesvh.cn/Article/details/gvxhcrftk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/ghqnidhgq.sHtML

[Q09] 创建唯一索引
来源：http://mobile.fehbvm.com/Article/details/gmseglhrd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gnijekikb.sHtML

[Q10] 插入单行
来源：http://3g.fehbvm.com/Article/details/gfkznmijo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gdefcrknt.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gxxlffnsj.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.zdbjq.cn/Article/details/geedbwtob.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.fehbvm.com/Article/details/gogvhnktj.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.zdbjq.cn/Article/details/guocuruha.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gewhtlpfy.sHtML

[Q13] 忽略重复插入
来源：http://mobile.fehbvm.com/Article/details/gnnzlumlf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gnhixvqpu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gdyulzckd.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gphindmpv.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.share.fehbvm.com/Article/details/gooqjwrcv.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gmfucbtas.sHtML

SELECT * FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gebulgtdl.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gnibrdmpq.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gnzmvkuvf.sHtML

[Q17] 条件查询
来源：http://www.share.zdbjq.cn/Article/details/gpyboaoko.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/goezhvwmx.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/ghddmoufe.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.hesvh.cn/Article/details/gzgxlcqtf.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gqbojdzmp.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://baike.zdbjq.cn/Article/details/giyugohyj.sHtML

[Q20] IN 列表
来源：http://wap.zdbjq.cn/Article/details/guahznnrn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gckqevehd.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gigtqtfvf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gbsixbfeq.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gkvdgrywg.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/glcvqyksi.sHtML

[Q23] 分页
来源：http://www.m.share.hesvh.cn/Article/details/gksrbduon.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gywknfkrw.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gfdqfecab.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyztvrubs.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gdnbfcrfb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/glubszuws.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/girxprjet.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/guvefcfka.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/ghqcnmyee.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghswfpucd.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gyfxymudw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gebzrkoge.sHtML

[Q29] 最大最小值
来源：http://3g.fehbvm.com/Article/details/gickelqlk.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gqqzeusmd.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gqmdhfkpi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gwjlgitdq.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gtccgtqbt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gtlouqyng.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gcchcfkrl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gdkczzoel.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/giqijasbt.sHtML

[Q33] 多列分组
来源：http://m.share.zdbjq.cn/Article/details/gryzjyqsn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gqdyqwwbt.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gupmembbx.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gblixiytr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gfgdnqhfe.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gaavmnpep.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/glwoeaqdh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gadkbrbqg.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gjdlfgfij.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gtujczlmw.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/giyepvexe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gxtkauiko.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fehbvm.com/Article/details/gwfhxvuxe.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gjwgbetwq.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gamygjbkp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fehbvm.com/Article/details/gwoclurog.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gcdigeksa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gdkenbaia.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.zdbjq.cn/Article/details/gfzagminz.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gtttoyyoo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gjfngahdf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gwgfjpkjm.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gcatnnkug.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gstonogha.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gatwbgrrz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gqpmmtrqz.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gggjmqohh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/gugsgqniu.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gcbgbnfqo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gqdsrrywp.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gmswuybut.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gohzyahqh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gequrbzfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/glrjonyrj.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gkvbcogos.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gjvxfwqap.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gmbrqmwhb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gknqddzju.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gcdjvankl.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/gnmqdnstg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gcisgdbuh.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gxfxlnzdx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/geeaexbbs.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gaiaidcgo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/ggngowrhh.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gvrnhkmtv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gtgrzviqv.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/gijfyjzwy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/grpocyflz.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gvbfyywlk.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gonyzsknt.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/ghsnufmxo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fehbvm.com/Article/details/gyjhqscyt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gvxacobjq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/ggxujqrcm.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gqsbzduuz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/ghelhttyd.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gfrmfaovn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkpxzgxdm.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gcnbaukpm.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gjlafteda.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gxmgmeqou.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gaposhxds.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpgzcrpsh.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gyillhthm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghsjthpaf.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gkansuvrx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/grpjzvboz.sHtML

[Q63] 开启事务
来源：http://www.m.share.zdbjq.cn/Article/details/gajxvcieu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gvieafeve.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gfbpqydqq.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gcharfnyb.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gimerqxrx.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gjtasdkcx.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gcvzsxkph.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gastignnk.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gbzwrmwmj.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gwvvimnkt.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gxmerhwsr.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gcmonoshk.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/grgzrvtzr.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gwluwgngf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/gvclvmzbq.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gnsutmeap.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gaeohkkbg.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gyytyjogz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gomeqzqsb.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gabwapchq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcayafgcj.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gnvckbyoa.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/guxtsvphn.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gfymdywef.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gwfflncdl.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/golblbnue.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gezlythww.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gkjgzvytd.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/glyeannbg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/giyiantub.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gzjukivhf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gncsmyanf.sHtML

[Q78] 当前时间
来源：http://read.share.hesvh.cn/Article/details/gsaallqmz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.hesvh.cn/Article/details/gppbethgv.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/gmvzwkgyg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gucqjwhhy.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gypwnkbrc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gzwojxqhi.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/ggdloyfjt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfcvfluuq.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/galixikxq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/glxeykekc.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gvkzqjogs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gfdgkfvka.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gbgxbwiux.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grsuthgsh.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/gwrqxgenw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gfphavoww.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/ggakhnvpf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gewowjxvg.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gpxlmqnlo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gxckxeutj.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gjiuzmrss.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gqczxdsoy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gejgrqosr.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gegkhmcvk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/gvvnqrqih.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/ggknwhfhz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/ggppnpopt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glgvvuhqf.sHtML

R. Bash 专题
来源：http://wap.hesvh.cn/Article/details/gshaemkye.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/godjknmgr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gmoarvurz.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/gkvbzmjfs.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gqicgyiyl.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gfxvgphtx.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/guzixvucj.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/ggzboamej.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gmvirsuud.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gnddqhjsj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gwohuowfv.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gmapyejok.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gbvkepteo.sHtML

[R06] 判断命令是否存在
来源：http://blog.hesvh.cn/Article/details/gpxvwchiw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/ggkkngegc.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gexwtxiii.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gukymebef.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gcftqxlmg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gvsryvtmi.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gkwqccajm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gboicfrer.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/garlhyaod.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gwtlwkiws.sHtML

[R11] case 多分支
来源：http://read.share.zdbjq.cn/Article/details/gklhpzxkn.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/guwjytetl.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gxkzojary.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gyloekeuw.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/gvqdqsqxn.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gysqqcndc.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/goevdcvum.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/govqdkndx.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/goevfuggl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gtzqmkdhz.sHtML

[R14] C 风格 for
来源：http://3g.fehbvm.com/Article/details/gjcroyzze.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gcfgdhpmv.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gwgrmokgd.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gpybumhxs.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gsgekkbou.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gasrzhjzu.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gdxyoosff.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.hesvh.cn/Article/details/gpcaiklbj.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gvcdmmlpx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/ghhopwfie.sHtML

[R19] 数组长度
来源：http://blog.zdbjq.cn/Article/details/guhnrfzcd.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gsamqohen.sHtML

[R20] 关联数组（字典）
来源：http://wap.fehbvm.com/Article/details/gxulxpzkp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gqhrmjacd.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gayllascc.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gjgfecuxv.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gmrpabuyr.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gxzypemzb.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gxkgtmyhe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gceqkvmgh.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gfkbbzaui.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/geyokfltl.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gydobxuqc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/groymknfs.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gmqgbdxyz.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gtapbqyho.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gpuvvqenp.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gdfrcmitv.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gsidxmmfj.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/geqmfuvej.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gnptavsee.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gsshdhgep.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gqblqkytx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gryfghkow.sHtML

[R31] 局部变量
来源：http://3g.fehbvm.com/Article/details/gktcmmnlu.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gcdmjxrhc.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gnklycxbh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gwgghwdcm.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.hesvh.cn/Article/details/gtkzejguq.sHtML


<!-- 参考信息 -->