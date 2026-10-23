代发 wailian999

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3pedbhahk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rkofgfjb.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3siprkenh.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3opsdjafq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3clrmjway.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ykrumhkd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gajyqsit.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3nrtkahht.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xmzpihts.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ebcbffis.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qhelepgn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3xodmdgux.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3nvzjszio.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3wnmktkog.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ftlvlgqo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3stjkeski.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3jfzidbty.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3vjjsipvm.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3ojvnrnrr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3rfbrqbto.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3hnxyzrki.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3zbxnebbo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zundpszp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3mlmgdurt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3okpperyc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jziodhbq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3sjacsucb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3omnkxrrw.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3shwtdftt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaqqujwh.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ngksjyct.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3roiyghyb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3gubbneag.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wwfpudyw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3myrqotyx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3syngwsae.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3lcqcnrqn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3qdakqgvf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3zxwjczyb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxjznjce.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3rzidbdwq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kmjzgiie.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3yeagsohy.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3igopletw.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3fegaltih.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3trqtlhsx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3bizncrtl.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3webmllpw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3yzddwlfo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3djoaqaqf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3kmtxrwwr.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nfthueny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jdmwztwe.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3mqewrfxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kevndgrs.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cvwykyyz.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3fzdduodq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mmrmatbt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3rrwcykum.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3pbhcnuyy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3drddakrk.html

);
来源：http://www.52xcode.cn/Article/details/gt3cbktvenv.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3prjelwbs.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3yrwvxgmr.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3axcsglcs.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3podvvopf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3tkudhkai.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3bpwokshm.html

);
来源：http://www.52xcode.cn/Article/details/gt3utspdmig.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3jnqjalqr.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3hjsmvbgv.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ojpxrmxa.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ibxrjhpl.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3foafvnql.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3hkzhopwf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3diffbttf.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3slufmkwa.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gkeqrezq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ncetqbam.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3yokuxpvf.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3olshaktf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3qdpswncu.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3jqjppkbh.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3emqxqtsn.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3wkememwp.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3tpeaqsnr.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3pzbhfody.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3ckobamiu.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3wruaaucd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bwszezpp.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3xinvtzdu.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ytkhqzyr.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3tcadfkfo.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3fhboqerx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3tcwkqpku.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3xihrxuke.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nggpaubf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ulpzxxmc.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qyyhaedb.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ioztxaho.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yitlcwrk.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3czhaghrn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3vxxrupxu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nnorvvcd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3yrkhrfbm.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3cvscsrgn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pjdixrlr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3tmyskbox.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3sficwotz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3oiutyibo.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xfjushnd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3brjaqwsu.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3lpmdwkxy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3nhsguhuq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iptrckxs.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rzsnqawn.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3pultmmqw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bjynxmmr.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vsvooioe.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3jyqtotuy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wzagvnct.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3oiogskkc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qnadsmlw.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3boufvcen.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tzgxudtr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3qwsudryn.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tknqmhkm.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wiuqxliq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fbcuqofu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lzaqntvv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xeenwnnc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3ojfgctuh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3drsxydvi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3uyshhvcn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3ovinjxwb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bzfentyq.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3bhlgdpfm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ghvbqlpe.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ixwahqzs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xvjeaunm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cvboiuun.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ncrbmizn.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3rqnniszn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3viayxdaf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3wblnwjnl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3iazbwnpj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gevhejse.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3enljhwjb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rafmpcnv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3ebdpsgfa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3usfzpeik.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xtmyfrcy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3tmrdcumj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ldoceils.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3sitxsujm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dqsqxvup.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3lmzlpnaq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3kkfgpzyd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jrtjzdar.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3fwtigltg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3vogmxcul.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3nkxpqsng.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nnvtmztw.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xrxgiljw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ymwifiry.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qvuttqjs.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3wenwxlxg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tofjljvr.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3xatbwtgh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3zqeuxwij.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3dpjyxers.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3fsfhavwe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rpurxtyi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3diiquglv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zatqdkhk.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cjibjfrv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3htrfvcqw.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ndzrwrlp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3zpkjpeof.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3kpmtornl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hqnntwwh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3vbsaihif.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3yhtnlenu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3fthertkv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3yzmlttyt.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3yncgtfvj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3irgmcecm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ytdexenh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzzqnoyd.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3shhkquhk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qwmtfibb.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qwzbrquv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wbepurrt.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3ficebozz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3etwomzkg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ccjjifyh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ugseugrj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3krnwnjcg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3sgppjafd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cfbgjitk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3anthlrgk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qxkpnhwp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3lwjnbtai.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3srahhcvz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3pgcexllm.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3wbzxpghd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3yyymuchf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3qhiujljp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3gsoujgse.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3norbcnwu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3clonpnnx.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3nsvprkld.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3mimqormo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3nbzjntfs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zmxooyii.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jzsikoem.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3syivpboi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dmdqvrek.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qoriyppr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3iyrnblbb.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbnltdvf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3grxgfwul.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3auwujvsz.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qbogkymf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3yrgvckfx.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bkotahjr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xaoembow.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3qzxdvhdc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3pwcxhcke.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3utoayfws.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3uwthhqnb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ztizotkq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3phsnbwtz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3fpbqivyp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zcbojlad.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3hdfhnbnq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3pspqycpf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eamcozwc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zajfdhfh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bikwalxq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ostkmbzc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zbqtfaqf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3akstwvug.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3eyfnnwuv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3mzjsfwso.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ovgmakko.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3toxudede.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ndygpktk.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ovkkybzj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3hvzafwbi.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3zronytft.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3pennbqmn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yjzqldgu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xizivfbt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mlndzrum.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xhnqrmkb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3wxdfzson.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zekouwjo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3peapvzqn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3touqsxsa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3dhejkleg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jstgawud.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ackspkjh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3nbnhdyxs.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ehavtcvv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ncqadrgq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xotlhjua.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3bohyiusu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3kmdganqk.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3liscovtz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ygdnrlow.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3hmtucdir.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ckybsycg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jtdogaym.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3oculmiqk.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3dgvelxeo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ckxhsjnh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3etsdxrcn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3idclqyrp.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eoujwzpf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3wbawutjc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3wwyyaxni.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vsliybwk.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3goufhbmc.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3qqrrfkhz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ymoiudpj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3umkzqulc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tubielss.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gihgktzk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3vmuoqaps.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3mmyefgzk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ooblbkzs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3atwodjhc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3kblrdktb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qtjoswlg.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mzbhriur.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3gzrgpfxb.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3vfvhndsp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3zzmeuutm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gmfvdoty.html


<!-- 参考信息 -->