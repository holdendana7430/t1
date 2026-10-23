代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3szadhrkp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3xcxrkmfs.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3wiootsdx.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eywmoueo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kqoyqxlp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3evcryvap.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iuzqqjkz.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrrbrkfx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3rmpzvdar.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elrcdvwb.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dqthpblv.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mcqwsnld.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qzsuhcxz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rspilmbc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3gqaxinhi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sclhmmro.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3ylpqqgid.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3gloznjru.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3sncepcuh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3kkzyecmr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3hzqfotms.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3vrhhaizz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3dbzdauim.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzwxvukc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3adylcsdg.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ozzylfmi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3hziklkqp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3usmvigbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bbsweeqw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3coqjjkuw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kpmgdqyt.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xhesknah.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3hjdbssjy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xkzkkqcl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3wkxoabeb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3wjvkdlfu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3xwbxxkjn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3inqkiwzb.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3rexxowsg.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3jmmqhefe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ijaxrqeb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rbbdyxvc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tskxjirs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wbzbrwzw.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3teoayoty.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zbrepkcm.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3mbngprko.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3qsnqaqng.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dlcqhmjg.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rrwjukus.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3pmpdasmo.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3iaiouewk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3tgbqbevc.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wxxqzlzy.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3umegpcby.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3knaudcpy.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3kjwcjiff.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gvyrbslm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3gmgkgqly.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3phkrscns.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3awhinhiw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3voeznsjv.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3wrucrpbf.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xiaqzjfp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qrldwcqm.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3atokzhra.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3akufblgc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3jfvpnxzq.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3qeyrtqbi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mmaujgil.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mbqvlqvd.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3uaoimqeu.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iqjyrlbp.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3vfmmzwsb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3boeyzikk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3gdvcieci.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cwtofrfg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3doebsdiz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3rsbbahww.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xuwsoqqa.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ukgxcrjz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3xcgmrxcr.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3ngfixfxa.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zpynubrd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yxgojfcy.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gomjpqya.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xznxvzax.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3huerdbji.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3dumczjfu.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3bthitmfi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrsqylcy.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3zjvfmnxk.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3eohdzkaq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cxkyhegw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iqkakneo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3vrzfvmff.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ulhmiiyb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3heghiset.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oidmivep.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ofutfyiv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jopttuqm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3mnvcrhvv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tjvhhzue.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3pknmhxth.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rbcugvpi.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3eyuseuvh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bycreugp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3gjihtzhb.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3ysyqayqr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yzqkdcyu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kleoseag.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3zojmgeiy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3triwwjor.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gqoixwgd.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ywltmref.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3cjnbftbo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gqrfjtfr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3trmjxikh.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3hqqbwlfp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gbxrfdqw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3azzmvzed.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3pblfhilp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3krxurigs.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3fvocepah.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3mbaibuks.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3nlgtudxs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ddoprpjx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3iidttgup.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3eynwfapx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3iwjvuvgh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zsqviljp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nzehwagt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mjtjnfxp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rhdxfkvs.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nscxbeha.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3sotynznc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3opxofitc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3jazwohvp.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3xlgqjgwr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ahwppbbu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3iyohwkrt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ppyibnvx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3hhhmwmkb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3lahqvhkg.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3suadfnuk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3eowrpizd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3bfxeicqm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hdhtbprk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3mhbdowbr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zazpioyp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cfmfyufn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mnocffsw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3ytnbiked.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ieoxknpr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bmnhubon.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3exzpfrie.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cspryqlb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3mqzuzrox.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ddscrarx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hnvfokdt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3imkhcsqa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3tmpydyvo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pdkzglkh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pilmpctz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hbxqbnte.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wtzeamhh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hvzevqwf.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lpdladbp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3umorrfeb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3zlzetplx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3slbqpfto.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3awxdtady.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3yflqtehg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3eyggyiwt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3odamgusw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3epthgyxb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3nntkhiur.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uvgfolmf.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rolwmdhi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3aodkshkk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ocilrtuw.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3yzaaskmc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3himnahml.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3uadhbrtn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3hbfwfudj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3pwpktttc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3qbmimjeb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mkjrhwfy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kcbqivxt.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3rlduvgzw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3nzczsymw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3aokqursp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3klebusyw.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gvoolxeg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sfecnejy.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zrdyeuao.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ghlnstkq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lqtdnlri.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3uacguphj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3swbbhdei.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3jpnzbfrf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kwkyvecp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ldeznfjn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3fsixvgvq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3blcswmwu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3goixvloa.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3iirnpjeo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ctggkilb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gabzugvw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wzkidpxl.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jmhjykmm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3oqgqwkyl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zbvkotel.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3owgiwupx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3dwerreio.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vdmnszdw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3zokpxdqc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qjfjworn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mnemdpej.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msgoixox.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3zkpyqqqu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xiwioqyb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3owiyddsw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3untpzxeh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3tpxazksk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3asjqmxxg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hnbwjzbj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tokzodtj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ziunjnzk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3gtbsbcyt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhfzgppo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3whjbpluy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zaylqtka.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ikhxrueb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3myedxnij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yejenipr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pphocozr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lczoklgu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mpszfbdz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3oqcriedu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3gtsqznlr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3phpalgax.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3atpjrnrr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mcvcggyb.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ficsgoam.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hfvljpeq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rqpeumwa.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pbqeenxf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3kmvthfac.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hqqyznft.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3juuxqxcn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ioknriqp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xqrfkvar.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3htpemmgv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bcpogqjw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3kmspdbqq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3nnkrmbip.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mlypevuq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nkivyktt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3keioydam.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3omglulco.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ndvsufxe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qoowqarb.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kneradbd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xzjcmhsd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3qidwcfvt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3psffqrbq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3phqnuzym.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nzeceqbf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3miubwgvq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hygypojv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3faleltqz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3oahvcxdd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fzioiowm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wzrlhzye.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3uaxbapso.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kzpsfzal.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3uujbsjtq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iwlvcnif.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hiyxqllu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ojsbmfgt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3croqkncj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pydnehea.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3idwjcbsx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3osxldqnw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lncjyhhc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3uzqlvskw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bkxuapsr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mfiwmnka.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fwetrlll.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3xdfrbqyo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3irgdgtmt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nmggczpz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3gkkoyhgj.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ynkzkmun.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3griyakci.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3kpalqdgk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3cjpndgrb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3kcvbczmk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3qrtcdami.html


<!-- 参考信息 -->