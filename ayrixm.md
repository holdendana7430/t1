代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3jahhowaa.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dgdrhsil.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hewshluw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3hovqagni.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hksovlmu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3zdqelrzb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3wmkbdgeb.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3nxxuksxj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3dabfzwwi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3uqzibras.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3obebpieu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3momsuuqx.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qvsjvpml.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3lzpljoix.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jimebgwa.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3tradpbfk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3sxmqnvkt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3msqiyxyn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3knkiliwa.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jtalgkmc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3wlivwhwn.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3riskfzjt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ucysdngd.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ymtyuwjh.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3xggrdgsl.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3vejtmkze.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3czwpbhge.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wcawspcd.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3mlbgawjt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hofbaqbg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ywghkjse.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3dwkorgck.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3bwarfquj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nbcxavah.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lkcfkgrt.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jewdzhxy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3yhndkswq.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3llcbwfze.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3azuxnhcg.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3ejceuzuc.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3kkmnebuj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3vyhlxzte.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ysbzwqyj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3pdiuloyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jndjudka.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mxmfbftk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnzupstl.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3lgfrplhe.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3oyjdnpqp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3pnrvqaky.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3poegqrbu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3uiyxathu.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3esocskec.html

);
来源：http://www.52xcode.cn/Article/details/gt3wvbriqkx.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3xlhgtcgb.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3thtwiqxg.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3qtuzffbe.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vqekajxg.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3dbsfybeb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3utqwjlmv.html

);
来源：http://www.52xcode.cn/Article/details/gt3vjcmipdk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3iperwpui.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3azffwqgx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3enrtxnlb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rkjhbooh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3azyeobya.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ocdxuyue.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3uerczghf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3dfmaewgy.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3xfmlbzdt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mjtrtfot.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3qndmyvzi.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3wunwycff.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3ounvsbzl.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3exapxbmj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3lqnaaghm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wnxypesh.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3bycwewpy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3nbwowfph.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3dbbwaojx.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nvdyllqn.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3eemafgur.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3fixhweep.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3bopjzkaw.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3zqgoxemc.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3ispdzmgq.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3jsdsvlzj.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3elssoreo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tnmbhtap.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3aznmozdc.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qriywlkq.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3psyscycs.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3zqeilqcw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3cqqqndsz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3rkndccov.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3gatcgzws.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wysfjreq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3fufjxxap.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3dkckchwf.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3zmifekws.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xhyuodrk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3hvghbwog.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3monrshdb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3asfxcrno.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3jmccndiw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3yamzyfqm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tsxcairs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3xocoerms.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3bjjnkosc.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3cgshkgqy.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zlrinitk.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3poiqtxgb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bvlnhgsq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3wvryehnc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fpdbhcwe.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3ghlqqpgr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tnzknmjt.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3lifijpjm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yihmrqcl.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3luzqhiye.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3vdadafrl.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hvqhyoeu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cugfsufq.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3shamjlyd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3xmewbkiu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3uejxuxzk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gtkoichy.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ovnvspti.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3kbhlmtdt.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ryyfplfv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3czynvgid.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nzhffaek.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fswtfbyi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3jggextjy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3piwpsshv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3efdmhehl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jtrlyism.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bcuurivk.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3vsijhphz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3pxhfijgt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ufveepmp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3qzijubpj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3rxczrkjc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3baxsrfky.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yirliwef.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3khcqefyr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3tbbsnisd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pnlplhcf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3vkjbcdue.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ouopjnui.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jkpfsavw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xjksezcr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kdhvwnxo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3objbxbvw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3crnohhov.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3mggjllds.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3uewwwvkf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3uwrrqwfy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fizlvbng.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3nqmwulys.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kzloxcoj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ygochczw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mavgjqqj.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3nioqhxfj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vwgyrjdt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3cqzeyswx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fcggongw.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3baktpisq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3edgxpfzu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qheyivbd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nnyzxvli.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3aahzwoio.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3vnkkxmop.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3secsixmd.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3tjwuyhih.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gterirxl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kwigxdsw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3qkarpqgd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3dvpritij.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ehsvribv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jenhujjg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ohwjqniu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3puzovouv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3efgqskwe.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ayjefiiy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3kirbuigl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3jcqiedda.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3allxqyuu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cgzxcdac.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pwitzlzq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3chkmgdmx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tstzqayp.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3swrtjnft.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3nljczhsv.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3utbhqdqk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3lfgqmdtl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3wdabbhmy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cwmvxomv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pyxsztwa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3uxjnasjv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xsenltcn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3giazvbfm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xhmcwods.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sqzskqfi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pyqvgcet.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bduhzcaj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ogrrnufd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dthrfrka.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3vbrppoas.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3azjcctkt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3uewjiaft.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3vyhkvmli.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rebmrwov.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3mvhdjjys.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3pbhdeccv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3sgpwmbta.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3tiefwesv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3frszqwvo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vmtvgkpa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xavljetw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3pvpwwurw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3grscymfd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3zpbgfxsy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vipcowqw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jgesqbyb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ypetwiar.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ijyzrcvq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3umkducxy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3iqlowpos.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3buisizxt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3zbikuwmf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ofznisud.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3euhsircx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dovsgboz.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3lyluldkw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fptrhjxd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ngubcnwi.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qtyzkanx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zhccxdja.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qzvodasr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3octzxsbj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3jtpchuvh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3bbcarmrp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qkpjfwab.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3otxgccug.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3dehmfuic.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czubklws.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3frdffidt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jdniphta.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nnuhxxcj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3urclfuaz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lzkgogvg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3tiwqiwga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3birimxxs.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zcrbrsde.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3omohxfos.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3lmztecwe.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nuglnpdu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dwjheqka.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bcitdyjh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wqnfrepj.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3rrgyrwgt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3dhlpzyzg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3stmbcnjo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3bnaticcl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3wkjstoca.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jzizqrpj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3icajaagp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vwkywcun.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3sfkqsaph.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3odqxqygh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sklmiyeo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vopwziur.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zcfxrkgr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3revkijad.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jmwglayp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3dkbzugam.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3jzxkjolt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jshsxyys.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bzonyudj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ixapjcxv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3aewptudg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3xvlvrayw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qlxyqfix.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dtkaqrip.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3kdgsxfqk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vktsniie.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3nqhwoofu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jytxvble.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3qvfskuqr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3antkynfe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3uspbaqbs.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3wphudwmw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xkzdmxif.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3oufgegnp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3kolwqxge.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3veaaoxtz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3dwvyciff.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bkzizuwx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3hrwmagah.html


<!-- 参考信息 -->