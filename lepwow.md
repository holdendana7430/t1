代发 wailian999

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3bispfvtj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3tqfgdlkx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3icxknnsb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3umpogvnk.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3xfqtkmsz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3uxhpzxra.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3xbrtwtwf.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3djytjmnf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3evtcdquj.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3eofaavmh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3uvtxrhvf.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3aiygultf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3xcfdapad.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3ihkjvzjp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3eooujgaa.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3uqbbjdvc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3getbhbuc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lgeksfvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkejsmnb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3ogfufocp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3jlyusahs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3dsrnpzew.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vutlieqn.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rbdsvtbs.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3shuwirhy.html

);
来源：http://www.52xcode.cn/Article/details/gt3uxtcygwo.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3dfypjpiq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3yblsbojq.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3owyrkpqt.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3pijchnux.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3ejazleuk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bpraznzp.html

);
来源：http://www.52xcode.cn/Article/details/gt3btcfvpzb.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3eucfynwe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3exbxkmlu.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3leebvdos.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3jrxcssvv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3jspqrbbm.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3svmkfsnr.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3fcvtcsaz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3uecmnuqx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3opgndehn.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tlwjsafc.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gttnhabr.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cddxcfwo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ajdwxfma.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3wkeviyjq.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3hakscugu.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3shkuyqxw.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3gccvzuph.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3llglejgx.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3jpamrzoe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3mtrcffmd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3thnwacth.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3cgmsvjqb.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lpoyrnee.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jtmmipgc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3gdrzippy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3fjacheyq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ojposocy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bkfqvyjc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3rckgdjcg.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3klarxkgl.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xifctzfi.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3ybevtndi.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ehkoimvv.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3zjwjtstq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3azgkkvog.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zkqtcnlo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3emeovqbg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ichgazsa.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3wxgyulup.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3hnmxmuzu.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3azlytrbi.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3yqajnakj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3echrekdr.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3zgwbnjmm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3tfxkpbgl.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dyrzdhej.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ctyllygv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qqtwtreo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3rhxbwjva.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xjsqgiwd.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3ccokraqf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gavwlkdi.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ixxkqaes.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qmtymitq.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3aduqsjtj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufkuatxf.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3agumjwof.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3mebqnprm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3asynjbkq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3askxxikm.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hwiohimu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bybveklo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3kkrbcuny.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xskgcumg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gyrqbqaj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3myszaeyw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nnfsdfbx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3icarorvf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pxpgnxac.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jjjizcxb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mqwkloga.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mpdmrigc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dvhsfayu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3httmnuci.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3qxdvyrbx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3ucoejgjq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xsutnqdo.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3glsjabzx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3aqvnqemk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3tymalcvk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hdamqjtc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3tgzanxab.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3fytxqggi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3oejfyoho.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wyihoxre.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3czwopoev.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yifmyatj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3dxrldfxe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nqefskxs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3otiubsxq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xeibgjck.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pjfmcupb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3tykahfwd.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dznmzggv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uvdxsjsw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3aswzfaly.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ykbvqvsx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3biagdvfy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3byfwnnat.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3aqxictkn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3gzmoqczg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nsxvcenc.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3quulpqnz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jlxbscxp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fqfuezlm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3cnrvcqjm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vmbnoxjh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3baueqjxl.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3hfwboxwr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kglcbwxv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3yqfkipoo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vvjcrryz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3lrmizlam.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hxqncmqk.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wchufhdb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3dprmfvea.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3ogjxicih.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3roksvvbw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nirmfcym.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qenaannr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3uuwjubhr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mlepyvxr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3cpibdark.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kyypwahx.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3pcrxtlnn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3rjgumogc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nlfomtgn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3dqptbzlf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ycgsoejb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3jgumisae.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rpnbwupa.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gqhquomu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rbqhvrie.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wskbaqyv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3rcxpwkbq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yllkxgyk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3laojchss.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dyirnkyf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ygezdigh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3fdvdtlto.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3oaqowcdp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3rsgescdm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3yepqojaw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3mhyyjcuk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3dpmckyhf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xepvbize.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jgobfyvz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3trbpbjtx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3vpldadxb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3nbmuzbkz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3igzwwjjl.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eevxtqoo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3oqsghbwj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3eltqpuel.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qrhofxfi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pfowkpxx.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3kuululda.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3inzwpizy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qprzmzoe.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ebtcovla.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ppwlmkim.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3svfecdrr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ejquuogj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3gxzhxgga.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bqmnpllk.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yumlcrlk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3kelobots.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3lnulaihy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovwmsywi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pykvqkdx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3olxrosev.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vpqknvnl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nohwrhwe.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3iixvejgn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3llgnjlve.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ivymvfdt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ojdlmedq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rtwmaaqz.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wxsjwxss.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mqkigjpp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ccyoblbq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wttzjhkw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3lqwvhqja.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3eseurtqf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qnijzsfw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3acfkcztf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ticossby.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3loewdgpx.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3oqkupxje.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3tygxovld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwbydxux.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3fxvnygza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfvzymtg.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tvvitqpk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3bpxbmcvf.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3eeorzmkx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fcicyzjk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3rwjacgdj.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uybhgeif.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3bsiaxdqe.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3hupnlbxi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jbemlbvu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3txpfhrrz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3edfeyrwz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fbtjqdau.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3vrpjfhol.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3juqqfriv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jfikiatj.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lesxwyev.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dkefaejt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nxdmpuzc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ftqretwr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3uwzuouiy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iblzppbd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3emebzofo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ouofwcgr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aejxntji.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vgwvvmwk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3stedkvnr.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ndloahwa.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3coiqskxm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ejcgxgwa.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3rlkwlylb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ndzdgchs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fhzwholi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xqxnlapx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kqgbcyds.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3snekjjqh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uzskgzuz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ctdixfat.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tqkhobgk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3myauwzyd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cpgjfgpn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sjdxzteq.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3bkrljmfo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3bbkvcwuu.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3iektejio.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fmhxjfbz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hviqdgpo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zcsjbrtz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mwheawqv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3byhrsgam.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3sjhzsvlr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gprzticv.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3bllieinn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mmjkvlgb.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3pmttrsez.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3aaohbani.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3iijjuubq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gqhjsjjr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fxmrfeyf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tbrohrye.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lwnybfvz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tkjoifxa.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ahkbobaj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3ayjulife.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3mamvezkn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3xhhwxwvy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qcmgdtsl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qugtuzpj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3rzhmmyhe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3gdieaaqh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ioexbeek.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3hlkzpxxu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3imzuqzaq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3msnyvzhw.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3lnamxjks.html


<!-- 参考信息 -->