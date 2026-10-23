代发 wailian999

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3vcksvjts.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3gwgyymnb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3nnzrdshb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qegkglou.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3yoapefzd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ogbvyxtk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3knwlyhqd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3ofpdvzvl.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3pvcrdztx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3gzsqllnx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3hoqdfzit.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3dqsxfsgg.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3owugtuun.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ullvxzhk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wsrcmqmb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oqdkhjdr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3mlygiwgv.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3sxpnzzhs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3suxlwzck.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gdjnlpsx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfbtwvwd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3yhndxznb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snjvvrra.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3slgtifxw.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3myvdwalo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3prbqgads.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kgybpekq.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vviukkql.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3swqxazmy.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3aszlrnaa.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3yjzozuqv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3kyxpkwdz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xdtrksgg.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xxwcbpia.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3awhqoper.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mepyiioa.html

);
来源：http://www.52xcode.cn/Article/details/gt3etenppin.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3zrgetlph.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3zklauphy.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3frpyytei.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3boxnocee.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3opnrahca.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lglyojat.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3nquszikz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ahliasmk.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3xykrpqpc.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gaseueyo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3ogehysiz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3xazscegx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3iyizqdlh.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ybfcodmm.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3njjynkit.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3swqsmyyd.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3harirhia.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3slijdicz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ldrysbxu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3dtkjyfwu.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3vgaogphm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3oqqgakjr.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3gxadmcpc.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3hsvxppmo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3cqgeauon.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3rdaljjct.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ksnboskd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3clmmqsga.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3miupdfok.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qitgytek.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3dmkuvnvs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ipxcxgei.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3nmwodgxx.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nxdlxrnb.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3bcerepjo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3bjglyqph.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3tzspwhbs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cdtfzndb.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3medlqxbi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3nndncqto.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3gutdaxop.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3zmkfrgkc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3pmhzhqjy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3cxqvvcnc.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3exqdcdzs.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xomhzjay.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3qgsriubf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3cldkfqni.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3xbrmglff.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oorqxanv.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ruwhhqgf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pgqvmmzz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3qvrrekmx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bplasjbv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3xlcxumfg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3acoonpog.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qvhnrphr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3cccflfyi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bpgfuucw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zuksghmw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3zhxpegqv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ezeffiat.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cybpjpcd.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3tnfbdqqe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3rbohzobb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3mluxslmg.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3liikzplw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3liesssnu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3wmeirqmw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3oaclxgqd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rfdmeneo.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3mvrtsyyn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3swrkgnwu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3amahwcqz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3frcyuqwh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3vgemzndo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3khpreicv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nbdrhnvn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pcyhlgbv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3epkdlhfy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3jgbtgadx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3cwewsnff.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3yhkbevdk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3tcjvuwzj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ofaduqdr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lomssklc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3eiskdkce.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gthfxmlz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3xkkebpou.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qpqravbd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3pmvfzxff.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ntsbtnpe.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3aseldfjq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ibaflbwh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3jjafvvut.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ojuudtvv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3coygebzb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ldnsgxea.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ztubdsek.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3vuctdwxt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mxesynbu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nzxegcgr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lpxksdjo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rywdcvew.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3sdeiuvyv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3xezrcast.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3lzvpfkak.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wryldfkd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mrettebx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gbljzoyn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3bkwehcxl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3husrxzgj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3dbxkdjdh.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3wkcsmxzw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pknjnbqn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3qfysoyja.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3mqortcgj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ggvzmzjw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ygrvwqxv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fnjfyadi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3jyoxkssa.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dnxlbyle.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3kahcrlvo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ttgnxzwj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3lskbxxkt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zkbtqjgd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zgjpovzq.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3jwkhgrmu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gbhlkdet.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tvgqzfdi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3rsptswqp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3mjfizrsw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3pzohvole.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3pndboeqx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zbbdwsmz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ibrszsvk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qrzkcmde.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vsaxzuvz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pcrmdsez.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sobobbzt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lpdekbaw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3prokcyfd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ikpxwfcx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gcwmcciv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3huavqrox.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3vmnukaeb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3edumxmfv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3dhaaljqd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3zeziljzw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3ctopblen.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3riltwsep.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ofzdglme.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vwfqnoaq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tjfexpro.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zfbknnuy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cfdgtkuj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vxqlhhfh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iuiuryrw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3eyrolfbk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3tldtyggi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ugrtltsh.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3thobdurl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3dgnjeill.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3srwvdlmd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3cqpkqims.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ovsmafzg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vvnqtira.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3tjbngqsl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3chihznds.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kjqgwmji.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3idabuhrm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3heewoogb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cqieuzsv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pxyafywb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fdsqyznu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cjymznhz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wvwjnynk.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mjkybyvx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ojiyqprr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lpfuilvx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cubsougf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rfsdvpoj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3znjlozho.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3siqwpnmk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3kpgbtjfd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hdzxagzx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3plzzjrid.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3tqxttrka.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3eisarsmf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3oyopsyyl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3exnpgwzf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vfjwcfmf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ylojtaen.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3blcenzli.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3vkbgrocl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3igcqycqn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3iyqlwxuo.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jdxwdlzj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ekjebfps.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3nqwyufon.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3utrbzwbg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3osludqte.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3wmshpsxy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3scpfsbxw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ujngmmwp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gjlnzgrp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3qxljgeak.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kpldezdd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tfifohzg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rtkfllzu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3uiesqgpw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bxkaqfgt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hwydtzwl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3lktrcvnl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rwmcnndb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3aqjwhwih.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ewwrpvey.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jyxzqadq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jrezwfma.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qxrkhwzl.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxqopzqw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xozrulhl.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tqzvwhia.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jgaizyeh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xxpctdlx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3avcwcyoo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3udqnfxga.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cvceernw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yatsuzlu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zukevqku.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mwoearsy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ehnrydwi.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3oqrahbrm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3eeingqcn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3wxbmlhud.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iqvrsaqv.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3preylbhg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvqymwfe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lgbijarj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3cmbvfoiz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ccgjubkd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rksotrbp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3jdkwcizw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mkwnvkwp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ftosggdv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3sfjwdaoh.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bjzrfekt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ztetthwv.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qdpmzauc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ejfmilsw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3sprkcplt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rvuadavl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3opwuhrmg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3khozjsqs.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3wmcksiea.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mkvvmijr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vtzejjal.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kgxsgoij.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3uwbichlj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ekihicjs.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3hbyjbcae.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yijwiicp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3nvyatsrt.html


<!-- 参考信息 -->