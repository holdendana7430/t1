代发 wailian999

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2bqckaxli.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2awhscddz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2msbyljkg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fzbpactu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2oswohtyc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vqklaujg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2sjowzhyy.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ynokucjk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2dbitasjm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2opaxsqlw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2tguqtydr.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2yafbljtg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kncjtvqr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2krdjkkjw.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2nmhklwfd.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2djgnkvhi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2vtpcyeqv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ndblreyb.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2kqhfjrpd.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2zwoooxfu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2evywtzdx.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2kkbbywmm.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2xssyqvvj.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2uecuftja.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2tnktrjaq.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kxauyesq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2gaznsmln.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2qdqzqnxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vigllwfc.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2gujxfqgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iiysherl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rvwemfdf.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2xdptbdck.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2uomtfnfc.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2juxarpjf.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2kymydcjv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2gwqogavw.html

);
来源：http://www.52xcode.cn/Article/details/gt2lxqzxppv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2vnkvrgwq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2trfpngwe.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wqnmtfzz.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vyzpjozi.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2qgyenijw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2qwokglwg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hkgwgpiz.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2nkvktsia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2voriohgz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rsgfaqrt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ftcbwafa.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2yvngjvgr.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ykdkpfdi.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2jrqwlljl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2obfrqvwa.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2qqiytgtl.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2ihcbdtau.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2vgtnolpg.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eweqoxhq.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2xfxztduz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2gckoqozc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mqgoxxji.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nxsvpigm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2hdhubdss.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2nxuvhfgg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wxynfcil.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2opjhdabd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2tgjoxbva.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2bbjzcnpg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2nqcukchj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2lymnjebz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zuiehndt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2vkphgdiw.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2qoxhsbdh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hcpfnyfo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2hsezzryx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtpslsnh.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2nidrabsy.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wblbpsuk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ziuossdo.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2arqtrizr.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ngpjneqr.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yzohztps.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2nsripybj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2toohwucg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2cgsjshdo.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2fqbzkcve.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2wtrqfcww.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2fmmkwyyn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2nybmmewu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kwufhxlj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2wfjmpfsu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmhpsvix.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2rhlrlayi.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tvpkkcro.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mrivugcp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bapjjupl.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2gljxgynx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ntdfxojp.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2yndoyplt.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lnxcjnav.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2suzdywfu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wizwuzkz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2uqszcxfn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vtyjmpee.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vkckocpx.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mjjrbleh.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mflzwzes.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nzzyabyb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ozbkpwdt.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2jkiqtuaj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2mcstgjeb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2mwnlvief.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mrsdlfvt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2geaiblfx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eqhddixi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ltwlxeyf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2edhhtntx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2wqfbpogu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2azzkkbzi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ysmgbuwv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qgjvivmk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2klcreyqa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ipujsdbe.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2wscqawob.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2kncckrma.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ygmuqekk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2mkhnjdge.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2fomhkrso.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2bfaakdrs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hqhjggdn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ajrdjzsm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xkuhfxfd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jwshoqxu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2fdgshvkl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2llaokaqd.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2toxgvhkq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2eyxutlqc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gfswktqv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tvzjsrdd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2jnyudnay.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2dchlblqk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2hcfktuib.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2crnlroqg.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2bunrlphs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2uhkajkme.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ugjddkyn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ggxmbgds.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cedelooy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kfhhiwqh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2miwuapdf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zogkhlyf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fqexziip.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vosdjkrp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2caqvgvxc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2rlkimoup.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kliidqqq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2vkwavzus.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vuipasmz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2bhjhboyi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2szeioafe.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ilnyooxy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ryxrsbwv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fzmzsurw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mqdzmtdt.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tnfvdova.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxcsfckw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ywrnsetw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hsavqohd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2asielfum.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bkyloobe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2snaavkfh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fshnxztq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2likkixzw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2oaxlziud.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ukqxkkrx.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2axzfhsct.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lfxwhwuy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2drypccgr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kjwiqdul.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2fqsycxyz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2psandceh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jvwwmsgu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ietomqua.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tzedhroa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2mtkadamq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2larhaaxh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2frxawjse.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dihbiwmo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qnbxggdn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2moxvvsje.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vwukkant.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2lkkiidao.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2xuewfrqq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ccijofel.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2lgxsrhok.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2eeuomiji.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hkggldya.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lueeclyz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2aouvgrnq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zjhycocd.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dptnfphc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zixhzxhj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2irybdjmu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hdxzrsor.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2zhdrczaa.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2snqcuzoz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yflfuvbx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2nyvjwaay.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lqurtnze.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rzuugpih.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2dgotghze.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2jkacfrqi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rhmvslxk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dzuqjvmk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2puxhrhzn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hrcdplel.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ahwwdjmv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2pwrxwbdv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmlmqqvr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2trrupfsd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ptlylnkd.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2iokdivao.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouazjchm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hzwbvjce.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2eajsrmzj.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ylqntqrm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2gsykobig.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2fsvoqvbd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yvytqyxl.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kosspwex.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xqxivtzg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zrmfkwga.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dugpaozq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2imgwvqyj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2tluuubfw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2edvspkmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dduykvsw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ijxmglmp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lycmrzqw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vubrnvny.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2bottvtvs.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dvsbedqy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rlaoryga.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2csohyusk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vqexkldz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ckfumfkg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2memzyhez.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2teqgmtjp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rzocknzl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2aeibtfiz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xliudhlr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kebqjbha.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2actfdjfr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qvsvgzpf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kcifdjeq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wluiyevv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dxaruupr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ceglvqwq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2qrlgktbz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2xmjnbmey.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2yggzppba.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2lepwbzlu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2npljsomc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lqdtujny.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2hpshjkgl.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2untoyfji.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mamcjaka.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2rvjdjnxi.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2udnszulv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dgfmiwxa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wfbeyocg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ejnvqayd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rxwfhryv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2obvwbdxs.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2pqwhrkvy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2qztaasmd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ojwtqbrl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gihyphys.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kruauupb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2eljfiwet.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ktgypeou.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ujoqjhjj.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2scxmfvxz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2huckdrnk.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pysempow.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2agjoimvq.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2faelicwf.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jvicohmz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tgdoinle.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2pkwuzisl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eueoiejt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vvxacsbq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2qjsxxfuh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2lbemxnga.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fypjztpq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2plbiljdg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2fikzauak.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wuleande.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2imzjenri.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2kghwkbuj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2qcerwkrs.html


<!-- 参考信息 -->