代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qmyuyoul.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3vkayuhqa.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3uheefwun.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3iyjqabcm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rhazivkd.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dktttrok.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pqhmxmjn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3cgygwblr.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hhtdoqnj.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3lpictxoa.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3haastgbl.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3eefmkapk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bqnddiav.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3ylvrqnjg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3pvqcltda.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3fcccntev.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3xguxwpoc.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3tnesgrcz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cdcnjymg.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gletgppz.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3bkfyswad.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ablwxcot.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3jktwfuzw.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3kdyrapyv.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3lcjfrbyp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3qewbacgz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lnpdqdry.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3bqsffzoq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3wyawepsm.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mwmyidxm.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3hbicslnu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3wxpnvwoi.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3eisiwhrs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3lhtqdzim.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3hypjvurl.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3zxlfzblo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3mnvbwevw.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3tqyscktl.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3jozreell.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3ulfktvdb.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3cywjruga.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3mcamtnom.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3mhjaqgea.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3oddhaabz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3tggkzgob.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nfhqtkxs.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3dhblzoip.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3lmnavjja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hberbeqz.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3pjbhzjuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pykskwuk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3xoqowhls.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3uajiapnu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3wmtzzemj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3cspedlyv.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3xtehaose.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3qgbgmssk.html

);
来源：http://www.52xcode.cn/Article/details/gt3fjuyqxdm.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3wlzezozv.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3duzctxkh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ngwyksqr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3eyormthb.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3nzaywxzo.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3suhceesg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3wtvbfabl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3tuframzw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3fzguavfx.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3bdsltxvv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3eoqvunxy.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3xvddzjfl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hrnkvijb.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ulanorzm.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3nspogpjr.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3nctvgtxc.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3kjbqvdtq.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3gmouuqfa.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3tuockavh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3efhxuxcr.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3linrftmj.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3hsunrcfh.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3aamnhymw.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3lghcgasa.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wjywfqyi.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3booktlvg.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt3gnblblen.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3xjjmsrdy.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3owobwhsp.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ostsglax.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3oqkfzpil.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3eeludfmr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3dbuldqzn.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3rpeqapsr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zmcijcfp.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3tcgfakiu.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qmacuizl.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3infgscft.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3gzjmufpo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vbgmjutu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3yogxobxq.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3ugyhygvc.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tjdmnmks.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3zcfepvqx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hacmcvkv.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3exikdopt.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3xccgpsku.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3raapoicx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3bkartwxc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3uahriooi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3voquyffr.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3uifznjav.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sseusntv.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3edxejjei.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3dzkufrot.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3qxrshgld.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jlvbvtmm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3liotjpnu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bwfjplki.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3yxlljuam.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lnpfkhbp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3brlyvzzl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qkaagzpa.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pkhrpfkz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3hotslczs.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qdwmkudv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3qcoepkjt.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rkrzmvsl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3udmogzck.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ioylxgot.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lsrrelrb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3jmsflfhk.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3edskkfsu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3atldvdzx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3qglxtspo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3necsepcn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3eywbhvoc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3souejyki.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3nbcanvoy.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uypgryes.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vcodyvfz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3lbuvyzoo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3bjuwpckd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3nbyhehbh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3xwldxnnm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yipbxvny.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3ygzwhunb.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vlncccoy.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xovggqcy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3lgpdkqto.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3utllmsuv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3rjngpaqh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vrnlyjdu.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3axvvvqxx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3ifesewal.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3epehbjlz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3flcxsnox.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3vjaqwuqa.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3ogweykqv.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3zxkgtlcw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3zrozbcqx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3rbxrsgyd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3vljuznwh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ppkirsug.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3juzxjufp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3zzgypqsq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ypzrjcfm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3sflevjjb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3mhgnknvg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3gsefvajb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3tdsjhcbi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3owdxmyxf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3deujgodd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3mlknrgrx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3nsubynhl.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3teqlslzb.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3socatpzb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hwilobpy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wftmwjcl.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3hdytejgr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3izybznwo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fqhksxdc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3btjlkgig.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fipvlncu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3tfltznvr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3zawnaafb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tddflkcv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pylggjyz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nmovpfty.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tpvuwyjl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dmvxwfep.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3pcseisdu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3zncfvwvx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hvyvatna.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ylkxvbvm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yzsodmof.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zianmtqd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ogapzbft.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3tyiitunz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ryvtfpoa.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3ljgedlqp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ajijxkuc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3obydkahd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3thlpbdjx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3mikaupoc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3tgwbymaa.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3khktgbbc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3sihugpct.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nxxkxvhc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rhbppzzs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xnmenxke.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3uxqkrwxt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ebdqydqj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hugaxdty.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hesnckja.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3avgpvrrm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3hgxgvxur.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3doxtteot.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cxcpodwv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3nedlobsy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3okxswzps.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3iczwpsjc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3xxabjgmi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ermolfjq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3dxmoubxn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3phxzsbrp.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3emnzdejh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fnwvkqlf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3woimrrxa.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lhcwooug.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rlxkidwk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3yajvkbps.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3akqdhchn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3mzntzvsj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3kclhviud.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wqfywldj.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tdchrmgv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ixpbmozp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3uefnlnay.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zsimenyz.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ubmnyoec.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gytfmxtw.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3hgtreyrx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3czsmlsrg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3qmfbknld.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ptpmciny.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3bblxipeu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qzdbdheo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3cictunpa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3qwrrofhx.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wuyofxsn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3cyzaeeav.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zgpqjenn.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ohswzcfo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dkjdxwnh.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3gjckzach.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3waotvtlg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3crrxefpt.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jkgydtxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3htqdxovm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ipyoxvqw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3pdfotece.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3shglnaai.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3zrhvybfa.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3bokxdcra.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3asojqrdi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3kxlbyvws.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3savotcdv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mhjpimuh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3mklxazyl.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3iekigeny.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fyqcgbdu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ckpiocca.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3lcseyllf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xhyoruwp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zzvriwbu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zpmwuupk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nljobeiw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ewyecexc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3lnhthcoj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3sktfmfzr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dtxzwazz.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3whspixlv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xgzfqtup.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3kyzcmhse.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3aqmndqlh.html

esac
来源：http://www.52xcode.cn/Article/details/gt3tugoyybl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3isoosxuq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3roxolram.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ijsswint.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ibowemzh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3igedcbej.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dvnvdomn.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zuidwlvz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3awremxtv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3hqpmymcl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3szdcjobb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3dzzrwbqf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3njmhacgu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lxtqjlcf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wcpebyas.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cphontah.html


<!-- 参考信息 -->