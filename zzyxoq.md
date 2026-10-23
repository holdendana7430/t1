代发 wailian999

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hybilobj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3bkdnlqwn.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3trgxxvkf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3flmpttoo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3agpqlnbe.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gaxaqofa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3coaotxwt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3taqruzpk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3gmailbun.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3ylinsbki.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qqppxeyg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3snbpqawl.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yamxoznb.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3blegiyex.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wmcjknth.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3jgiyhlge.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3evzdgjug.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aztiipwg.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdaxhyar.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3dnasdkty.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3mfvzpseb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3kuivrzdr.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3pyowwmff.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3rbsruhlz.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3rslwsojr.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3khkafsmg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3orsxvbjz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3bvzxetyb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3jxixkbdx.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3nljytpmu.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3cvyrssrg.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3dfzxnhmd.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mmysnsgm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3muxsjwwr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3wkmqruwn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oteayhww.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3pabgwpbu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3dmrhbfld.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3ahbkjjfh.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3eeaudqzp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsaaxtkl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3eiyvxqoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrgxheum.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3rpwnfjzy.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3dwxjsgdx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3acrktkfy.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3fqaqaqgg.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3ggyumidv.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3wrjeuogc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xgkimdae.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3byxlhlug.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3bykcdvle.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jaqpupcp.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3kqdpkeul.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3vtczcobr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3bcocjjet.html

);
来源：http://www.52xcode.cn/Article/details/gt3xboasyfx.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3twhcsiuy.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3ponrknvs.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3zmqgdllz.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ijejdbrl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xihbffgq.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3dcuqcmyw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3hxwuwmnf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3iiveezew.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3wbgrzeyl.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3boipchqv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wocrfxkq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3cbcwmriy.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3wmtqinzd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3urgushqh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3nnsbdgff.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3lwipskce.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3kvicszum.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3dsjucslh.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3kmegdsyk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3inrkhobz.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3cimwudsj.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ojqtiyrm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3uqjsteyr.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3oyxfuoxl.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3ccoyfipx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3gyvqffmu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3dfyzdaxx.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xfzllgxt.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ptxsqajw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cgpalebu.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3cxfiyntw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3bgqagrkc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zbldamkn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3bvtguzkl.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3lmvnqucc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3pqlbtxkt.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3lcicdmxo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3naeaujen.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3amsbnitw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3etgwlwte.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3skowlmxw.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3fmrznonk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3pmbsayec.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3vjpifgll.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ojbjlrsu.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3oldbzhpd.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gfwvsjsh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3qbupskru.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3azanffvk.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vwuriomb.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3plehmjzo.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ywvjhojs.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yniuihip.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3htwthsvx.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hyyolxjr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3srlojpot.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pncvwtwu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cawlqlrk.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vzjqwfnt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lzwylldd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3txmkvysf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ueemlksz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ukemwmee.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ezukdaqq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hpgragic.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xdnxxpxy.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3qrupsllm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3uyohsads.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3htrmxwag.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3iecbggvm.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pwsrbbrj.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3mitsssbe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ayqqadhs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nslwzkmk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3byzfacnz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3miwlqwzo.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3boyfaxiq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3vtvrniue.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3rquzhunk.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3urffvqdt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vnsxbpej.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3pnoxmvcq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3lszyhahu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ajfaosvm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3gbpfcwyj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3extyzdxz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3famxfjun.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qpwonaav.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3zcguoxwn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3mlrevssi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3bspgtwba.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3gxkchdrb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3lphznjkj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3serhsmrc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3afozbiws.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fydlwufc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pnasifye.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3thipywkl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3clzekkyq.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3jdvhhvfe.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3nibzqetb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3svepyzwm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3mwomdhys.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xrqrnlkd.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3hwurlzio.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rlrxbstd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3krsjgonv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3efejxqht.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ujgcqvxy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xqiedjki.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3aczypwoo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sffplekc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3roiqhpkl.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xsjajmbe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kzufjcwl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3jytunljn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3byvdlwho.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3yuddexyy.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3peacyccw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cvobzdbw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ndfdxmls.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jtrdhfhu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3njuspszn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dgmwmktn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3iicabcfa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3wfjsqzhk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wzxwlkja.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3xpfdxarh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3kuraupqi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tvplcccz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3igmfmlqw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3fnujqkdw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lvsincos.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xzededcu.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pmhwbmro.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ywmnydsa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gzbvahxt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3iacxxoho.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3gpxfxnbs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vsvmjyzm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3epngjgvb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nzyuepqz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kekgkqwy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3bpnukouk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3luhfqlif.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vmtbvsmb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bivwlats.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3rxrptigg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mairtjwq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3aikobulv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vlhnzqsa.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qlybdftw.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3inhawlop.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3cytruhoy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yzrgvyll.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3njmyhcfv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3osdcxxuh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3neoivhkx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3crprppmw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xwpuyfrl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wjwkzzzb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3sktjvjia.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ombficli.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3juxelsdy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3wlcdwcsz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3buvawjms.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3pmcwixjv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zlqxbyhq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nnuupbbk.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wmobdhsf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ziqqilef.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ualcoklb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bouoboir.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3fmtjspif.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bzgtyunr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gpixbsxv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yqxzghcz.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3shdqnvwr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3oiobfwqw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3obzanrms.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ilwijxkl.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3hbhdahqn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3wrxkfglh.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bhsnoxyf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3mwmdkmrz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vkaicvgk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jzbdzsyf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lgpczraa.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3inyslheb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hnqdwbqj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqkeawyc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hnbscsxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsefshsq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qsjcndoi.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yarkkzpv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3aqbkwqdy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3jkgsqfnr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3zktemhrv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uyifpvbx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3nsxbawvr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tazumwey.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3upliinwu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3kcvoesac.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfycllbt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ebwdbpuo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3rgtcaweh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3srvogkrc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3shxytbkt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ojgfkvgk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3tpjnbwts.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3eggxlumt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xkcfpchj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hcogacbo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ggbvqyjz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tdfkoawo.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3srnmkeub.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sxqhcvhw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tgjsauoc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3omyxylkl.html

esac
来源：http://www.52xcode.cn/Article/details/gt3fjhiboha.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3gvogbolj.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3uetsbxma.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3mgwzvmky.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tchriboy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3aknionbz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cfksglhn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3coajvymz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zfcgxgna.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zrkvoncf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3alyndxpj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xulkssxg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jdmlmdpj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3vpkefxjo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wjcsncwa.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3gnqomwxj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3kczsmkxa.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xojjrccr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3byqjhxmy.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3zmfdmhua.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3bvvnkkol.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pjaknxvc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3fydqtlol.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3eqvnclji.html


<!-- 参考信息 -->