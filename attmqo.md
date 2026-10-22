代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bunthnyz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2sirvobxp.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2fzilzfae.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2yhwjxiqd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2gpdfizsj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ftvpzmpw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2fxkaagyu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2qibkdgyl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2kwlmpben.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2oqxzdkqw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vokhfove.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rwgxfgvf.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2iwqimsvs.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2erxivbsg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2wrhiepdc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2hcihxrfg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2ofqmddla.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2yxdyfxui.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gkddqlht.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mwpmuqtz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2hpcfhckm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2imypqnly.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yctwxgkh.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ausxqwjj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lajhpwwe.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2slcbtitx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ijijcpjb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2otcoydxs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2obnqzxar.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddgexkue.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2afrpogam.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2ujmdlhdp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2ticzbvck.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2jqcjviwg.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nhzrfqdt.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2wtapcwlb.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2mmmsixaj.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2xakydqmq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2arvoolqv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2amynfqkc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kbrexvdt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2whgiwqlt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zwvsbtqk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ftygnike.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wrsnptnx.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2ykxlosik.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2mbqtxlcc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2llfidshx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdlsawkv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jhrajhki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ndvidtmo.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2bhjprlfb.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2gzheewfg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ijosmshj.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zemsyxwc.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2ftqxvthr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2zyonikdz.html

);
来源：http://www.52xcode.cn/Article/details/gt2cdizbmrh.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2omemlzjo.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2xldvuyvb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2vtxzegpf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jjwytice.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2wayhtbqw.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cvvluvzj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qyvxjzoh.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2duavqdld.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2zgchtjaw.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2pxzgbedk.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dodwknjt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2fstguyip.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2fsmtcpua.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2pltirkph.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2vexenekn.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2enlelhlk.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2yuykatna.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2znrhgfmf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2pewjwsqk.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2xswedydd.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2kjlpayrr.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2mlxdpykd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xuucadln.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2fibocdvr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ymimavig.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2hnfdbzxi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2igpupinr.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hoqxsmig.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2cjrprzvs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2drdwbkxj.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2nhexoqaq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2ejfczygy.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2zdakazhy.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2muvsoqbh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mywmfbac.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2simfqkrs.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ludfulah.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2xadlfdrg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tnizbqek.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qnbtckkm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2rduimaqz.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zdmfxjnw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2megdnqhk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ugxvynlb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2cjgrvcyw.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xlebjoww.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2gfpedkox.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2twkswtui.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2sszjywpi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2oavlseej.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hxrolmso.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pmhwatok.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qfvmczmf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2liltrifg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2gqlflfev.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2bywpcaku.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2znymttfx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nkuyecsc.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lzovffjt.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wnfopvmz.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zhcxhgnd.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mbhqqitq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2elppjxav.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xqwfujuq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2cxcokelv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ildehlir.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2fdhfrxki.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ijyfqdmw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qykqkcav.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rizwjfjw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ststilwg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2scytaqvc.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2qzjklumn.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nacjwfcz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2xqoqqfwq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kxaaqppj.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2mhmskshs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rdejpzms.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2epbmeblo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yagsmfwc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2osnssvxz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2zcucsagp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2txhrpsuc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2bikltxmo.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xoflkvvi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2murbtvrp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rzfbvbfm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vrmgfilg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ktomuymn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2qvfyrzdi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jwagjmkp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2izqewwvm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qczifeyr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2gzydxsug.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kbybkbdn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2enjymgjz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zobvcvpx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2tmnrlghe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xjaulqsm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2mucxaktv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2obeeanxw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2srjezzfv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wlejebqa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xoohxevy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jxjutbse.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2kduioogx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vpeyormb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ufhcyihk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2bheemieh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kdvzxmti.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2vrebgzqg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2wbapglki.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zbuoflsq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ffbraysg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jxotndfw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2akohmbjw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2qzugxjun.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2sssuthbo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2guwxfewp.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vqvihpxq.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2bpvgzhef.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2piwdndda.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ceybvbzj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rjgbgdpx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ppxbofrq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ynqlkbix.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ewxkhics.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2bxcmrtde.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mgedcdiz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2jdmauawk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qwplyosc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ydwuqotm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2xdnupmsn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cmbxtkhh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zfvcrpro.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yvjukdba.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ktrvrsjy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2adzxlllu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ibltzpzg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2jtpbthoy.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2enjgynha.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2hytkecbv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2jxcthuih.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2kzbsouqs.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ujoktgck.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rpfywuwz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2iozluskn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2odzfgrbf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qpkdauel.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2bigeutgi.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dtcgelyq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2elrmsgou.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kxusdkup.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bxzipzeo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkxflppq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2idsqncnh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ogufclzb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2qciimatc.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilzzgkky.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dyuulvgy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ueuckrhs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kzhzifus.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2iowsxpxl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2bnmrmsfo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bocynolf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2eedxdquy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2duprkrpa.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2gszkuweq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2dhwfwrmq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xorokmvj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tztidrzh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2sclzdifc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2rijfgpxs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yyqqxwko.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2anbmdxrb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dvcdgutj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mdmvqxpe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ijihrcho.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2fweowoxb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kmqitqmd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eeypuyat.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xbxehkzp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zmmldgfg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ylqyhgud.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gximdnjp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2hdnpkfhm.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2tkeouijz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uwjejcbn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xmrndmcu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2facmltpt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hidxzjcr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2jpwoxmoa.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycwehbat.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xipldzaq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yfsniwbs.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ecfwtftp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2vxnyuuzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sjgzvkdb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zsmknpik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bgncwlga.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2sgmvafgk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nboytgot.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2rdeskljn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qkxsiagd.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qgfijulv.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2gquhugxc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qpqhubol.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2eupggjqq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wyaqekxt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2sidhuuju.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jippzegn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2cqjmoqvz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ocdpjnrr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2djikrjmi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cltiwlqp.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qowhjnue.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2nifyjzew.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qeuhsyvr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qkrypcvy.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ampfofar.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mtifzgos.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2avngkern.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2vbhjztsy.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2egqecoea.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2abihkacz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2azotvkyt.html

esac
来源：http://www.52xcode.cn/Article/details/gt2unmcjrcy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2hketeyop.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2grzuhtas.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2iqemlfgk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vcvbsvjk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zuuwzxwt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2idrqqbxv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fvjzseez.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2kekeflpb.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ilnrakea.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uwdpygdf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hesohmxy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2rcxjcoto.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2vkzbndqz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2xwkagapr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ldlhpdtw.html


<!-- 参考信息 -->