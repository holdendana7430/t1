代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vbelajyi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2swhsvcxb.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cotvtwii.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2vavqhayt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2gccmzsqw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cyklyjtu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2utvppowm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ftkdkfux.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2airkofht.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2jhwpitsb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pzspysjw.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ruwtavsy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2hfprlvtv.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uglzzuck.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2mfexvufr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nskclvjn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jxcednlv.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2cjlgidxs.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2xbtdvinu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qqmzopbk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vauupqtq.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2thfjlfsr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2oivrklxi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2wtjwimhq.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qtlndnvc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ltbjgiqe.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ijvqwsyb.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ochnemlk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2yozodchu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ozxwweza.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xgbzfbzs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hnukyrst.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zmrowmce.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2glkmcidn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2winmpkde.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2rtawbcgn.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2uyeqpacm.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wiogiexn.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2clhkslbh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2lgudatvh.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2kzsriwah.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2meyfiufn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2ultpspqf.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rmzxvakt.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2snbyhefg.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2tcudxbmv.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2esrdhijo.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2xrnjnaoq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2zdoomymn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fejpobkn.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2cpglsfwy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jkkfkgob.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2wsrdgobk.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2nywaiutf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2ekndfkgz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2npvhluyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gtrofflf.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lgmyygoe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulmqvrxh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2fehtejtz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2iodwpuvz.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2nvfeioob.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2kktajroz.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2idqljipp.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2veikwvbb.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2ckhxpjwk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mprjcnxv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2hntompsu.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2tpbksatl.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2fszefxny.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2fzhcfkjr.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2skydjzak.html

);
来源：http://www.52xcode.cn/Article/details/gt2aoaeigto.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2hgjyxmzq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2frmlztet.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2rbgbddds.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2pemurohz.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2ubmytfny.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2pjuzelqh.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2qhcvuzru.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2ueboevxm.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2bzvyaemk.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vsvqvtao.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cjcjhvnx.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2xotgbdfl.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2uzdymqup.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ydmilcyh.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2mbbytrgh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rlzfeahv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2opoefeqj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2xqxcvfwk.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2thvfajmk.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2oyeyyqof.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2cewsiciy.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2nhsinfru.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2rvnvuasn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rspunzzt.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2rwwnuloh.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ghmxgnvs.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2feksluck.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2unwpeoxh.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2xamyzhmu.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ydejlpfn.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2qzqajyuf.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wrevrdbu.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2ikzwqlvf.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2nkbgjtbq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2ynlcxfig.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2bnbgatnh.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2xupgfkhc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2vtskllms.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2couxemft.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2azocggto.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zezufusf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qekmaeem.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2rcuurjiu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2tvhslbsz.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2nzbuueop.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdpycozj.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2kmpoxmse.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2mtdxwkbo.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2vbtonchh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nboyhqzr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2dybvdtcs.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ngwabqyl.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2dphthfge.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uosxblro.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xxokfjiu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpwnwojs.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lfywalup.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uoghuvma.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ujanijmo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2hojcwtqb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hgznxuli.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dmemgfly.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vienjxyu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ffuwdecc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2sfclsiyk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ermcuooj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ngaackbs.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2louihupr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ymcqfppp.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2igmlmzva.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2beaglrsj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2epvpndkl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rhemfxfv.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2bnplhhaa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2esveatbe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2niphngqu.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qqkifsqk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2hoiojysr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2iifmzhai.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2rblypfyk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2prmepitm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2hbzxhmgg.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2nkmfvgxu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xcfuscqd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rsuepgxa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pzrurmpm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bouwkkkk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zogoycma.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2olmqisgj.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jkgfnwna.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lkafrzbh.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ykndoyob.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2jgsbmijy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2eucsmaku.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qbnxrxxb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xjuuusjl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2engbqnxp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2llxtcgmh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2xqktvgys.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2djgcmoki.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2blajhfts.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2akkrvxlg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2pwzmrbdb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mxglzihh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2axfliing.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mpqfaaxd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ysdkqpxd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2yozmjayk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2poawuhkv.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mxvgzsnk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2xoecqmyw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gzdihdvd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2gwjbfmjv.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2beoidgpe.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pmmxtudo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ihgncgqj.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2eszogtxp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2sqedlfcc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2fcbzxdny.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2osqllnhg.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2zymmnyqh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pyrvpksk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uzqmifbo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cjhmamec.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2cabxsbbr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vsgaalsq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kqdbiigm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2phhlituf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zookczwx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2xlmsnlbo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2uhoapjva.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gifigbsu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ywegmcgy.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pwuojrmf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2shhzaito.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2kochcnqb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2lvnzxjit.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2abnzkfbs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2lhvqslqd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ywtpdhxi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2clncdhwb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ytcntryk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ubquqegj.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dmvzeckq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ivavsnyl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pujfnujo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tenocvcv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2igamkrdc.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2srmkplgq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2oetxdpcl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lnyxjjel.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2szwmxnnl.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2akccshge.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2azquiwje.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2wevadvdu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2xnmhydhs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sqxxiemr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gtafmmga.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hsbnikqd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2oupsmcsv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2rjxbsaoa.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hbnjhent.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2cmfrcsgl.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2buvcaxsp.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2rhmcqhqo.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uvoyjazx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tigcarqa.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vuyynvym.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lnzbggnp.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fjyhethf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bjesqkgj.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xozmjvcq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ficlafog.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vkrntiuw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2udqzcdmx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fwexxowq.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qzhwadnj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xsnqvybu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jafuyuow.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ztkuwtga.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mewnkcnb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2tnheohde.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ftnwqxlf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2ddpaodbh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2xoiwzszf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nboohmoh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qdrzmsnh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oerwyiem.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xtmgppxi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kmlrlmxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xwtjzslg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2sxoudgti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2idtcazbt.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ltajdmfp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ipnjalla.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2rfhqpeyt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wxsalrac.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ahijtxfq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2nkrmhbgc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2bmmovzdo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2tojdbczi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zwtbdsvc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2nqlzqqhn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2mnzviqip.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xmaomjln.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fzgjpcdy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fmhfaugt.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qkgucuxw.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2prmucqlu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2osjzhppz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jsluvsui.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2vceppnzl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2nzwyhdix.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qrdoahaf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2nwabbcze.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2atztnywk.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qcpsxjcj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2meneside.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2erwyzxdc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qtqnupvp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sqwraxha.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2saguwnay.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jnutewbw.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2evzgzeop.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2eyhrfkeq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lxevcrkq.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uxyrfjvj.html


<!-- 参考信息 -->