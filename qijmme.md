代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2bajlloqy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ezqcrsgv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2bkqqniah.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cnjcujok.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2trpuvtxt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jvmaxkan.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2arelnhcg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yfpevksa.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2okudqjok.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2pytmgnbm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jljsumfm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fbsxudlo.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2wcnujqye.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2aunusmkc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2ywwxhysd.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xeflkqse.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nrzakylb.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2fpzjzelb.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lrxjtmpf.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xrqhbzhe.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gzlecekq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2knoqdffn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2hbgkaoid.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2efiqxlge.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2xybzhlnk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2hxuwrugv.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jrnisbkj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlpxvdrt.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qlcbmzqd.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ueekoawk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2jqvvsbnq.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2rvmwfunu.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2imjtdfcu.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ohsbvqgz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ebnjpjtl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2qbbuoovu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2lbxufvwf.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2udzloydc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2jdopncxh.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qjebgtqb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2xdabpysd.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2foiakbim.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ttbwuohd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2skbxhinu.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vccehjcw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2kxoywimc.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2chcxydyb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2sqwnlhww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdkndkih.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2tlcduiwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnjzobvp.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2zvbjygyi.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2cxprgrpy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qymdknvn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2tglvttlv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2hkfzqbdq.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fdgaqazd.html

);
来源：http://www.52xcode.cn/Article/details/gt2oojqovuo.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2naliefje.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2gsjbilud.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2jzybvsll.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hcgvltah.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2etfzwrfc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2rrcvnbqr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2cukpkfqo.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2eihsgjil.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wqvenisl.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2xvzxbozx.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2nqzxebdn.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2efdxlgzj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2mnojukrq.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2yhtqpvxr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2gdpwezcf.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2pkaesckq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xdqkhfdr.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2rwokhdgb.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ybtoxqaj.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2wsslzafx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2hysnpxqh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2uzrlksfv.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2tuduiimf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kvwprtqz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2qnrxnbto.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2jjjgwygf.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2kdachgkt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2ervdffhc.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2wkjssgtf.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2snuxrpqk.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2ftcojtdr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2tfinqbqv.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2nawmcelp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2iglbansd.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2txohrplv.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2ximffpnb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tzbuyrnp.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wunqevjg.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cxvxlouc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2buriclsu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2lhstioda.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2usmadigk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2lqtkzher.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ckbnikel.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ovrbkpke.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2fcrcsbzr.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2xhsrgnsv.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2iglbguno.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gdbbmirf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wnyewods.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2hztknmmp.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2srqrwltq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2daxeiwmb.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2sjtjdjds.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2pdlwdazz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vdvmyuss.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2necolgrq.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2cgnzqnjb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rdmtyciw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qmknwfbv.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jhlneyzt.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2qijrtxbb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mwhxlinf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2dnwcdhca.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xtylfslu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dbtgapog.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zhigcjqz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2orwahdsw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uapdlnxk.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dybkprhb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2stiodddh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ddegblxj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2neppsagi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pdfjttaz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2sirnbidx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2htpukcbx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2brioysld.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rsyqxzvf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qizaimwv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rkwkdomi.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2xnxtupem.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dgopcwgq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2looqlpam.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2edodketb.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xtjqkdjf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jonkucoj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mdmlyntv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pnqhxjzq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2ntxmlapf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2xqiedwsu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2msngfsno.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2puyfoqyn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pyowytpu.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kekojbxd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2mwubpjbm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2huygyron.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gufubbmd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2owkeczwn.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wskbjvfk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2pzngezuy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wbdkrodf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bfrqsxan.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ssehbbve.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wykqnpsn.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2czoyvmjm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2rsutvtle.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ammncqyk.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lviggbgi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tbrgnwho.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2kwrjbgpf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vebcjhym.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2haffnask.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2fdoygpdh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2rzwrrubt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2pzlhjieh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2inmunkht.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ufopaykd.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2joxwkzuu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xpsefakf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2wdmfpuqc.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2zrowxgpu.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2usfkyacu.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ymemdseq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fhunjcto.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vzvrlnrc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2iabtoraw.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2txrfznhm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2msgiljia.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uypnzror.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2lbaywfws.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qcdcuoay.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2flcregrm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yvirchha.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ggvdrtic.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jvttqexh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qdlonpdc.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2pqdzsski.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kxmbkfhi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2aucyhzco.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2bkuvjnlm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2nshlsmmc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ltvqbpcz.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zzqolgfp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zmfhkfal.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2msvegppn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2iuavnwqn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yfymgntv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2qqxbpfut.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fneuelgi.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bkihhphu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2imrizdxl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2licueeiz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zgeuxglj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tuztnbag.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fiytoyyu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hgxyqcha.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rpzznsmi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wualovkj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ixverufh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2djcztecv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2umkoxqmz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ijzgldne.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jnyzglsf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qxdgnsqu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sxaztdwx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2uwzbsfxd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2bgtjttzd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qjtopfqy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2aequalfu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2biflgthc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ngjdpbjl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2syqmlsxj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2mbkxyrzp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2hsgutzvg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xdvndawu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2okeocisq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eqaouyhk.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fncitfas.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2werierhz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfctkkhu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2stndggcf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hzfmvjez.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hdefzheq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgxvrytg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2mjsukafi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ynqbebqc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kpxrpejg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2auxzexao.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2dwrnrmhv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ffkuvuqa.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2cxzscicz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kwsgkqyx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gijskudm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ltbcicsk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2yhkzyubs.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2sqhgdfes.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qvxwkwlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yepqkzsa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2wlxkrehp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aezyclyz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2onmuwawx.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2xfdlttog.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2grlzzzww.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yekhbxvw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2uglsmzym.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2kadfiijg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2sbvxolkl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2pfxrsnbx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fzghbctp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2uyypqulp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2knqvsysy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mtnpielu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zszwuyln.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2qweprmwf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2orqtlncs.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2iraiince.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yxfqmvey.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2lcyzzaaa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ohcxaggw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2afywfyse.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2wychglom.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vlnlyeqv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rdjwtcsl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2lkhebsvt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oiutoeum.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gthmakqj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2vfnzzipc.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vhdstbor.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wbircetx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jaaaqyrn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2anhdjawi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ojsydiei.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2wohhemzv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hrbhwgye.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2njkgzqwo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2quwiyaxz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bepjxbss.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ruwuwadt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qcnrsqlq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2paqudluh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jbjjiybw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wditwgic.html


<!-- 参考信息 -->