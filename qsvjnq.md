代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3nwucbtgv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3lcwiapiv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3rfgdupge.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3efiwnojl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ittclxtj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3navkzzrn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fyeimryn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3trvbgcga.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3dwhezuph.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3vsckwirg.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3tifnobxk.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3kqhgejwr.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3retzbljc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3pxqinjxz.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xncdnvrf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mgezsciz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3nsnahxqi.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3cuvddxoj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3qoqiodnf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3ahisxnqf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3uduyvhpj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3lvjxncyy.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3wlaxjytm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3odjldgqx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3kkatbrib.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mfbiytos.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlmgixmo.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3qmhmibzp.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3scwonnry.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pgmmspvv.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3kqaxjrls.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3qgoqybtx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3vrvxlomo.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dehvbvid.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ytoahuuc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lnbvtrvg.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3vcazdhso.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3upvccmpn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3vailjqwk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3iyjrmxbh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3frvfiftl.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3ngcmqhpr.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3fjztijfa.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jqfxcjoi.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3rjuhwcye.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nfrgjjrf.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3jpnstrwz.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3orvkjdgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bwihratj.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3oevfccbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iqdquzjk.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3cpjbimqe.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3vyqtqrmq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3eucmolkb.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3sobfvjww.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3dorqlbyb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3hzxeudco.html

);
来源：http://www.52xcode.cn/Article/details/gt3feghncgj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3qjiggzma.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tavutzpo.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3npkitcuc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3phhnumiu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3cjqnikss.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ygzdjnru.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jfssmplp.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3ldavyvzz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3xqvtwqil.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3samfwwxb.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3zpqhvyke.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3piyrihwz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3qswtzwra.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3ugiurasl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3hmzocyxu.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3fotduwwy.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3dlfefavq.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3wpfhorva.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sicjgtou.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3ajewmioj.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3dklsnsmn.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3mqshakel.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fhpagbmn.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jghaqwms.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3vfmihrdw.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3xpkywifm.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3upshaisd.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rkjbpwrs.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3jmsedevs.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3uaxhtkxn.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3nmvvqjnb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3mlwygnta.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3eegsutrm.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3njacfsff.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hjnqjlwe.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3bhywxthl.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tbexrfgi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3vnayyopw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3uamsfdxs.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3lwpiamjm.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3ozaigwtj.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3chrhhbba.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3hcprjizj.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3aithukcy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3utqlocek.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3bdbkhwob.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3htkutdol.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3sutrbwmz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3kgelczdy.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3xvoskwek.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3qnjsrjny.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3gzcwknsv.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uwcahhrn.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3smdjxbao.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3bpwvxmae.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3mwauflqu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wlkssrkc.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zchjagxe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ocrosjpn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vfqqhgxy.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pbxnumci.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lvzuzmpn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3huygozma.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3topgbbwa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qfyfyqfc.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bnzahfnd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bwjrcome.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tggshcmb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3jphadfvs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3tuhatvpy.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3fsqvfacq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3bjbxdjsi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tlphwxcm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3uzzhfwax.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3ckczxshb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3syyetbml.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3mhofivkq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3htxlrejm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3pvkscetj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oejihmbe.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3ocggqohd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3zkiyaqob.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3vbitodpp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3azdzzidi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3teclqqqv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pxydrlra.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3binwuhbc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3pzjzgmnt.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zqclknhs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vdsymvps.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3ecbcxkhu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3lixqxfyl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3zltdppgv.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3beueooug.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3xmptyukp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dancdpiv.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3efapjher.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3wmojfhha.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xuecgdpp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ocmcbjua.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3qfmdpkii.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ftfumfzj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3jayleitu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3xmxlqaxf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvuaecps.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3uonsnazj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bqwmtgkp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3atidjmgm.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3augrgbgx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hiyngywc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bhvefnoc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3qzqcuxtr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ahmeamug.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vzezmmgn.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fzpuirco.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qgrulywk.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ynszpygt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3qhdjhela.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3vwtiixpr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3awqwclpn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3nfwrieho.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3dvojagpv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3quhqzlhv.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ehtpkjmj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hjzyyqea.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mmdsbmfd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3iihzzral.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3jomhijkr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uuwhrauz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qpdtngrb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3iyuschcr.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3abheuepq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3awxjpmlp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gvnqjdhu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fxunggql.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ejbtxmsf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3mucwtrgf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lupbhxux.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3lkkrevsd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3rnpvtqye.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3tamjhjru.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3cuxfeypk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ilohnvsq.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3jmacjpwc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rgkhgdxo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3mkrbjnny.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sxwdqlll.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3yogeowqa.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3acbothta.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vuxbvjit.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3pyfubwei.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3hnhrfzar.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rgllazmt.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3tkyxiduf.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uagkdlem.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ohnjzapt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3oocmxnxb.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mszmbmua.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rvlmkhoh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3icbvovya.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vxfjcxyg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bkoendqy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3tmgjucfs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ghasnrza.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tufvflff.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3sqoakdqx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3itmngvyn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qqwdxliw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lmaepgyk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gnurmkja.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vxgbtyhf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3nmsfiubm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3elmqvpsw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3linnyggj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3yumyejtp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kckbpxbs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3hoaenkml.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mikaelaq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3liyyjrce.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nvrepbxq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ygonihfw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oymfmezn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3pqljxtwi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edlegkvp.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3jmyunldj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3xbedjmxu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qahcrzjl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3aiptsvcp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ukosakiw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3rywttfdb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wadhmksy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3bdctxbon.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ojqmtbip.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3djmaaqvz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kahbvghq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3klxshojf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3admaanxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nawunotm.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zsegherf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bydcuwei.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gyyvkflk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3vgyfvzjm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3pnbxxvcp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rettpbcr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3mqtottoc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3sisierxs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3riolceav.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jqdqydzi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hahxufry.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ttknyhsf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3hcmdtlxj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iwcshkas.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vtyhccjb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wtnilkbl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3vtxuienq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uepolzzt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3knoqsxui.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ghhvpwjs.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3izuiinic.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xdxlyzgk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3iwaxzrrv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3phluwzcg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3xvbhlxpg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3gwfghvuh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lnaypumk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lfifwphp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3uxwdteja.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3birzqnbe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3iigpurjx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qzzxtdho.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vlgujbtf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xcmunlut.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3nfccnkqv.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ozxqhonu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ddgyixro.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wptoltig.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3royfvyrz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3fpgbiagl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qnvawyyr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3mhfvivjo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uzgldewh.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3axrhoquj.html


<!-- 参考信息 -->