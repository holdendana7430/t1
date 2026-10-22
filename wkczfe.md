代发 wailian999

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ostxldsy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qcrcwkvt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2rmurbohk.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qmzzyqnl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2eumgztvn.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xzucncuh.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2srzqpryq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2dzjdxcdy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2xkdvasgb.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2cmefnvdi.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2uvivshkl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2bhouoheu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aancurfd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2kybzagjj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ayhroqaz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2wwxrksjn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zwreqijf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ojcogsxa.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2aypwcvoi.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2fsrybyfl.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2vunhzccg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ljjpskwe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qbjswejv.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2xrqimxsk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2dzhyiouu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2swuydlss.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2stlzerwb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xmjakkiy.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2pbkjlxek.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xwjkeyhm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oksehkjk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qxfqzeoj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lqhehnma.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2uwafrsrh.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2diuqjgyh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2exrekkxb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2doerhwew.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nretldsa.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zgbzagwk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2onjnjemr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2eqnlkvez.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hrwosxur.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2epdxiihc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2lhxbbdwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jshtnidp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2diacxjja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnhhbewu.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2ugtlkqvo.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2kqjwkptm.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2fbgblxtu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ayulgyut.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2sezpnhby.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2nxlcdtyj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2czhdbwxn.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2hfpfttlh.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2mjefcbie.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ayqifmof.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cieiqbcq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2bsyczkpv.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2pdmdxeht.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2sdybveka.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2cslfwgtp.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2bqkqgatz.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2hodjumoi.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2hviybkki.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2jgbqcugz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2rqneasss.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2tfmloecz.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2uzmkwktx.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2nxccxcvm.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ldazufmc.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2yfqoikld.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ajwsldlm.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2amqgoegp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dwpxwzkl.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2nosoolpy.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2pqwujzlb.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2thmdzrvz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2zclftbaa.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2kitvremu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2drqungip.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2sqryxabt.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2gfahtthg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2omqvdolh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2opocnxdq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lpllxehv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2awrruzlt.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2pycgskwl.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tlpvdimf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2gfqavhlp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lborlnvj.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2zwggkkoa.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2nsevkycl.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2niwbbskj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2ukxmfvwx.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2avrtjytz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2jtdglxjo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ivuuugaq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hqnsifvn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2wlrgjbjg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2lastnfjz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2piuvyhgk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xsnodlmr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ptvfuifi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2xfvxrbts.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qglorluv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ozndphhx.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2strfumjz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wtbkvsqe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2pjufayrl.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zihjoncw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2urnohbtd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vqqmliph.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lkjgqepi.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2deuofzgs.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2pyxqfmxe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cjeudove.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2wjrfcrjp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aryfkejf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dpwwcadu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mxoytgyt.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dvwslxah.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xjpdwnjb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ghwbhmzd.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2fjspzngy.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2yjeuntmw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2axsabawj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2whqhcodm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vjmclavn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yfcagjem.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ellrzqch.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ktwmehku.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ncszridr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ckcmghht.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vmajdttl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ooowubzw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qjkucymh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2syxugaoh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vukqawpi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wyckfyay.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2aiaucvce.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2jdwdnkfq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2qykfcpty.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ghtnaisl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cflhtkfn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2itfqeyyd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vzsejqem.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lzqdozxr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nbbfpkly.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ivjxivbc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rdeqjxwj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2pkrguuhb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2futqebnh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2oblxcrmc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2yxbriaba.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tgorgatq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2krpwhxzo.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qgwrtvvt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2gnscjoam.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2jambxmmi.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2kxbzvsvx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jmknmvzk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2usujyopq.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2uzfjezsk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jzvtjcnp.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ggknyrqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2sbmqpzud.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hcjgurji.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2plwehzsu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2qkkriyhe.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fwkvxmeo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ytayhamp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2qwanqizn.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2zgcilcme.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hvhoccet.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nhdxzwvt.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gbjqybjn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bielhkcg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kxnxenxp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qpdqkmqn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gagkppay.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2jfmmonah.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ocrclvov.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2evglbfkk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mvzfffrg.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2blmrnefd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2eyyenuoy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ntszdogm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2uywvmdgw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wouljvdd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2itgopjjs.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wvylkqhy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2hjfvcsrr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2miwleixp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2uyalxzwv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2sksemzhu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mjqennjd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2uxgozfea.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2fdkeztyd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yxwxsglq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2phqnzftk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wydmefhm.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2qpakdeqp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2flhgjjee.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wtufuqor.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2hsdkqlnv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gacxgusd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xxoblzec.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jdixydfe.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2sofatqab.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2iviitclc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2btchxhll.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2reayozgn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2svcvfndz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2evrrzxhy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qzucwlhd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2kzvvlysv.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xliwlczr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2grjathhv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hivkeoic.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2sajzyctj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wfbdtoyc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ksxrqjtc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xyayzrpu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rkqqseuu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2qvbgxjqo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dsuinvcb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zuzklmec.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2yfyjyisv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jlpnolpy.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jmjhorrh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fsbvanhr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2cmtrztyk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pjzvqmyj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lirykekf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fafrdlua.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jveufhrt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tzwpinfu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mrjqatwb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ffnaivnq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tzkfaoqt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ivqqxfig.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2afryvmdc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nvadiqzz.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pfrzgplz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2meswsyry.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pdkqtnme.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2akwhsthb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tgcomnbm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ofdfemgt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lhinsuqg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnnknhvi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ypqboznt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fdijgqzw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2dktfyucr.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2llsmurqo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2evrppqgt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fqjhtvaj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ktrrqmha.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mlhnipqk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2glwwbtvf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2gfsfmcnf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2hrhngxqg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2npzvnecs.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2oyxeagfr.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2accnacbm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ldfkexvb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uifesalr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nigntpuc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hjffgivk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jcqdnlmg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2xrjrwxcm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zaknvkjk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cutfnbtx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kewqjpdg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kbgpkzwy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2sostxncn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pptmctqv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2idolbgmt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2yixycnpa.html

esac
来源：http://www.52xcode.cn/Article/details/gt2htnilslk.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozuyabgc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xmoswhco.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2bmgepdxs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2poviyoup.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2orbbqnvs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lwjtsqok.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2diiqyafd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2zexiosby.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kjuojjzu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xfxkpdpu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2htnbzjsz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2exlzflcg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xkgdgmhb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lfiryiej.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kkyxethj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2cmsisylp.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2lfcpaceq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2odpbbhyf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2twymjrvg.html


<!-- 参考信息 -->