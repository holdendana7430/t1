代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jvzzdzrb.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3vjygmzdg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bsxgonvy.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lanxlcni.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3gmoqigac.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vppvwzou.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3tprorqdm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3hijrjtmc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3wxfgxibz.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3vvwukrhh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3oqcqimbr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3eijbxlni.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3ujtwqcdr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vjhehuok.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3sdinehlg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3omytkokx.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ivfqetjh.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3pqgqrfjt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ximpxsjm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vrmmdyva.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rseexaau.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3uqmbtfzd.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3wrumbnvt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ntmgpmht.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3spanllib.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3qzchmagl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nncocflf.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3wnnricld.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3bcqzwwcs.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3dvqactfd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3rsncmqvc.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3mvrusxit.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dxxoyflz.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cilwhzrf.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3lstjixnm.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhumzfir.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3yilubhxz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3elllxdxq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3vmllpmtc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3nhgdtqyd.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt3uudegmfj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tkxoiabt.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3glsyotyu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3oflhyqdq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3alvooxjn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3qksxdwmj.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3mmkmhzqu.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3avdyiwqu.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3mvnzasyy.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt3jyjcfhhv.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3tjtjzixo.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3jqlrgqch.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3uzsonbtf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3wmjcuett.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qthemzcf.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3thjebmxl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ecoheqew.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt3ubyvpxnk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vidcgyos.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3aauonqer.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3gwwyfgdg.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3qxmhfjdk.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3xuzsuygu.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3vpurdixt.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3henqqvjr.html

);
来源：http://www.52xcode.cn/Article/details/gt3phnvdfbu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3woqllnxz.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3pelzbnrf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3ugrnefym.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3qdselmsu.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt3twvxbtqb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt3veqmzpwi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3msuawlot.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3kprbkomx.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3twnzfmrp.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3aumehjzn.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3yirstodx.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3davysgen.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3ianmeosf.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt3erstguly.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3gfftjzrg.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3gijrbivt.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3klrbflvg.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3gnronjuw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3tkpcixpt.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3clmaxcyn.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt3ggfpwugz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3tqqwhbgk.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3fcgommlm.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3usemssyd.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3zbcyceym.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3hrgobdqs.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3ylzmcphf.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3rjmukmvk.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3bqxbcnkg.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3fggnazdo.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dgrijvsr.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3grbndrlj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3qhjlgeub.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3soalxuwb.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nozzvzes.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3lnbbtynm.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3owptvxhu.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3bosjygoz.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3xfmgzgix.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mmvcyvdz.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3iyghxkid.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3rpszvlek.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3qmjxlstl.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3diyhcjyb.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3fbtezxgz.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3oitxujtz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3ucenkgjg.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ogevnxln.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3dndvuafq.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3ravqntan.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3mjiixkaz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rmpxbckz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qngagora.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3cvniuagx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3yzohznuj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3mnhzwonu.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3duzegkce.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3eurnkpud.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3meihymvd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3vkfsgomq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qqihwjwz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pyzmfthq.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ylzhawyx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zcomotje.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3cfakjgdi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3bojpfjir.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3dywxdpmz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3jzblkqpo.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3uzraehoo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3kldyugwm.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3kshkizuv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3omfszxwg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3xmkgmaad.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3wyjsvjvt.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3rjmebtfg.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pwcskrlh.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3xyvlhaaj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ckrodian.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3vrfqierc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3uejozbmx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3lriqceej.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dolzysos.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3metsrpey.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3abfrhifw.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3thlfrjrn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3xijnjacd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3biutiecn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cbkdcbuk.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3kucefbie.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3gfdtbhae.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3byqjuewo.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fxdtzdkz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wqmpohoa.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kbkpimqk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3apdjheed.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ddwoohga.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uquukkee.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3otzoleba.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3iftsfqie.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kpxpvrqt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3aukynjyl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ehnbjaoo.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3fdlbpsds.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cjfzelkk.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3msktfvnf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pzaklwti.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xbtaysgy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3prsdmluc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3yiozlqya.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bqolhidg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3fsxldtla.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3ivldsgxk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gfndujdg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3uqpvkhja.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ceandqdw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3qogkvpyf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3spakqhqx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3fxbhgyin.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kkljmnrx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yfgvzcvk.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ilhebwbt.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3aesfveur.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sxqslkmd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3eaduxwhv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3gjwaorpx.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3fejfyeyd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3msiromym.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3wtkemypb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uidyixhv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ivaapbhd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yohlqvvo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3fhrqedil.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3lhnqsgql.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pzodrnct.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3chralasf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ijsbsuml.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3tvcxqnwk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ylosuapr.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jwalxmqt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ncoeayxx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3yfirdxhl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3odzdsyir.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3achatlzi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3gcktwdkp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3qwxtgose.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3lodabilr.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ywwgcuxu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3omlwvcgp.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xbcynpoi.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3fuuamzty.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3oxaskudm.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3umalqrbg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ztlbsicw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xffzcniw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3vwqdjekd.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tfwoqsqs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qpptlpkf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dioncrin.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sgkttusv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3azamdsya.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jmodpono.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3bmhaiejg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3himssqzy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vwzaoblt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xqstblvh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3xgumgfcn.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3itgeytha.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qttghyif.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3bbhgdyyn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3vrgmnajj.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zlmnjfop.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hpauxpcu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rzcxdqxx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3aaudqrsy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3oyxazkyk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mxolttoq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3depitque.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kvnjinhl.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3vyhudoro.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xabgkknp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vrxwosfb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yucdvnkr.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3cwwxhsjd.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3snxdsqys.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3dpbunbri.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jwnglzav.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rktfwwyw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lgkircfi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kidsowgg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ryiyktrd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xbslgeoo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3mprzjzom.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ibnpgxqj.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zgeveiza.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3bilxeadk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3lzsxtsnr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3uisiygyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3closwsnq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jztxgyfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkuubjut.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qqrbdbml.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qiugbxvl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3eqdkpfwi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bfrbjrfb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xmqvqeaq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3zsjceqee.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lgjjhbhm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3sdlufvol.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3bgugeshf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3chastjpx.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3cmwhiyrt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3aeuppwat.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ienmlymi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zfabpxxy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ownlievy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ambhmnje.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3papewubc.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sraspxgo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ahdomhjm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bwpiaxpd.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jynuaynh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3wkpaffxl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3joeddzud.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3faqiwuaa.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kgjljxlh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3yfjemuyd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3rfqaryvc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3rlhpudhe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3ulhpnztu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dmunmeef.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lxozqiid.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xoieyvuh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sxoknutz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vmbigggv.html


<!-- 参考信息 -->