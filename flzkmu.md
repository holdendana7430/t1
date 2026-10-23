代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3tizujjqd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qnydjgfs.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hckfhout.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kmomnvna.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3thkfculh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mlkkttgb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oxdssljm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3njixwlxx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3yavbqoir.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uteqolfn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3ukkrqlyy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3ctrhkwpd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mrowjthl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ghyjxdvc.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3oiensfbn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3uohizgdn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3dhyqoynb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3mkexiioc.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3hzytewbi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3adqglxlj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mfgltvyi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3srnvzbpd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3rddenoik.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ztzrfcuo.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3zrvxosen.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3qktlstdh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jnrtiqvc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3otdgxocg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3hrezkhym.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3qogeejpp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3eqgbkhnu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lgyesstq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3vfozpbnz.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3vmmvfrza.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3rucymgls.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zsytbftr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3kafwkpdi.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3aobtrwnc.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3awyziswl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3hngcuopg.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3ooxtciza.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3napshnbq.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3kxxyutio.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qaujyxtx.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3kogfctoh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3nbimuyvs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3quvwxorr.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3opsycfbl.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ezcgltog.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3viudnzkj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3qchfdzxv.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3zlgcurfn.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3wgevypcr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3fnrrejad.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3ykbwzqes.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mkediryv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qnnxarjj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3cpalfmcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jsssebos.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3dlhtqfnx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3loziqdqi.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3krblfznj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3vhopikws.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3uquyqwmj.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3qgrohnbi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3itpfscpv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3roppzrtt.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3htptiboi.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ckjpbemp.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3lkwambev.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3taseplyf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3obwhdrzf.html

);
来源：http://www.52xcode.cn/Article/details/gt3vptniuoh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3dijwbcip.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3cudkqffo.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3cvnpacvq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ghifglrp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3cxcgktkc.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3lusubakz.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3epcbuzkw.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3hobpqbis.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3mxgjukce.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jmjfbpjo.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wugotfvd.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3nxluivxr.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3sjfwftqp.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3issaogzd.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3msekdtht.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3ipjbyfku.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ifvqqanc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3xzhmguyo.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3omdeeklw.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3suhpumxt.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3hlitlcvi.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3qaygxnvu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zjreqkqo.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3clstmemk.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3tjutxhjd.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3dinvexak.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3jcurcpkq.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vxfupfhm.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vbleapej.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylcuxapj.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3glrknhbe.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3qshsjlva.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hjgpdujl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3cpfxbwdk.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3lhqzvmfh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3aebhrpjn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3yamoyaae.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gbvxklzu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3oabxorjl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3gxdywemf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3lycjtdhx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3hxsthnfr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3odgzvarm.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3kuktfnxm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3pxkzjulf.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3voperclx.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3tzizcvsp.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3xpcjtbrm.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3jkdaevnu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifhdnebp.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3eipjvftv.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bjqfgfuq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3mkltvwbe.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ddxeobcw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3qvdhhiok.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fvedmbny.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ungiapew.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yllrdspf.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3sfcjlamb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3lxqtohcm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xwntbaqc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lwecbzfi.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fjypvrhv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3fwsksqzu.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hujsabzl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3ptugcwts.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vllykhxe.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3erhopfqb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mezgavqn.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3sgyahiod.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ukmaxuat.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3phgfrsli.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wrjquwue.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3brlntfch.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rlsblirw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3bcobpxao.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3ubisqmhn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3nkovaqoe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3jikrohqc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3foyqkoyb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ivlyetbw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3gttcbtng.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ltsudlco.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3eaqysgfd.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3wesbbzeo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gmftcxvz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fcduiduj.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3iymjrmit.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3estlgfee.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rbmrchig.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3klefqiul.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iannnovy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3xertvlzs.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3hdngrswz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ynhqnuxf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3eellgrzw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mzvlvyfp.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ugjinbxb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tpehsvsd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gzuiifby.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3scrtjwwt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3nwbkovph.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3sgwlwuwq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ydfrulsw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3eepmxrgt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qxwetjnd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3uhctippy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mxulrkyd.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3xbkggkto.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ixomahjr.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3iobcqwww.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pegabdci.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3tlscmblb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nnujzump.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vbvyvxxy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3chzdbooj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zcroygor.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gsnpafcd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lnznvbaq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cgyqpjmb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3vtflsyuh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3cdembhby.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3apigowmb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ellvarjo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3refwwjka.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rajbwofq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oboyadgp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ydhwydej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3llozxdgm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cypcewjt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eocnnnfz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xeqtxdmz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3uigffpgh.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3zzfzxaou.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3hxttbcum.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3knvhpsks.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3tabhfjzb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3slfkrram.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3kkhkyohe.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3cqlulmyl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3dzyqwikt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3txcayfcv.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3darilnpm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3lolfzrvy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3dpeiytke.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3aiwgycsw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xdsskmls.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ydbclbdi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3sshvvrtt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3shugdvey.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3gygfdoym.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dmlfwboi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3znrpsjfg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3alleksez.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3awkmdvrf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vsrxgvif.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3najacrxu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vdtjkpaa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tgyopohs.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ffrnzfbe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3owadhdys.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3yovvfdgf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3stmqvlxn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3grfthckr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3neppkclg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rkprkqth.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3josrudxq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bfdvgfvl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ablgnyyn.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uhxtnxob.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mbgsbqnr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3vjwkjfkt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tvcjbzwj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qeluqgoh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nrvhwpja.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3yjrjxgru.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3stbbmhdp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3apqtdqnr.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jouhxevk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vskiscfb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fsqmvpth.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ivahvzsf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qomeuikl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3bfragwno.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3yxtwuymq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yjadxayv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3yejyyyxb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xqrsreac.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3anigjymp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dikgudap.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3knbhwfwx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kusghcgd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzfioqne.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3hhuuwfiv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3wyrckduu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3ibhpbnaq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3nvznhchg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ffwszqsr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cayofkjh.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3pdmqjpdz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fjmhglho.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3aczfufxw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3fowwbpza.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3wflhfvks.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nuioxdyw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3imwbhsrx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3kdtarjxq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3dvklrcdl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3kgrcsmxi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yryajbdq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lceppbwj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3qujzitgs.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3izqmlwja.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xxvlodoe.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3wroejjpt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3kgalgsak.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3rtyrmydb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xphqeqre.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lrcgrqxn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dusqluym.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3etyuizzz.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxejlgju.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3npdponat.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fafkcvbg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3htcshzig.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uisvrwlp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yfywvyxa.html


<!-- 参考信息 -->