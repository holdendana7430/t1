代发 wailian999

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jnpovxzj.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3icvyavrd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qdwaieko.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3lrqsbnqo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3agajodbr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jvzybhrz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zfmwbsvu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3eorcepzv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3nnigapfy.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3awxjfwue.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sccawljv.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3hwupdogu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xiwnnrrb.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hioqojvs.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3zfenlkem.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vwugllfj.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3jtigfnju.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3czgdxegs.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3vetcqjmt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zsjuqpkw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3exhsdkjr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3yzdyddfb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3bszaohhk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3elixvosq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3edpbenea.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3sdjvtgdy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fvboemxi.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ihnfpvmp.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ymjxmxut.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3amnkqzhk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3fvrjcenr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3xlkjevus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hefejefi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3cycwajys.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3svlwbbrw.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3iyxurnnh.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3coxcfdpu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3ssmxhgeg.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3xtnebasn.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3exxzkuhr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3bgosjsqd.html

);
来源：http://www.52xcode.cn/Article/details/gt3bbwtsqvd.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3xubszlin.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bfdpbrab.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3goimlvnu.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3czdijzsc.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3tepzqkem.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3nrkolsfr.html

);
来源：http://www.52xcode.cn/Article/details/gt3sspokgoh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3cqilylpl.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fvzsleqk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ntlhognq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3kmecofyp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3igzhiflb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3yvnyxemk.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3zlluazlb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3umgizgur.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3vazrjweq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vcaddpxu.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3ihzgbpqa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3bcgkiigy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3dqvzrjmj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3vtenwjse.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3vrqbjgez.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ypxjaiut.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3pegevtfy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3tlsblfpb.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3xpkqypeg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3jldhewfx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3lespedot.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3imuhivas.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3hacpkqrf.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3elgbdrvh.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3cleuqczq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tnoopouf.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rrrvdcwt.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ieiehycz.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3zniscrpo.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3elxuvpgv.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3seufdseq.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kpqryhfz.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3ugitnnut.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3gtaugnsq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3osabcqie.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3jdsthhxs.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3ldhoimkt.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3lmmebrhq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wmezcjsp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3tsawgvfb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3prgdwgpw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wqfisndv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3mnyaprdm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mjeuwoxb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3ovzhefko.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ruilczny.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fpxldexi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3oosaaebx.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3fqaadlhk.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kpdqhpcg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pqcwlazc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tahxuuur.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ktqdocfo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fdkeumbz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3imcfyisl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fgzskjuk.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3hkddzxwx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wcxqvggh.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tyxnhagi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zncopueh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rgbuqmza.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3azavjjgf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3iwfyslgn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3eaqbpgse.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3vcrftwjl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3pyvlfgdo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3afonsjnp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3oqvjrunp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aohbkhpv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ragulsks.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vkglyriy.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3oiaqychw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xyuqmqdo.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3cdewfvcm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tozhrjyo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3tjwydzky.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3lztjkcgg.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jfwbawdr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3bidqmexv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3bmzglbff.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3qakadxgj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ezmejmdi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3etlvyjxz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bfsulyrg.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ydambzei.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ysunuons.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3syilyarx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3oynjkbrc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3tzbdeejn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3onmpbbej.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3dbavxznb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ouecxinj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3pyohwcvt.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3jqadaelj.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3uivpfbwh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3zfzagodc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qhjhnrkh.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3dhhbihei.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dptalvro.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3sgzydvpi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3lduauuno.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3kgczujxm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3nlqkpfwz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xrlnujrr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wgcblqsx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bqnbajjk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3ybbjaimf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tmnvmozj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3bdekzsxz.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3okddntsk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3owkwhmuv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3xzdfgqzf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3idwuvzzs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xheltnef.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3xjeomuno.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rtkkizlv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3hpddcwbk.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3zpyygehr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zahdkzls.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wpfgfzcs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3yozumxwk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3igcrdvgv.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3yfroqxut.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pfkuinmo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3jahnoebn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nknswgwc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cdqzjeln.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ahnwsjaw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fncnezfw.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3oqhcwffw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3eaarsofc.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vbywxbas.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3enomtzqi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ivlveqrc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hzldabcy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3oxtxzzwd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3dpymjhtt.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3suaqtblx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3hcrkqylk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3qagzyqpa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3atpmpabb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3cqbcweaq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wzdmzwjg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3iqlnhacf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xwpiquwc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3goqsjoin.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3glhxmiep.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3obasrjay.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3odxaksgt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3oaasjyib.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rgqlnuzp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jryhmdqz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3glnuopko.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3oocttanx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qrwizxfa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3zeixmrgj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gfhtlldb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qdmklyab.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3nqyhyqpk.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3kmiqgjfz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kwdrispl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3fasoeeyl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ifjnmcum.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3lycpytom.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zgkpapnd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3anytnfhx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ndfggbpa.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3aotdstup.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3flcgnkyh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bvgpswbv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rudqactq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3axuvdgwl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3infhdgai.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3fuuynohs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nbmbljki.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3aooisnaf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gstradtq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vbtjewlj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3zdetrkqv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ohcczizx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3apzrmmmh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gbreegfx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3pjqzetxf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3azwqwtpf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3jxlmaiha.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wkzyrdsj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lsrutusn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qjspclzg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ivdubhtu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3alkwoeff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjvtlljx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xwzoefhs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eiijlqcq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3oojmshgp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3feodzlsj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qgjlysmm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3gfpcjgno.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bcpiobfs.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3uugwgfva.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3dhjzohxd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xdjsxxyt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3uwguncbb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3acqlzqvr.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qlajdaqs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ovixdpcg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3idpnnnlz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lttceewr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3fhlvmtca.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3nincrdbh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fkcouglw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qervdiwe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3nhgxxqym.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ryhlzthv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3cjtrdsiz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3bkbphspl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vxrkolvc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3cnlxirln.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3lskndiyd.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ijzdtupi.html

esac
来源：http://www.52xcode.cn/Article/details/gt3iarrggjs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vomlxwwx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bgdeyftm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zahlcbmm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3aoixodcp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3bnibiafy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wxechsci.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mdussbct.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bwafawyw.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3arremxyb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cfaqlfdj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3ssztbidg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3autxvhla.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zupxzykq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yebldvsx.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rxybyikg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3srzupogb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3dvadyswo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3klmxyxax.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qsmgslkk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3gxsuddph.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mohmlzqm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zmynhdun.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zyuztwzr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ayxzjilw.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tvuottvd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rnfgxhlh.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3gvbyoflz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dpeerrcn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3kpddktuw.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ftsdxgem.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3scitsefx.html


<!-- 参考信息 -->