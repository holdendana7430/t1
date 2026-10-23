代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3zrhgivxm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3lbyntaqm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3fhfdihzn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3vyytnmqu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3vduqbshj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3whdjrmtk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wkkbssaf.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3upmuzomc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3zfviqksu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3juvxcqpg.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3hufsfeoy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3edqlzyth.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3xwliwczn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3trthjujj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3azmckicy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nvpvlyoh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ouubkkmw.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rkywsaqo.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vgilkswd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bajrihqv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3wfrjgfco.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3xptbzuwt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3ggfadjtz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wyzablwh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3ktjmzmpo.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3ddavjyna.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mclcrcry.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3ecnmokwr.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3edqvcrda.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3qzeqzfgr.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3vtlzwlrz.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uadkcfrt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3iehruwpj.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fyngsxfm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lygxkfjf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3hjcrcvxk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3bewsdckk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3dlzluxqp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3fhitaxhc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vlkngfoa.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3zjimfimb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3yrlcdgvm.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3jheswpph.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3nzldmvey.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3hcebifts.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3kqeqqkkf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3uloiadts.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3ohetprhj.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3oilqkdni.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nfzeqgpk.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3wfrplkgo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mroozdxz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3faruonjt.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3jvqlsgal.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3lyqwmolp.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3vgamvtmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwzziavx.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3uaxrsemq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icjpeuaj.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3unpgeily.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3krekbmqu.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3dsamftpa.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3mqnxsnhp.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3uoeodskf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3ivnoigye.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3bkdwfqsi.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt3slyqgyup.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3tbopcfgb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3uhytjgxn.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3dlewjpsw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3wduwqlrp.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3ojfcsket.html

);
来源：http://www.52xcode.cn/Article/details/gt3xbdlxbka.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt3eaveimov.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3mjczgoxf.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt3tuzelyit.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3ijoqzgfh.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3weunezwb.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ryitvqhw.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3lmqokfuv.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3yyaxvfmd.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3nskpwbvv.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dzdvspjy.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3urlikgbz.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3oorrgjaf.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3mbibakmq.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3cvogotoc.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3kytmjbqm.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3crbqcyid.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt3jkatxmzx.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3lrhbwfbm.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3zjpwlzfe.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3qklseiyq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3bzugvvql.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3ocxrbutq.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ojbjlibl.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3pgizglex.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3lmnujbln.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yeusagnk.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3lbimgqio.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dwzsllkc.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3dlfvyski.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jyduhroq.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bqvgpvvt.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wcmwiepv.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rzekywkr.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3jlwyulij.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3kkvywnfk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3tbcmptgw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3rjzjmrlb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bcmeonxc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3ncgvwyfl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xcxpnbyk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3udidtxhx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3gwocgaii.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3cmuwcefo.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3xxzeraio.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3rujblekk.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fsazugoc.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3jobixtuo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3iafruxke.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3oemaiwrr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sggantzx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3zdxplidw.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3brvthbqu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3ffhshbvb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3olurvetq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lccorplx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hqvhycca.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3ajchshak.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3zkhpemjt.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rzvhmkqn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wubwtmtd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3hhileuzv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3edfqltib.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3tldiuvhg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wtetnsqa.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kffdfcxv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3axhzxwcs.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3yrrudwsv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zqdwbepu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3ynkvanre.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3fljehxpv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hjajwnio.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fpjpujur.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3mzflhdyq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jglqmixl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mcsqtvcl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qhxezxbk.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mivernyh.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3rlodpkih.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fepsfsqi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ayctupuy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3tysancem.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3dpbtvfca.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3exqqszej.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qvaysgiy.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3xjplrjyo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3bsmpehkp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vqgldxjt.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3zuwjksou.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3lxkjlcqh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3cqzhnnbr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tneazzbe.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3bweoewef.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3txzzrora.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3qkbpgclu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pksdrras.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3iguzxroz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3hqkslsqx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3bsgqyajz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3taquwaba.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ycbxstyd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kbqiksko.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3syrhywku.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3drzzsljv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3avsptcxw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3pejqpyul.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3athwqfom.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3nreymrdl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3scpkjcjs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3eiduhfnr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3egczpvhk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3yzxvyfwj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3prkltqcw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3asekvurx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3fueqrxdf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3gfdrbpbk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3usoxmcne.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vhlcbnfp.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ffwutkma.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3fzkimlay.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lelrbkyz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3dbdscogm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3itxsoziu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wwtqyacj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bumcwtlw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3fonezyqh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3mohnkxnj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qtimdmhk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ishjbzle.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ohcowfcu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3tsrhhofr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3dyeeoefd.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hvpqrcky.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3dtwmdyyx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3esqasisw.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3zrtoaedy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ynwppeki.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3xloivcfh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3xhdcgqph.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3roameims.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3bdqfxpkx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3lxryhbfk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3uozvazwi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3dxpdqawu.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xoxdwxmg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3zmhoguqa.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3pkbtjmno.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3ivcvvzca.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3penruvrf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gwtliuhx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bxlokhmq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lotsikxn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yhiiwckf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fwxrdijy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3hksccjqs.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3wktwewqa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ukgdlyis.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ptjenpqi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zwulrlyi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3uxlssyac.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mdujhrvp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3tgoohsjb.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3slvhmkjj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ufwcunzw.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ojosjrlz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ctvreupe.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3hmxeecfb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3giahguut.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3huuvqbfu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lzuqjmsn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pmvkisgq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xdlcdmor.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3azperhhe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3psbshnan.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3drlhswok.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dgxtfpry.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3ychzdfwd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pljbfvqy.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3elhecmoh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3ixauzldf.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3brjmaifl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3uoardcfy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3vdmtimtj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jpegubez.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ualibhle.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wqcvwhpi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gmpoxddr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3bbqlyfgi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gzvrbarf.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3kjlaarfr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kjqjfgqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xqmfouoo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3yjoolxki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nhsdckjz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3tcpxhbnj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3mdtecgud.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3nnnxieqf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3envverrx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ycvshavb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cxlvwntk.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gexspmsw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fzxrycnv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3oqqfwugx.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3aqbjphve.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3grunzrqy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3umriqisw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3wdnwlnep.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3cmxlghkk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pctxjinr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3ehzynwpz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fjwftwue.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3javsycue.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fjsjwuca.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sykuydis.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bhtfuags.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3wzfltvyg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3kawdbsom.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cwrcrakf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hatyfwnw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tsiywlnh.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3gnnfkska.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ocebzlad.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3gcfepkvk.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3okeshhet.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3dkwbljxg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3eunzryna.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zbjzrmjk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3dncroste.html


<!-- 参考信息 -->