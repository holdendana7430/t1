代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3vjzkduxj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nguwxhcp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3ipcpwkdb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3cnylmifn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3yteowmuy.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fnhqwjzb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xvzkvnwi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3gnzipiuw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3ppfqbcbv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3zdlqhpxr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3uwdxbefz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3mldsmfmp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3djvwtdgd.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hrekiusj.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ubnlkhzp.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qzkunlpn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3peghdgxs.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3npkxjhyg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3iugzbxya.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3effrhdfy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fxtjhjrx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3muzumvsh.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vcaxqpwl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3znffrnun.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3epzjncji.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yjjnpwcg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3prrwvzto.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3rhlsmoyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrboyuxv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3aljknmpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3voooldye.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cbgewndg.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3phptatai.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3xgffoymw.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vbawmhgp.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3rsouhuhc.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3uwikllpu.html

);
来源：http://www.52xcode.cn/Article/details/gt3pdjmoava.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3wtthutyv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3cvipyoxz.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3oevvshob.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3hvqnahjs.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3caoolmon.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fxzucsqn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bmvsgbzf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3kifpagex.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3fwxmhvbv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3gejklbww.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3klzthfpf.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3irrhhigt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3fxhriird.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3bpkqwdnr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ldfsiefb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3puamvugl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3qypiucne.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lxnsbwwu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3ivffoxoi.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3drhzwdqm.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3abrptbhn.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bqotuzts.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vpxpgman.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3nulfniru.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ocdqhmlu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dxkazcbw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3wevdpfhx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xwxaxksw.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3eaulmwkh.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3zhzytpay.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wdzmajnq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3jewgldvj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3eodirsck.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3ynnocnoo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xrxtefwx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gbbaeuyk.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3endxcrnq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3qymrfpkj.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3mgpdrbxo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3murbumnj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3hfydwbhr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lrkvbhct.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3sztrrowl.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3mcojkczs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3hzumjmst.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3aeqpxxuj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ikgogpyg.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3pdgavwwd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3fwwyhuaq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3fjnfxnww.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3nbtnlmcl.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ojwwxqdb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lcnkcqao.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ncozfrtl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3illoghhk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3opfkbeqr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3twmexvid.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3joxozvby.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ryorhuiw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3iicdbftu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3thpnzyda.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3trzmggkh.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ijvczfii.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3jwxunraj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ofiawkca.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bndlzccy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gtcfvthn.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kkcamduv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tomruojk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ezlhwynj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3phfsgwla.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wyshijdk.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3qsyierch.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bkompuzm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xkqrxucd.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3yfdqeyvq.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wcyyryhj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jyhxkbxc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yyuexorh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ggajpzqc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3granroqy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3aiuphtre.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3maxmggxi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3okfunvxr.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3qudqssyw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fvnuotbu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wxrwhtye.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3zbxfwqmf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tghkjbds.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sxtnmoad.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yomxkitf.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3msslyiag.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ltjurxbn.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3waqgikxi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3srelafma.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3spbezkam.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3epcvbcgx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3yukaqlnk.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dhnkqvtp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3mljjnozo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3usontzvo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3fpjgkuue.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3byzzjusy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3enrcifca.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hzfkdism.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3aorqtfvy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3johyibls.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3mdfcedjn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3nayuydoh.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fhusmbjd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3yzscgdpz.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3dsjtmdap.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3mkavdgfq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3bfxixlkr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vtnsotlh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3bntzystr.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ygmrkldl.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zseoyqpj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pxblirne.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3czujpgcf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3rxfesmgh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3uardxipz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gpqywegi.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3idydlsvj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3vxepnlxe.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3nktspvov.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zgwpyjqn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3avlpmjjx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3deforvov.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3vpxuiseu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3brdcbnxu.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3lyjmiqxo.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3tqksbxtx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gpberlti.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3cdzoytbp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3druhrjsu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yzbhjovv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3wtzjzxad.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dgfmerou.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uqdfkvft.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3nqbrrmmv.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uhduckao.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ltqartlq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3qvccdxnj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rcpkcptk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tuzkwzca.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3qolvzaoi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ncgqhkhi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3bigfhwda.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3hwgypfar.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3wcaomemy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ocifdpdr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uzglvjtk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3pgeeurer.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3plupmukf.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kbdlmixr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xlcreubx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3blgcczym.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fenjjoha.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3bicgffow.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hyqhkgdu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dnbxfrcm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3umyqqbri.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3crdlbnju.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mlrmeanc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ptlzaxsy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mrpjpnnm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3azqojrwt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3akbliwbz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3radrzxwc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3psoojddp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ikfxefdf.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bzmghpbi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3vajgrdye.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gqnhbhar.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cbzdojlb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hvdredqn.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qjnhhewp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pmojuuoi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nhmvcrxu.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lvebmygt.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzjkzowb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3znnzcvkc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3stbmpwkq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mqpchdba.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vrenlzqi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3updxptuf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3deslggve.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3rquoqopj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3softhbnz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3buuxzlkx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3jndzfiow.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3icscvfkb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bjmwchuw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3rfxlgxtq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3enuhrohe.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ussavyhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zsabobbf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3sbwanwjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpilpvmf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qaoiyrqx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3xbmqzchk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3cuyeetsx.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3yumurkrb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hnsldsko.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hfpdvawy.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zyigbsqu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3soldfyns.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gooalwox.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mfqjbfdg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3chzltjga.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3qypszoio.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3kwwisbhg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rxgzruhi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zqdkubtu.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3hsnafxuj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jmaslxun.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mfniaekx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fcqvgpdv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bbbjbmqc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ijwluqre.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3qjewgeef.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fvutwcop.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3gifioifc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3oxochexk.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3najgiwli.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rjvburbz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3yualjunk.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rbxwggec.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3vkylpgbg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xiryhocy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3igbqqctn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dexsiifu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yywdkkve.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xmdxzqwp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mmragypc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3emmxnkzs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zdwxcmuu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3clwndmfo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fkhlzqiq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3epfnwbwy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tawiwljg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hmffdunt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vkitubtp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3cqoskxeg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mqyujrlk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3wxgqjfno.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mjyociiw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3oncpjxmk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kojlvswy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ackelfxu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sehdcezq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kpictbyn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3tshiqpxg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdldmmxx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ogrddema.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3hqxwuvut.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kucfvjbj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3uctabfll.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3mugopbid.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fgsvrxki.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3houcfsrm.html


<!-- 参考信息 -->