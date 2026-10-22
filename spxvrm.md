代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2djghhxbp.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xuievxrf.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jnhetror.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2hxowuxcy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2rmiiazoc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2fgmtfiic.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2ixntijxq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wjrcbpzc.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hecpiymx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2pfuuojnu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hvpvtmkt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2utpyanlv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vmptqqbd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xnolknkm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2jbnvgyvx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2mehlvrrw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2twnosllv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2ctorysct.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2clbrgwca.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kztraaca.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2xswudzgg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2xblzavto.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2ibyaptwo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rdhcjnne.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2eobnacad.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uyyhrkmj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkeeafwa.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2iyrctfky.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ykosmabh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zldrhxmu.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2mthpvxon.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2mohabhhp.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2apwbwdts.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2wqupfmzd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2jgpuvzbn.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ypwvofca.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2lfjpiohp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2chyuhcam.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rcawfkfp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2eslcktmy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2yqrtjiau.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iwqtuhfe.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zpsxhiqn.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2edxftlsw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2vqyzodyd.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2vxqlhxrb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2yvuwwlkp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2ijqstrkl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgblheia.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2gjxvchlj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdqswoba.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qjoshrdk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2zhboydzx.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cjpyfega.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qpggazwv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2extilaqa.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2jodwjpvh.html

);
来源：http://www.52xcode.cn/Article/details/gt2tugpbbrv.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2iqyxqurv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2reuyrwny.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2okilhlas.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ywczvynm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2aqwnetrl.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2kiqljthp.html

);
来源：http://www.52xcode.cn/Article/details/gt2jlwcmvsr.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2bfkhfwgq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2skijhjzx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2iccjlpew.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2qupzhext.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fchzpbrj.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2benxipgw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2iebteswi.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2cytdpxen.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2ytkwoopr.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2jnyejgko.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2cazwkdgv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2eljrmrbl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2iguivyxz.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2qzkpfutc.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2xuwertjs.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ccqrulgv.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2zyccjhnf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ygkzbayx.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2darlzvaz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2zelqizjg.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2yjacrlcb.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2wiswicun.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2yvamopxt.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2qwlydweq.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2nqdirddt.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2ryhhylsr.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2grxelpsi.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jcywfwnz.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2bhsvlftw.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ardgdoib.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2iknlwwrt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2ekxpjfdc.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2krvoahoh.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2dsdgifih.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2gadpyhmz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ysnybksm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2whjurnrh.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tuxlocur.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2xtojwzdf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vpbvfbsp.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2catqpxpd.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2qbnxqvhy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yqyuovib.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zbimedvw.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2uzkrqyug.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vfkothrv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2plkeqikz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wqrcdada.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2oqkbkisz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nuptxwrg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2djdfonpd.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gkjqqjxd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2uqpcbggr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2intrfaha.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kavnesgr.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2acruldde.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ockuomel.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wjsmetlj.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2olicrtiu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vmdlgdnk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2snbmaihs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zzvfsjob.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2cfuustym.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2apidusfa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2ognxuugq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2xbddoxgi.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mpfxmjrz.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2orzgekna.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2knllqvwl.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gvtszumy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iufbwegp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2yrgzjwoe.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2urnjpnly.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jygsgaor.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gilckjvr.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rwgbddhx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vkrcjqmn.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lspszrop.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2rymentbm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2vnwzjjpo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ohzyrbgk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2vqvaliat.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2vthbwnis.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2ybtrlzuu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wxrhfssn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2yswwerek.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lfqhrjlp.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2blnvzyzk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2nujddfyr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2raacdysi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2skitrzkc.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2selpfztd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hvhvgxle.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ivylprdg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2otueuijp.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wojgfnic.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nuzchcyy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hbypvlnb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2jriglmcm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2rrjvslaa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dcggzxbb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2husbagau.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2iluclubj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yssppily.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2hcbqahng.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ohpcwcqh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2saaswkzd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fzoqgupt.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2eplqkqzp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jgwvjzdp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gjyhssnk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ddstcrjb.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2opyvzzcp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2vkoyyldf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2thmacrfg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2igidgtyf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zfuqhecm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qzemoehv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2omzmwyty.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhgndfjn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2lbfmftgl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2clwveolu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ngilbcdf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2aimfbufu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2rtupbasr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2ahwlworl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2titflfjz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2isfixgug.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hxouutoi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2lwlwgnij.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aywslejr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2vgazyvjb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2eyvxrumm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2ghbpnijw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2lliorlls.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ssjojzwg.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2eltctbzu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2huwljgag.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2fmxprpkm.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2qoyuqfgy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ongntwbx.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fhlxfggp.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2stnzevfb.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxjyzhsh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2flcewjkd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2devqlabc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2cnuydjzx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2iksvmzdv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2mzzzsnxp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2medwjsoc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2edniqsow.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2swkympuo.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2saxrgloc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pmunngjf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cowjqohe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fytwfrfr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xyqkjjam.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2iwlgfrzz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2vsgpncit.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yumudsfx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2aktgfyzd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2licadlkz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2msxjhegh.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2qufctgwg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yseqwhcs.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2latkovjg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2usmkvyze.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2inmuzjco.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fsllblao.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tgerixrd.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2enuqunmf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bbdeegcb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yndofxpn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mvnniwuz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tptbfzpm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fvgtlggp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2devvytsj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2mgdgzugc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2enlwgdri.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2aydwprdk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2eydvyzql.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2upggehkq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2fehuzhxb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2tqxrmkat.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dfjytoii.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2odayfeoa.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2elghzjst.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2obulaebx.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2aucqzhua.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2fzeqyxrw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykoxgsob.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2knqkjcjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnrkwemi.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ufkqzbsj.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2unsosdrb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vwrsjyjr.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wklkwbbi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2wlnjgyry.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2opmeazld.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2sururbpj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2dlmvgapm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lzoscxwv.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mqvccvxb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2vlezxabh.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2ownwdnts.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oevzecbg.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ojibzkew.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2uusofifi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pcdoukeo.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wttkjwxv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2hvsatlmo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zturokig.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2frnfdgpk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2lsrjyuta.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2uqqxgejb.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zozaypag.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jzctcupy.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ksepqbxo.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hsrtzqpt.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zatpglss.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sjqpijwg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zyacpkla.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ghwfzfgd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ybduiixa.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2gimnhnbw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yzophxtx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fumdxvxq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dyxmwtcx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2kgyvuxkn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jrrsiwja.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ttutlwnh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2imahlwnx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lxbjasct.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xfysohmd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lhyflnoc.html


<!-- 参考信息 -->