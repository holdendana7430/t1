代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3mjtijowe.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qutjbvhe.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3cbiqsuta.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3igagzyvt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kdmlpjli.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ofshwdqs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hlsdvojb.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3pjcssyzi.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3qqnuwxzd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qacpafeu.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qimsqkkk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jjocwvey.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xmbcusld.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rcztuqkr.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3tqkcisno.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3wedfzqwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xchonyze.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lbvygprn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhawhtzr.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3glxeqaoi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3vwpfmkuk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bovmmfum.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dmvkfxso.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3jomdbyji.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3lqrtuegv.html

);
来源：http://www.52xcode.cn/Article/details/gt3itqwsfua.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3ymjxulwq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3ybwitlrz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3bpxuwasb.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ajtfmllk.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3imgcgqcg.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3wiehjlfm.html

);
来源：http://www.52xcode.cn/Article/details/gt3qfrursib.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3yqaynkte.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3itoevybw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3yodazedh.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3wqlydcxw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3sofdcxmf.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3aundcjrc.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3xkoywaou.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ifikbyju.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xdmufmcq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uxkmcllj.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3opeoaifq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3qojvanab.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ouuasrpb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rbmbenvj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3eeyomyih.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3gutfrjcu.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ejfjquyg.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3priljtcb.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3pftnkfme.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3cxftzbkr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vsndprpx.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3viuqraxo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hlrjtmef.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3sygxdrky.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mdhdalni.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ilvvpsgf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3sqqslufu.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sylznvqe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3xwtwmglp.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wvxppdks.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dnnzolqc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kclumpjv.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3bufwlzzc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3awlkliyh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3avdudjhd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3qoodbfst.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3drjipndj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3awwrvrta.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ukwmigqy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3lmiegodx.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3iobkggoc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3jyaqrvqu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3jomifoff.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ymkfpicn.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3mdwdqmlt.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3chcbyiuc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3eunfynfr.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dytxvypj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3yzdlmuvj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vymqwuhf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3jyuffadr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrwwjpax.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3fhcnpyro.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tvxlksfb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3jwzxkkoa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3geojlsfm.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3xnrchdyu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pemkniow.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hizmwkaw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mrpnrybb.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xwypnsdg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wmclxsvl.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3zzrftqcm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3yfqmlnsb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ailvacez.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3kicjefyn.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3uterzrao.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3kxjjowjr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3frhpmhgv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3lkropbwb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lrvladng.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3vyyenpad.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3oyxpffmq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3adkdacrj.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mqddpbvr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rkufirsl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bxhaydly.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dmdnojal.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3dkufkvtz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gjsqkjgf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3iklyjkmx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tjxnictf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3dxagcaoj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bmvhpcuy.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3tzillsou.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ibwviies.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3xkfcxfrl.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3twllpagx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3khmpfpnj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3vgxryser.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3skjlaanc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vismsgqq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ihjjnxdo.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qtnejzdf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qsxxxwey.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3rjvtqotm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vwpgxvgt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nzoyoglo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3gbucpbld.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3cgrphbtw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3cxkczmmz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mxjodnzp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lrvoimfg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3bcotqlaq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ftjvrgts.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pqomfipn.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3fasxiyvd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3eejjpjpj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qpapnvau.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3emjnntzc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3pykmbqvl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sgifxtux.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3eziuhyrx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3grpbelgn.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wxexefbx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3oyxksgbv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ognenknl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sbrotzrx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3jfbhxrrd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rkxulhen.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ktoromju.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yxxvsvzj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3aepkxxbn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pkwamjce.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fjbxbqfr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3txlqvwpt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xagcejfp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3iapypuwp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wqhgbflv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mspdpoli.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ygeodiux.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xpsbkmlg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jwvgikrs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3hlnvzasw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3qqxtecww.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3spoosnnu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3uwporgwl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tkgkjrcc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3aosrmyhf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gswrcbbj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wsnjucjv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3admsxlno.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3spggatlm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wlmydbkd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3smkdspmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3chflpxcb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3gulsqytz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dxxipzhg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3awhvcxbp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wywduerc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dxtrpytp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lzecpsyq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3idnjejco.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3psjsivgs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3gthddlbb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3zthgychj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pyzaskjo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3remlfwqf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3kyjpmanm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3viirdnyq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xeshvjse.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xcmhikaw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3pzkjbcya.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vnmpuack.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cfzgpslg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bsaokwyu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3fgphzkyz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3sxqknrpu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gavtgick.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zlxojmlr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qlpwxrpi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3byzugzvk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cyliuauo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3yzerxtyw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qkbxwmab.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qwbelrlh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kncuzpjo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ztyfujli.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3apqikulp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jnyyrlbz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3pkeyzmnq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3klifaymd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3tdbportt.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3jybabypi.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3leqcatfa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yhkjqkqd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3neyhitby.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3eislpceg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3mliealpn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3aaqiobkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gityflov.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3nshcyhll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbhiught.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hlhtjfbv.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3hvygfkiy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3vziukrxp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ureljkdd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3wzwwnxnx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qpaojzsp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3vefqnbyv.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3uuthqzvq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3nfcbcwjo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3pwdxkvpv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cawfouzb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pqkdqnje.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zsbbknhx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3uehrnejt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rmnkhrcq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tlnchxdu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yigkrcss.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gtsokxma.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lookmksw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ygvuejvm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eyoogviw.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3lnemhrhy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3erlqhtxc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3euecmnng.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3nkqqwmdd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ffpuspsj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gjbptjgd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jvdrblyf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kggxjmva.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lnwjexbs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uegabmfr.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ygdnkfqb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fjeizmwr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zfrzqvjx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cxkvhnxq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3lxkmcbrv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xpsxxitw.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gcntwmxc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3igqvcjpb.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3zcsjkzpb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dutwstjg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3drqyxsur.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3zhrflxci.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3wyjkgyyk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3gcbedrgp.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rrmujmkb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ohykiygh.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mivpsupy.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zfzyywwz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bsywsgbh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wfkrfgqa.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3readohkz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hpfxdzbt.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ukjeairm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3syhqcqdp.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mftdozld.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jzxyhbne.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rtqyerda.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ywllnyfd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iwlchqkr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3eskukhhh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3nlfzjnlb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3zgkrswny.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ysptiqce.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3umooirys.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3odfdikbb.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3mgbidamq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mqjdnciu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfdtdfjs.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3odvqzlmn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3tekqonjn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3omctswyw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3diinxlyz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mqxchoec.html


<!-- 参考信息 -->