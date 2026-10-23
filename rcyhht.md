代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3zhffvdhy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ueejxbus.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3vcyenvlk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3azsjpnuq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3lmagbksm.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3qakdcdqv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3augyoalj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3atuckjmz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3xysfthwp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3crhkhxmk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pheyabdo.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3rfitgbyv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3wwaivekt.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3txovuyeb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3kzatnwgt.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jtnixocv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3eocnvtcv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ilqpecis.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zvawubsp.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qltweyuo.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kayeeatt.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3utedzezs.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3edbaznqg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3rwepgbrx.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3elxhonss.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzbmtgqw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3gopurbhl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3qspsujxf.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3pginsdjs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3xvxaccrr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3innknuld.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3aiwsmuaf.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3arnyvxam.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nffvhong.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3msokgfro.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3fleoeecs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3kbqzdryt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ypotfgqi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3cpehigxg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jbrrixsa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3uvtcxpgo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3zojcwszb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3mhclxqox.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3chkxatnl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hdkywsrv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3zfjbejnw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uifditjj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fxtaxfwi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3ojkghlgf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3pvzphcgs.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3jbkmxysw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3fqecxzfw.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ptpdsvfx.html

);
来源：http://www.52xcode.cn/Article/details/gt3dadwyyrr.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3oowzxtjo.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3trpaerwl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3sbmiuhel.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3kfutfifo.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3adixpuix.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3mcsfkspj.html

);
来源：http://www.52xcode.cn/Article/details/gt3gxpxhrye.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3rraigljq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3ifvavgwh.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3muzbcdul.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3hyssnwbk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3kzjkrhno.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lioumcky.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3bdwyvwoo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3qudersbm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3piqstfoz.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3lgnmcovd.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3fzvkzckx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jzoyfzrx.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3fshoipgf.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3sowoufyp.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3difjycym.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jcchjssc.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3ufnhaxsy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bseedpgh.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3kjxmobqe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3evfixyvl.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3vcioqybm.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3tdnphfdm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3idkcwnwt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3uvhpglkb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3evfmmvff.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3lmkmvkln.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jipxacfh.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wftwkwbs.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tekjrcjl.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3knylgzwb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3pqxalxpk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3wyfydczv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3loajpous.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3sonxqwzg.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3wkglzntb.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xgaijvum.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lpeqxnzj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3cybkmakx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tbgvqpvj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3rudteqiq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3xkljiwgj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3layxnvje.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cneelsfy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ogxiagwk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3kulyoiby.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ykanmvim.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3fcogavxg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3pxhutdez.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3rvmowdxp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ggghgcjt.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3dsladnvf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3atbaqzqd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3cvaoibqh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lzvqruyd.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3qjkzxssz.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzmfzlfu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bwjprrlg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3nblkopdv.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3accwzfph.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nikxmtmw.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cugirvek.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3upiounff.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bedbtdkj.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3aqqxamhk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3dyttqwda.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ingxxskl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3bobgoyph.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3wrgkhybr.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kkckeubf.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3tbyhbzjy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3xczlrlla.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mlijiwgh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wirfdtij.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jlifydmo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3neofukfa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3jlxstelx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3idghsgds.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3fqsalkxf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ooafooga.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wkljjwgj.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3josfphjv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gdnztaqt.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3kbmlycuv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qxsmuwfr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wdvifsak.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rfxswozv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3ulwtzqkj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3mhfyjdzm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3edutkgki.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3quaasrnz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3irxhzwap.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rslinwso.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zsqoyorg.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3pkfqbpda.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vwwmzpjs.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3oaupcvdx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3czjjzhau.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3chkwcvoo.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3jfbpfroo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3upcpvqhj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lcboetll.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3zdbyhoeb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3mojugjev.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3gdicqshu.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3atfesfij.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fniyombx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3mxgnomlf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hhnxzlce.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ioexllmv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3kbomiieh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3llscfcjy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3crznbzya.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3nkyqemwx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3jzqioprv.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pngsqemh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3slxdiotb.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3masjfnpv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3didmuovm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3wxpwhkop.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jprhrqoo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ymuzbxxo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wmxirjmi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3omtogxxq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nklsprfu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3isxzztpw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ralvhwgg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3nkldjfgr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3uocmtcwl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dgvggaxq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zpxnvwbn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3dnxcoubv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3aosuttfl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3itncmumw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3tdivpuhe.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3dgvrjhcy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ydwehhxl.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ywnqkkza.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3dszarhjq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3agvgercf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ibucyfhh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qcjsxkmb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3pedfxupm.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3wmrroegn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3jzosvurs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3czsavejt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fxffxiiq.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3swcondoj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3oioukodr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3sgtfwacs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xzsuwtcp.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3bjdswrqo.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wwhjdxvu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3pmdoidjd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vkremwia.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yybhfnnt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vjbaxwyp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ueihtkgr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rtliqfbi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3nzmskdmn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ypanxfdb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ilfdwfjf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ldvrdxnr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3swjsucku.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3mpzlxweg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3aevhvvxx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3oygajybi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ljthvbto.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3qfzfmjxr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfekyugz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3votenkun.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3umqcwxeb.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3euycfrap.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3metdbodo.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3uicqawbs.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cuzbspyf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3oqvryndx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxhmsjbs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3czzafbfu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3khibdlfq.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3eqgearwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ovpvqksb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xpsnyruk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hasshbvz.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vevzuxek.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3tzzpfpmn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3syanplrm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3xtpxbhsr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fgukyudg.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3sgnwhjwd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3avebcwbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bemngxon.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3iylhkuxd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dqaywvhe.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3mojhkklk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tiicnopd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yuljkdal.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xzqsxzoi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kpiidvpb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3opughulp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3pzewsjlg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wxgbxmyc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3uvwsuvlq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dokayevw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jmusozdj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bpmslrrz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpecydxq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3hwvqfnsx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3itwlvmee.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3qqfuwzky.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dnfrhcie.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3tdlkxoek.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ekzmasdm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3pitgrwom.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ncbkbrsl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3nvbnvpdj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ekgueuqx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3bfrhawha.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jdurirlt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3stynfhgc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uluazuuy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3tcywhvaz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3rarhgkpi.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dnwpjrip.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zngmhted.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3dwiycaoz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wiazboxp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3druspbzd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tlepfvlh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3aubxoqel.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uwbghrdm.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3hvpmaqcy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nycauhwd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3cpsprowy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bfoyfdwp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fcgbdcaz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mauxazea.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bubsmsxs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3fizdnhjh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3ipstghab.html


<!-- 参考信息 -->