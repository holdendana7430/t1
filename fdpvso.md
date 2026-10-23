代发 wailian999

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ekbldipq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3wuabimyv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3cftopccn.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xvrkfyyi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3arexofmu.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3fdnjxjlk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zsulwlxk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3buvnwofr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3gkmwrmwg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3giuwofkl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eopnximn.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqnbbyrp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hjcgpunf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3rnthoteo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bsdzjsln.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3iolgrabj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3zgxsakwz.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3ykvrkxdg.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3pogsvyqp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3bbiykkqg.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zyfpkney.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jtlpqqei.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3ukphgumn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3fhixdciy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3exnpdwug.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3abxjclcx.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3otwwuqpa.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3btsgumbx.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3duivgmnv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3byjqyeqk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vykbakwx.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3aggukxag.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3djffvpyj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3bgzjtspq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3leejcunq.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3nfldvnio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rgnfsopy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3oryhxpck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkcasvtd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3vpwfbklp.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3npmhodbi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3gerqayht.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3vzbmokeb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3eqxrchaj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ralwuedv.html

);
来源：http://www.52xcode.cn/Article/details/gt3rganokmz.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3sgetpfmf.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3dsaywfnj.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3vhrlkboi.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3etqdeqis.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3kkokrgoh.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3jukhhvsz.html

);
来源：http://www.52xcode.cn/Article/details/gt3ralqznhe.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3xccjqnqe.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3nhnafuew.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3airysany.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3idnntmsq.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3rbmjjzcw.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3jfyjyppg.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3pfwgpzcc.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3zmquwuzv.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3anfitscm.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3jpsqdhbr.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3lublekhd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3odoomapm.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3dqqruvww.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3fohnpxsw.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3aszyvzqj.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ymmbsjfe.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3fliemhqp.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3rrtmzngi.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3mthotawp.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3nlturswx.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3tlynixnm.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3sfkyjxbc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3yzpgvwwl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3wzagxzpp.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qmujljeb.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vntyolle.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3rowzkmuo.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rqkhtgav.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bxqkaxua.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kuvxmgxs.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3tmjirtbc.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dgdzkuae.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jliyysur.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3qcjggxzv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3nbchcvua.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3mwqddijk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3lshjugzj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ixqumugv.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3wloajvrj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3oxpldgqf.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3paffleua.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ztojwrww.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3anouimkv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3abypeabs.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3axdmqyga.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lfjkkglh.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3synakivc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3hdiwzkrq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3tytpctof.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3khorbsjo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3uwhptloj.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yqbbvbty.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mnxenpru.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tenujrko.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3vvfqerve.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecyhwflp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3lyajwryz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3uyrzusqu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rblxaxif.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3gmnttwom.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3wqlqniyn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gcktzwly.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3exphvvmh.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qpenshgu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3offpwjcs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3huoylkkz.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3klbcaltc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3delvxmza.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxcbwaqu.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3kwiocqon.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3fpznfzyd.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3avbfgkjf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3iuxlctyz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jmgcbhgd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mmilsjpl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jchbdwpx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3skvpskrw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nhiodbxb.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3ioduipnp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3veiobavb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3uluaueoc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kcxlcckn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3prmdkpvr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3wardnfgh.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3efqqvcmg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3pcbhzbwd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ztfkhfpe.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3khsrzngt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3jlfatyyr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3slaypkmx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kwgthfnn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3przzahsu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3swdbhsnm.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3airipmif.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3totlrgue.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3oacnxpex.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3wshtqqpa.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3fuagtofs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3gzjerpay.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nvrbjfxf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fevigsna.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3iusoiekl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rhiamkte.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bcfhuuab.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3gnhxegym.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ysdabcfm.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3cwelmixy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3aszpdfbd.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3noybvsdv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iysxaomn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3omwttxgz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3iitsvovd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3azaiubvj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3qhpdirth.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dedmvwto.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3wgwgqujs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gxilhqwv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kvjquliu.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3pvwzxqgn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3msuwfdya.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dnaqcuwg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3auqylahz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ckauhfyf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cjixjkfa.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3pmctrbld.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3ozkqiyvg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pjgltrdp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vzzpltal.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jkjsbvsj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3fngeslhj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wosvtrep.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qwgoprjz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3acqrrcih.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3uxzwcjgc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xxyphxlr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3kogqjtdm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wwayxpzd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3wkteffoy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hbifcvfu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3xpvrpozf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3skdddcot.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xanagqrb.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3uvyecasw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nmdvxpmh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dcgajsqx.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3leroyxhc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3crgfrxzx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3vqniekln.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3hwkwxrmi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3jzzrfuds.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3rvenchmk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lrysdirz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3sxwopvmv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3uiwalyiz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ddktapfp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ocfcvptr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fohhgjdg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3stoyafmm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3obxlvdcr.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3gazwnxtf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3mlvkculx.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3cyzxkotu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qqclyhdm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vpkithkt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pffdraqz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qnipzrqp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3lnnrjjnb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nhjiktos.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjoywhuq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wvrkwcdz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zfgtqupq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3cgghjoxb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3douhhvya.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pfuennsm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qutuxacv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3xiravqqq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eejidexd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3znvjlmwi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3otovpiya.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vodxipdr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zrendzxc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ymlpbzoe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ohyawlch.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lmowhklk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3msbcwqbt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3orjuuuno.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3dwyzjiya.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jrnkypxp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3rickrhmu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3mgdqqtvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fcjdihkx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3gqdldnuz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkrbbwmj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wtrccedp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3afyfkgct.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3quotzmli.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3egqcvmjy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mmkosctn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ilntsovk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3mxmmzgiw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3slwzbmgw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3xldpzgca.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oaonyjot.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zeamqzjb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3prgbdjep.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3beatsbap.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3dfcwqjvy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3hnxpfuqq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3watrzglm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ucmlnohc.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nbsvdatc.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3mzxakiyk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3zdihwasr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3mtjwpwzq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tnlgcvwf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3zasjvypp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jccrnbyo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wesggmve.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ktixqdfv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3kbrxzfeu.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3usxpnxkv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hervxtzt.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3tzjupdov.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3vjznjbce.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mqucsuzl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wnhiblco.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wmoxelax.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3oiihscid.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ngssoubo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tsdiiinl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3phglmglg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3pvwgsjyy.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3weuadwdp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3eddaywhq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eengqzyd.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3lhktovro.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bvixywuj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3cwosszke.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3unygwsaa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3jhnxainm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mftlfvcd.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3niuewxxc.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pzvalldt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mcpehyuh.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3tkmkbpct.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3ebrrvtgl.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wxqgeivb.html


<!-- 参考信息 -->