代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2tsxmetey.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jfitfvde.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2egebfgcj.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2udpmrawi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wltezqdv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ifdtmqyz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2aqzhttgr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2makntyam.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2brogbbmm.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lzsxwpax.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2udgulqcq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tkzqtwmu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2uyiwpiej.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2rywddiyn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2bvqfvzcd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xhfmkagr.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lfmsjmzm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2wzbufagq.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2kjhhpioc.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2eztavsso.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nxxafvuq.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2wrygldrq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2zwophhcz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bcosufxj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qkpkovwa.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vedtyzwr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2kmccncur.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2wewgfeto.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2hbciahgh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bpnhnjnn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlhevvog.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2mspbcain.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lluomcpc.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qkcbtffb.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2aoxwvqky.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2hmzlmjym.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2owlylygc.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2zvhjvawu.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2eapjyyfh.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rhlriihq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ajxcwuab.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kfyfaqlw.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2xafffsrk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2avyixhqs.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2udqtaqvo.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mvklabxd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ihnjllsm.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2ucdiprsy.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2nghcbixb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2vkrisevz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2glecwhcj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2rjzvozpy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qokpzsvl.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2jdtrxnky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uklmuyah.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2jiarsbxp.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2agizyzdk.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qzopoeqd.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vshlvzuq.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2mfhgudyk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qmwvuitd.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2tugiifbm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2khvhcwql.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2knlebydm.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2ljzqdsih.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2wpyhhspm.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2kjqarbbf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2lhxdgblr.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mvxbrksk.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2xvjhuzfu.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wnbkcytn.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2opejblvq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2txbxqvpw.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2mamkykry.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2roccmljw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ssdatzmy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2uuvjybwp.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2kyjvwzcp.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2hyqaelao.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2xoyvkojq.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ecukiffl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2thtqofek.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ximejeze.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2ntwgfitk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sqdzgrhf.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2wjizfxeu.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2panooimt.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2nzfjyorh.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2hgjdfjja.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2bxdmjqmn.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2jjyrirum.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2sccapofh.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2piwegopu.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2ysezfqps.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2ccgbciwv.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2ohhurovc.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2osdvyjjt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2mmjxnieq.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wxpwpybm.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2yvaqyfku.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hwypvlri.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2gtosiavb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2tapvhjlh.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gnnxtxpt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yjdktwlq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2phuefosq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2igcgpzth.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2jmgxhxri.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ckrplprz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2ypurqvcs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2exvdamut.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2sckkommv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2syelahso.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xvriqnxh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2anwlkukp.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2pzzyjyrw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kbapwytd.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2ciotansu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tbjfpnxz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hxczlchl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cewwqhkd.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2jvivnfdx.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2rltftxdn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2hspukhje.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ikgguzdf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jjtqhhli.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zjomgxuo.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qokvdxit.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mhdmibod.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oqeptgac.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xrwspmcc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bjnneuxb.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fywcdoah.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2tvrxevrk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uosxibeq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2spkdegcm.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2buhyzvji.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2khikrkiq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2glxnwvws.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cutdawdp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rzqlzfmi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rqcsjweb.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2brazvzqt.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2bfyxzrip.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hqskkagi.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vqqggohs.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vnmwzenr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2nxmokpvm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2otgyahet.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vbpnhyrv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2avpwskzw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2anwnbmku.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ssqzrxyi.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2mynkisjn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2chewuapd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qevxtgkp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2hloknqlo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ixmrinwe.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dxxakmnr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dynvkxru.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2omvupgxv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wsmhvfyw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ubnoxhbq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ervlwbwt.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gjtbknrk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2aludgsaq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2njwzqkbn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2rpbanjmy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rizhljbr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2azoigsca.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ngatrmmi.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zmysxbue.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2olnzlqrg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2gmpadtdh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ftgidhbd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2jpvhrjyv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gkpbvmaa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2plzbsjtj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2crgwxwmj.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ykrezcnr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2opqdqbgj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dcqtihwn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wfkchpfc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2wajzwazi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ncymcxbk.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2ascuuvbp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aopxzwzf.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2oreawhaa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cffidvno.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vccdtfos.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hgmjqsdd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2rrotfrst.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mcflunil.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dgoyhpem.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2xpdcjtfe.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2stciafsp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ftekdmlq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2drzzrigg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fdtmslgd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2prokhfcy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ptqucqxc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2mfdfzmjp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2lxmjwcrn.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zhdecykk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2mgaoqiic.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2udsvkrcf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2prkhccau.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ntnuagfp.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xxxbufpx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ejlzjfui.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2hyecpgef.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2kuxxtsoy.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mlhtqowq.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kthejscb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2jrfwpeam.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bfmsgzhr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2trfjaazd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kmukxtos.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2vrmpuyfa.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ojdnbhuf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tsckyapx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ohadzsub.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lhtdrtqy.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xhxubnqh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bycdhqwl.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2jzrnsmfy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hqqskbnm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2graaaccl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ywrgepte.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2rornqlgi.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2xgttoqtp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2sawcbzed.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2rjgoecql.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2okgzpeon.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qhrmcvwa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ewybslst.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xntaffgh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2impqiztn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uqzgbrbj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dxfumthl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vcuyyavk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ilkardct.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2uzckthuc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jsegywid.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ojatlaaa.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2htlvvmri.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hagwaynt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2nwgqlscd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2lqzhjmkl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zyedrznu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2quyndola.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ttwinmor.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jagwpysd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2vuvruslq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ciqewhor.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2tnyzwsje.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2medvbpny.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2auedmrov.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ewiiqtsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mzkjthno.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jtiykzhc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qeyfknue.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2scpdsgpm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jmqinsks.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vmkfisnr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nkjvfzhy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ohmotnlc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2vnpidiyi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fxpzxueb.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ruguadok.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ishrpepo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2usijmcyt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zpwsafvn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wwoxxdcx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uklfmssp.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdijcjdp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2haesxvdy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2isdijuit.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rjycwtmz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2junncllt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2prcvgqlc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2wbpybhep.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kpbxxbkr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2dkmislxl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ssorsdlu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uwzspshq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2qotyvzfe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zjjekuid.html

esac
来源：http://www.52xcode.cn/Article/details/gt2gixjgbuj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zticllzc.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2jlozukmr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2nufcjxan.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2efyvvvta.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ddsqkckx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jpfhpuxk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gicxpnvg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gdysoxme.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2gyrghneb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvyhgixy.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2phfrvetj.html


<!-- 参考信息 -->