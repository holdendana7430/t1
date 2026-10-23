代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3eeamcwxz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3wwoegwxr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3fmjksfbr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3bygaebmg.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3jowucltf.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qqkdhzse.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jeouempl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3heecydjv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gbbgqkyi.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3kbjidecf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3ctocgrvo.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3jwcihmwo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3irdrwnwp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xovbkpls.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3digxumif.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3nuqjwjcg.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zvjjwuca.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lgtigjxq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3bwhwljvd.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3dlqpeyzv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3rymzasfu.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3nhysboiz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3hxupjerq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vniejxyf.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bdjeqnns.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cgnxnhdi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cinyivqa.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ddoegpae.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3sqgraoii.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cycynwat.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3aqrkhihe.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3ijmcvauw.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3dcyrdcii.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3hwixvpwh.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3luksbeou.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3phjvuhsn.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3uimmzkjr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3dzgltpda.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3utsqlzne.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3nawqhuun.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3bwzctiek.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3fubmztqz.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3yqeqckny.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3scaecpaa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3ordxfpwi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3tessysps.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3audprbgm.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3cuevutlx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhzhvija.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3gxgtqhxe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tclhuhap.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3mtukamtz.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3trfqnewl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3crqouyuj.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3yevdboxm.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3braxeair.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3ijqdbdiw.html

);
来源：http://www.52xcode.cn/Article/details/gt3rlzqyulq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ykztxvxz.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt3ajyiqsfk.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3mflcpnup.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3unzyylra.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3mtsviwng.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3qytnydok.html

);
来源：http://www.52xcode.cn/Article/details/gt3tuwcghpn.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3fiildznq.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3nzsunfoe.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3ntuckvgt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3rgsflzbm.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt3gccqzrky.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3toivsxqp.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3dwkhimss.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3elrpbvpo.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt3lllozvpi.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ribgjlzt.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3utmzmsxe.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3pstnbogh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3kxoyboew.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3lwpnxrdo.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3jczocsfe.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3dkrlgcgr.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3pzdrtsuy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3nnwgxneg.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hlrzopet.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gjgewvdi.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3lshgvreb.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt3xyozedrm.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3jqugupqp.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jgmfeuqi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3qgvvxchi.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3mrpvgtln.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3sagsdtsn.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3okexfmas.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zebmaewt.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rlnhyanw.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3zapxobvm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hvkerbzq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3gdebcjfj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3oxwvektj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3yfurtxmq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3riwvsqkj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3drqhxckq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ugctjjnh.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3jtwyhwbu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ptfxxbyf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3tjmrksvf.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3wmohsnde.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3tjxftwxo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3amjlgkwm.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3atsxjdyr.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nqrsogvu.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3mquzkona.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3tjlyevuh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3eagipbjw.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3axcyjejs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3slyhuguh.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tlemhrvb.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3trqjlozc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lgepmusp.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fufphjai.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qasjirza.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3pvdcvhxr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rxkbcyls.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3qphqvnva.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3picmirvv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bbfbwvnv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gmpvmqwy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cjvxiwli.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jpzrcysw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3hkzbirbj.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3cexnndhd.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3lyfcjyka.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ulpuoijq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3chndfvxi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3zydmtajk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3pfpumpit.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3cpcsbczm.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lmfjhmuc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3uvecogpq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hebzwxpq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3etqpfshg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3qwzpwoyi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3kyhgpxng.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3oxtahaif.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nnomyboh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tbqxiryr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3hmwbmxhn.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ehbgzwgh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ywoctfzp.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3nfbzpssd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3jsgybdsy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3wumswxlv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3nosgamvg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dlupptzi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3frhygdjg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qxbdxunx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3jijidyhr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3upvzpnmq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3xhnurprc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3osroxvou.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wlobvyoa.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3zlwdoynw.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3ycfhshpr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3hakmeewp.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3kvnkiogd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3brjlnyri.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3rtmtncki.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3tsicfftb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3yzheeqty.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3znvhksqo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3sgpxwdgg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3itxjvdyx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3omvjqmtj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3hczimsdx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qlxqknke.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ckwwrqsv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bmludrzt.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zgfkpbte.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3xlvqyerp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bdenwpcl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3papirnxp.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tuvpajyj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3idfxwwdq.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rhlubbuv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qmpqdgsy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3thwwldmf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vwwiytoa.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3lanosfid.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3umbxpzzl.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3gzxdbpff.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3yzttizdb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lehigpbb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3sgvlmzgo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hyavchtq.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3yahcjbcq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3elgznhbz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pmfvvlmr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3fdvmocub.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cwwiacjp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3twlfficd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3mxmiwemt.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jrlsgvxq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3cqgrwmqb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rljxuatt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3olbizaxg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3xgneqclc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3tnodizyc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zfuemwdx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wxqpouir.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3xadtpydb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3oixwlfrr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3tylhnwgn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3fpvezjkd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3bcirxdlw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sufhcfcr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3pyvavyup.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fgepufzy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3jcspxmdd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3oaylinyc.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3dlofxcxm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3rblahnsr.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gzrpirsg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tfevpozr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ihvyucib.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3vxtgivte.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3fubqwwsd.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3piwkvupr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3siloluvw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3diqmqqxg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gbbujkis.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3njsqntpz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3zwmvkpxg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3vypolkra.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zrykctps.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3iydmhwtm.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jbvugrbq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3peocevql.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fhriwqdx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3wvmqqpwc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wcukaubu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qjjaelvp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dbgfbnqn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3cialufow.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3plpyujck.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3lelukdzm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3zdpylxea.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3bqjpzvao.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hxylcpys.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3xqgerdyu.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3goppiswz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zxvsagye.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jydknxkd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3myhvemoj.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ktyekcgx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qucbfqrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yyqwddbx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xxqaphjr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xrasupln.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3wnnrmxsb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3drfhizbg.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3xijtpazo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3mqawskgu.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3iqlbmtiv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ksscimyw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3liddxtgl.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3yiweaayx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3llnsavdw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3igjqhaou.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3djgjesxo.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ynbdqjpj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zwvxjkbg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3rqbgtwps.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ceqanphd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zqqrrlih.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3oqqhntsv.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3jzpytlpy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gqriddxb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cxwfsfsp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xejntalm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3qtdoicxb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fzvdijta.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3mfkamyrs.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3bmllsbti.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uzbjolvd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qhffpful.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jodulfkl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vhockfhw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ldrhomhi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ufemfjjs.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hrfonlct.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ctxspfck.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sjhynicw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3vcygyvjq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mnopmicw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xmnqhkwd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3arqlptdl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hhhavmxz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ydrtmjbv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3wimpzqqh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qezwjwqb.html


<!-- 参考信息 -->