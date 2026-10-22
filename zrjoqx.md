代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2cckusxio.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nahcxtfp.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fyqdiinp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qnqlqyuy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rbwyhloh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2srtalrpe.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2ezljmbot.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2rvxobili.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2vvesgnxe.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fxirdpjq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2awzznbtc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fdhpirin.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rpooqmwp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2avindmvd.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2qvxnohki.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ouofvggm.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2qcroyoek.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wydidprm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2lvavghgx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2aqovyjgv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wxbxolve.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2chzsmyvx.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tnkyypep.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2paohxktb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2bwlwhmgv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2dckdvubj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kkdvrksw.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ixnimiir.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mpvwzmun.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2zfsdvyvb.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zhnxdott.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2oaoywcln.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2plmpzxhv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2uzmktdgn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2oybxkjlu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rbwmsuds.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2scgoaggu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ctgrghxt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2itkzadfe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qbvfwfjd.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2hbechanc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2qpmkqslw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2wshdsuma.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2vwzkwnzn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2qrpqixxh.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2pdynyoeg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ykxqjllh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zefoohux.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2jukgsftk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2vucqydtc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2pcsgyodi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wconctrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jsknufno.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2yjtsnhox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bmtwajqd.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2yphsdsdi.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2blowxnng.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qvqdhumz.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2hbrpyayv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2jvbergkd.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2imfiwxxo.html

);
来源：http://www.52xcode.cn/Article/details/gt2aheahblw.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2busbtbbq.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2mdzkvunr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qjxbxlvu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2cwinfzde.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2sqlthqtk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2xlwntfjs.html

);
来源：http://www.52xcode.cn/Article/details/gt2rscesuam.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2nvhjbaaj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2awyoddiy.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xytfypui.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tandjbmk.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2algqcmdt.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2iluquhoq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2xkkupugb.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2hggdjqzw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2frjfnuep.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mrhdygci.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2hxdquctt.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ptzdsiqg.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2vtezyvts.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ymzldspg.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wmptgpdz.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2bobbhrav.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2ghiviwxn.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sqefjotn.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2wzhlfown.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2rquecdba.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2uronuzdz.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wucoqgcg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wcrkwlfp.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2egnwoanj.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2xvvmzfef.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lgdyjgnq.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2duviuvsj.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mlptzqpd.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2yckcemzh.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anvnswxi.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2ajayrbjn.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jinumwen.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2yukencws.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2xbejpsby.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2afgitaii.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jlgolrtp.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2crskrtem.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vrmzfbze.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2mefkhdwu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2aefmflcy.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fbudrary.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2merwoldn.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2oybedkvy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2agpwuyas.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2siezdeao.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2idespyyk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ivdrivbc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2lfxwjbbt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2vxgmmsfh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tjlyihbn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mimlkuvn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2flasmqes.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lstfdxst.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2yryaekhn.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2zvgftsms.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bjfymotz.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gjpxvher.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xijqzcev.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2vmrtuegt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ouleiahn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2enkbfpvy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2vnumwqil.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2oaqnksje.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ynfrhofr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tssyshzr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2dslhjedr.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2nxfhzijk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rplrfjzk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zfxcchzw.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2amqwscui.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yhcxicyn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2muxjvoja.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xpujgaoc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jyuoetjf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eyjemxpz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vescampa.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2yzjjcvhr.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vfpsxyic.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jfqetshd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2sprbhhfy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2headgpxf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vskgoehx.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2codlutqs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vvemzopx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2nyblsbkw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2obctyoxe.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lqrryosw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2nwxfjrre.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tsoszsue.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lldgrwsd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2eimeyvja.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2qnqvtqej.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dovgocft.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ejwbiqdk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qxdvlsxx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2mwlaahox.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2jyeljpvt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2clezzdnj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2uvasgklo.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2ggkmkfdb.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2dwdpgpkd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wchtevgw.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zlaflebn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hsqzjxwl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2apjtntfe.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2heeeguas.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2uolmvqjy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vpxhweji.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xdvvrydw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2xvwzruht.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wuyyoqjv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yvzpmthb.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ogllwjqi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2evrnkfsy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zsromdkp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zyhytygr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nftamlyn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2vhyflrxz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wahckkws.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2djymryws.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wovwqyht.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wzgnwinz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2qvjzsjst.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jwrwkufw.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2wkytfthq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2lqcjoysj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nqjnwkuy.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zkpphvxt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yfvcpwor.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rjemgsnm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2lxakbnmi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2jlvdrlgm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kqjjmhmt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2indgqzcc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2kiifesaq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2aeyloloo.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rxbatvjm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2txfhipnw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2zdrxzpez.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2tfeuvvsz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2yrteegcv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vuwwrzoy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ussfurpi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2vymmzslw.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oguxnulf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2zywdsmhe.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2xjayvydm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fptiviun.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ywyrlzqp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ggusemnb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hxkwbepr.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cafpigcl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2kiwaqnlt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2bmbsnylg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mxdhnoxg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2cldajlsw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2rhewstdp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xykpuzic.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2ynentqca.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nrcecrao.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2idkhqdth.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qleahvor.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2azmhnxvq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2krzhykgu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2utfpsdwf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hyehfwip.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gjuzynqz.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bvrncahe.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wwnfmkdb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2divcrext.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lvycblrg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ibyxnlpx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2siuhkqsp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rwkxjwnf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aqnxairm.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2eranyuda.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nwonsyim.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ofeziyqh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2dxfdjlta.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xptislen.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jzoujpku.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ykirawtl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ikajekow.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vwiyjlge.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2cbcfedsp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqjkrmuk.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hkzvpseo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mumdnxoh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2nmndmuhp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2lttequan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xlgstvrb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rdlbyqkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eqqosbfc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ilmbvngk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2txtgawxy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qteszgfr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vkxblsci.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2apaddlie.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ieurzfzx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ghfdyker.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yqvmdcjf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2bsoiauzi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2lbcniewp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yloeglzj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2owdxtcie.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2dnfvjskg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhsbovps.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2deecupgs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2rldkdcrg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2qwfdbyrw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mfidtime.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2dmwhiago.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2nnwhabof.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lwoocqfp.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rxaghfwm.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ejzcmien.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rijstewt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vpxkpisk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2kvdcsfcm.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2mqfvjwff.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnetpuzi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2dsxvlerb.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2czphkrry.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zibwrulr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jdpmbejg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gykkwllt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cngysfmj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xbmbssmk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gyosjumc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fsboavwe.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2eujnmajm.html


<!-- 参考信息 -->