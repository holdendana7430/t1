代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fbhglyir.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3csdfczab.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3vaixmdxl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3abpltcaa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3usdyskdo.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3yofaxroy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dyaczqmn.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wrwotluy.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qxlljapm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3qdfitocj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3dbxdrbtb.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3hejgmcem.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3nmnwbojl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3nchpvgyx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3bgznhtax.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3dgrfnaba.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3aswvyttb.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3rsnyidcm.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3nahaciga.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3chaiohgc.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ipfmmxzp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jeusifzg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3etlvysvs.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zpjtdelb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3fkpabhnh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3egvxeuix.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uquqfipp.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3qpxfkakk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3oqeuscek.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3ohoavnem.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ebitwsrq.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fgxnjeds.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3dckkjjqk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3zdrefnvu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ppvdcfgh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpxbbpqf.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3xxmviehy.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3blkebnni.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3osnvzyqj.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3offwkflr.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3caehfcas.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3vpeoqccn.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3dbfsidxe.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3zxbwcood.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3jjmiqxep.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3wgiozswk.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3tlgkwoyp.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3jefwjcsp.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3ypkptwdn.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xclgmzqw.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3nxrsbggb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3eshvhbpz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3xtseibqr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3kyabqxuu.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3wxpywgzk.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3dekufknj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aaqaimfr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3vinnpgrp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ysspgkcn.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3badydzlt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt3yakeqnrs.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3lqjlhgqt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3oboenbjb.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt3bgrhccud.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3svlrkcwo.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3cckzynke.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3poxbeqvv.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3oxmqdgau.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3fdivhkeu.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3nosainwv.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3qyqotgsn.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3fnrehwgq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3gsnhmxwb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3bfunphuz.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt3rquwwmas.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wahscgsq.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt3dqxwfpbi.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3yfsyaemh.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt3nwklshlr.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3mselvvya.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt3ddjrobom.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3nkxnnhsb.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt3ebqralus.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt3tnwkaoik.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3sibumwrh.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt3fycjgtjb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3rhhskeyw.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt3iziwimdc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt3iohigkcj.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3ebszuyaw.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3teliwiam.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt3ysswjrvo.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3gkvpjqqq.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt3ozgbdgwi.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3yjlwjlbe.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ywousaef.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3dvpmgzfx.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt3hroytiqr.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3vhwamdod.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3imgqvxcs.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ztyajllx.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3icqtqwuz.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mnbxvizd.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3cpfiyqif.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3tfqctdvi.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ydbavdpb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3irfanrha.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3xnkdwiwk.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3hduniotu.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3dcefabxx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3bnkaroho.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3qjkvozyp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3aaowhpom.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3qsewlwvl.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3apwekzzj.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3xxiaynau.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3zkevdjme.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3xemtdhah.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lxxrfwxt.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3iqkgoeph.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3appbetiu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3ghxjvdri.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgmghivz.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3klwvwhka.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3agnntnib.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3omxbphoh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ifyqhlqu.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3fdbprqkm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tluccicz.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3qumxaens.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3zimdiytp.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3waldgtub.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3jlnvleke.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3boafouru.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bcvnbzxb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3expqardr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3isabseqf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3wzbqaqlv.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vrqsrbee.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3epmvxhng.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3khnkjohu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3tfytycbc.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3vzziotcx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3iluezcbq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3yckyqeco.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mrxwnzgu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3dvmbcpeh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zhqvswnv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3uixgalpq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rzgegbki.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3raddpdxg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vumuonwc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hrxiqpkp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3nwyjaevu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bhzfbhby.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sdaxkwbt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3valzdcbt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3nkohrssx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vdepnvap.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3gfihhxdu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3bfxlgwqj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3tmncwoqe.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3fziuzoie.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3mlqdphnm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pitpztbj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3zfkwhmzr.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dpawneuc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3pkevihyb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ncqtdssn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3iwhbtstq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vapenuoe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3tbbbjnik.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3lygjirfr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3udtbmsot.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3hfmrfxiy.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3xlouihze.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3fobzddyh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3imnkcvwy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3dhipxnnf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3hnhplizl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dylplmqx.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3mujusbec.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3ohcegiin.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ruuvsbns.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3fnpkokbf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3zvixmmht.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3lvuikflo.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dmxwbdyn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3avwsynbe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jdmmlmay.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3uqdzwtms.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3asyamzxk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tfczdpox.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3xmagigfv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xnxunzmc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3tmqjluuh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3oqdnlemr.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3sfmeplyz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qhbuuser.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nyplyunv.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3mvqnmebh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ncnfcocf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3djinmssj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3omfwmmns.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3sqwwaaxe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lgzsaizx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jcellqqj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ylzqzyzx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3tkhzeica.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zvemtryi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3viwmggev.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3qgkrglza.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3yadtfaoo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kbuxeznv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3thjvseco.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3osrlwwcy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3cvwyltjf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3swqqozcf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3fyoyerdi.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jrutvmgh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3gxlfkqgy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ntuauqxj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gdaxvgto.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3woehpuva.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mpolftyy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yhkuxzlx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3womzkyto.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3fqvptfoi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3uqcawvci.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mfjcptwr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qhiwywev.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ykionzbo.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vftkecth.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3vxpnxxop.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nvjzxuzl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fwwbfvel.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3stnateeu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3drgfflav.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dbhpkdqs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3allxxhcs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3plggtllr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vkjvecqm.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gltvgdvv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sezmkvqe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nwomrcgw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mhbctcka.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kjgnqbty.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nnzdbgap.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3knzwrnvy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bzshciev.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ofgwzulv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tbqcaezs.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fgjkqicy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3fsqvgsdi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3kowhhruh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3gdygsfan.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3klqjtabe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ueyocxdm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uuurqkmc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3emyvyjhv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zraabuqp.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pumlduup.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hweuecnf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lssxmfbb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3cbuggggn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxgiminn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vydyyubp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3jlovfsdx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3nuxoruyv.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xfvefgpe.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3mseykuma.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3hwhvtnui.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3snwvykwh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3mbgbgnrk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ynfnsbyf.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pguqyams.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3jnaldqby.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lngxmusw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ikkisaqe.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3klhoasfu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3timzubpl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3csniikgc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mufnvbpz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3prnkaoho.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ryxxslfv.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3hezumsth.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hzgyattl.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dzpwbxie.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3gmbiycpz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3fnfogoek.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3afdoasyw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3drdzvpfz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ktcnadhh.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mtwoingn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3cwlprjlf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3pkjjoqbu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lxneczuq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3lysbjwdf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sgatqnks.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3uvrsscnq.html


<!-- 参考信息 -->