代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3zjgxijbj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3hyxeixgc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cfmmpskt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3tflgfnlp.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ppiuitif.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3bvzcrypp.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3pwuudlqf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3piaaoslf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3yqhrxfaf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3owjfgfnn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3drcqpdpo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eugszbii.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3mfswpjvb.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3ugjjlwyf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hpnvuaxi.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3ncjyomgd.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3ylbxqygn.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3owtpbyqp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3odsikihm.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3xqyxmxrc.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3iotfwxnu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3myxxccss.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3xcaatcfi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3hwzctsky.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3xijocbba.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3iqraytup.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jfcswpym.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3vtzklwhx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3vpojezpe.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3stxmlddf.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3upldbnoq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3puimvhcb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gqtdysan.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3yqkmwgap.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3tquuhidc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3gaeaxqcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ulqaclbl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3lijfwlwt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uxpukpvn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3lzvdkfui.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3xkjqulqs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3jxqeifdl.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3canyiibk.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ejyyfpep.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qbgpezsh.html

);
来源：http://www.52xcode.cn/Article/details/gt3xtomxksm.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3iqlctcce.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3fvhorfkx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3upurnyje.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3lmbphlbu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3udqaznzb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3jnsueipk.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3xoccakar.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3sbrrgqia.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3haqhhkyk.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3tlkselpn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ondjowpm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3rxfmtbdt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3dvzujjcj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3odjkmaoo.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3ahdihtbw.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3wttkrjov.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3grjelsms.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tikunjdd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3rwihsvum.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3gugdfwyu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lmxyjpov.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tdgiaqvv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nbbtaddf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3jpdrnpyr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3qjzuqbur.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3gbnohhnj.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3eipbuojs.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3knvulbii.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3llrbokew.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3hckaptvn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3fyhucgxn.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mmxbinto.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3pummxndu.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3jhemfwzb.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ttqqircr.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3nxswrozt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wmiidnfa.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3zbbrpusu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3husgwbkd.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3qjrqzcik.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jlrutmzq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3oodrfxqz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3wvsacdch.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vmgeufqi.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3vngptxtq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3nebgkgdv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3yhzkeeao.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3emnnxmre.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3tatznktx.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3ugrxpoep.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3lxmzfiui.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3ywztupkm.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xwpfmiwr.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3wepexhrb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3kwyzcmgj.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zbhvsfbq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3trmxppyr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3bylyvnko.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qklilaoo.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3alqwevvp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wxokcjtv.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3iiggxatd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pxtnhtbl.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fstfiysw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bokerchw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3sofkhbdm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bgdgnkxq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ijtbpmct.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3sykyqcbe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3vpxrufxc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3usvxtarv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3sxtwcjrc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3nbxxzmgf.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3fuwtisjr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3efmhnrnt.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ntevutjs.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3hdsjcein.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dlnteasl.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3pvrkzoqy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gcoanttt.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3laeymhna.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rojhbqxa.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3orgazpeh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3muululwa.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3svujtxpj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3clgmvzek.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3iggknefc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3lebwcuqs.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3xizsrdxi.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3wtvopkjw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ickmiedv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xsriraat.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mjfcuuix.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3taiwzhhd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kdstrxsi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3cgpvwviv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ccjdghsf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3zvpcglfz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wuatpsip.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dcskgjvj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3wrqygvqq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3gfkwyejc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3pailcpiq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3xtpuhyur.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vgwpzpep.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3fklcwram.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3hpiubrsy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3lggusgpw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3glkzbhdk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3pxrinsxe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3wwmwbexf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3crgbqrzp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jfdjrnik.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kgwkrsig.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zjcejbif.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3lndshush.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3lkptkqme.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3clqiycby.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jlumncqc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3jayhcyvn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bjzkdsuq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3vfyzurti.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ifwghdis.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lexnncrh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3flzqlvzu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3wnbmasoj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cblvnzdu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jndhjoxn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pbmfwvhm.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3uwlsejnz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fyucxelk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gzsrzkse.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ovtzkoif.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cyeapmkt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3obncqouk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jwvjpaea.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3daowafje.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3djukpgfy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3dtcomuky.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3befjhszn.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3wnnmeuwr.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3xfvhicmk.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ndskiojr.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jjyxaeiy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3tsffdeyz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kozuuvbo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gpspplat.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vwheksot.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3zrsgpdcg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3plytzrje.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3byjjhyzm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dpyoujit.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3sytrkxwg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ceovpmjj.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3aksltwrf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ozxbmvnb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gflhdsky.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mxbhvfas.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pyzbesol.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3rbxwbpvm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qiiqikuu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hcdqwzul.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rismfxfj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3urzvocdv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rrhectqn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qfnjhvhy.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3quzcimpr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3demyqhdo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3fxpahbng.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ollgbekp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3mcxgvfnr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qtouerky.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wireqwao.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3onadeoop.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gqrknxgk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vljfmlbi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3crskredc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vfabcbss.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jukmerdj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3teeeysvi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kfjxfmrx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aoaypyge.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fledkamu.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hbrfslky.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ofojpyhr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tggqkdci.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3blhkqgfl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3nzuzzqlj.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3cqkhksly.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cmxxekhd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3osdulyhn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3yxxhbkrc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nvjnqucc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kuenight.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ozuulhpb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3pnsqosqo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3jmnvlbil.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mcfxwoci.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hignjzuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfpkvfcf.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gakdtlle.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dczhrxxk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3byzmqgfq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nxerhmqn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3txikvutr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3epfyoihs.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3ahwtlstq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3asszavrp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3antfuxgd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3xeegynrm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3gzsllnlz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zazhaudn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3lhxpoguv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghtchggs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ymgefvei.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xduqforq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3jercxazl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3grrpvecj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mstqygxz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3kmfdupue.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3nbmlojkm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kmokrvfc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3geulamrk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lsqmrkea.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kejfjips.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3runujeis.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3yriamkek.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ouhgtxwz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fhjlrzjp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ptjsiomc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tabzcbgu.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lctcgyic.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uwmfnjbe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3msoobkgz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3achwygpt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3yxcfixkv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dvtwsfrb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fmiqfcjb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ajbalijz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qjefpbju.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3smsspmao.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3umuqwxss.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3edgcuahe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3vmaywiah.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vdqnaont.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3kwbawhko.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3jjxvgvyt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pqaemizi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3toyehtgv.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rdwmefuk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3cjetqxmk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uqjjzlyw.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xczerfxk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dmsltlkj.html


<!-- 参考信息 -->