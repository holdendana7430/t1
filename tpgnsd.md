代发 wailian999

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dczmeusj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bqgnobbj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3wmpzitqv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3qddotxdc.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3mtqanseg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ajcgitwd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3yjaurlwv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3jufvjvpt.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3mcsdttea.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3iwwewyka.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3htqieisf.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nqdlziak.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3bymrrmmk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3afeisnqx.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3xhbqgtle.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3mlcskonb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3eymxkena.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gdllyjaz.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3okopcwcv.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3djmqpogb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3tipdfbvc.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3jtzrwdlh.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3nsjektyg.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3vyebtvsq.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3bbifasjv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xnkqvmwj.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wdbadjea.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3ghevwegg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3yavwjsoj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dyrwflvr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3blkwaoud.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3jtmaiohv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3qvdhfxtb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ujqdycky.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3iyggkixw.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3mlucxwzw.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3guiceoky.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3mfwhcrip.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3aktqgtdw.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3yjtyexzy.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3pekcdyvr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ufstaqns.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3cekjaets.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvystago.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt3gkpydzkj.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3couhsdpa.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt3duojiedb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3nqxznxdp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llwlkkxd.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3btmlgzvp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mduxajhg.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3gswkbbti.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3uirsgbiq.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3isffoqnw.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3ziwvruzw.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3ovvetqdi.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt3nbxgwaqi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt3jbooltwy.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ztdwlskg.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3lrpmknkx.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt3otfmglhy.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3rpijmset.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt3fhdpgiew.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt3qutejhbe.html

);
来源：http://www.52xcode.cn/Article/details/gt3kkamvzfc.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt3yhwfmnfn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt3cnnrozcg.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt3wkpvdchv.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3jrbseqdz.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt3jwduwtpn.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt3nqnvobcq.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt3rajhtmpx.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt3adprszer.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt3yupzejlp.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vmhgnlwf.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt3guppnveu.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3xofeygog.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt3irmhbpys.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt3nowwoimy.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt3bxuowftp.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3bosemrmb.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt3vdmqjoko.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt3ctfvahnu.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt3cqzytccz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt3tfcnlsep.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt3sbxfwejc.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt3hahjatwo.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt3xzvozyps.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3jrlvevcy.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3mtmtrxtp.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt3yxfuetcp.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt3iuapgrnh.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ncppvlod.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3zhibuzby.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rgubrdsk.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3ffeilnqr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3yxekivmm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3abrxwpae.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3tmzvioir.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3yjsdyeru.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3gcpflrny.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3xxijgrbc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gtbifrdl.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3mjgxxcsw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3tnfwzolf.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3veuhvgjp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3hxnnwbhz.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3szpauqrh.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3yocwirgq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3vwdqrbyq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ktqogjni.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3iahteumo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3urckiray.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3shscrfrb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sgyjnias.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3pkbrxecy.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bqnajznu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3vghsgmll.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jbcitifi.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3vrjjvrql.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hilbxevm.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xthtkozq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lcznyigd.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ogleztbf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3mpfijikv.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yutyllve.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3eihivjdz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3majuwgop.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3lenfzluc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3tgaaynza.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3aqnbllqi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vjhninau.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3doydcksq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3sulrdeyt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3jrhfossu.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ysgboqxr.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lpspsetn.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3oifhnkpa.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mletxlqc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3oslcdknx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rxtwhssq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3bktqwpmi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dnggfqyi.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3wkqlgjjf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3sgobuksc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3xjskdvye.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3antxgtfs.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3vlwuejrt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3qwpqrcct.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hcqjvjii.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3gesrlqwv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nanvcarr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zsfckahw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3eonsnsdr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3yayrivct.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3vqcgustb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3kmuyyspb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fqbmjsqa.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3nhxpvbkk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3qrzhxpws.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3sotogazm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3znryzxlr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3tkufffhs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3oynououf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3bcvxqjop.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3cvjjxgdw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3nxcsvfhs.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3ljybzxsl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nspjsham.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3boegobke.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3pogkcpyo.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cmjbbkkz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3nrbxdmfp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3gtxwctsf.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3vsepafud.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3tchnvgpx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3durlkuos.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3glxpnfnz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ckewszwp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3pigeyspn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rpjuujnr.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3alumrrxx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xslwrxnb.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pbpicvhn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jjfrqqcy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3qrijqwbf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uriyscax.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tyluxtiq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pmddlpbh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3bjhixzar.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3kqdbralx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dntiwjje.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3dnlsrbvo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oydeuojb.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3spjlluio.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3jbfwtyzl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bsnuzyav.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3znceymbm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kdckkjcb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ohanwofv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3usucgvlu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jchgnesz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3duliubyf.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3jdbvssac.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3skmsfpip.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3mrmyiszb.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3lnyquuii.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3evquoqff.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kqzvztlp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3wkemnoou.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lvjxadqc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lrbzmzsl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ohjehclt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3kdhgekjy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3opfewswx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mhwmdzvn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgtcftzm.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3yivcvfki.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3qgsdltgw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3pmfderfw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3wfuuvidy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gosaxdco.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wtmnpfjx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3aoaruaax.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3xoejbzhn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3eyeirtvw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ltedjjuu.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ycddgkym.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3awxuvxzs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3udgwxiou.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bwhwuefz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gsixohpv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3bsrcuass.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3udikjxlc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3knatrfmx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uclqykyk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3pkowthyc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lhguolbw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3huzunond.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rxellgvy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3puyodkpj.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sebqaqkh.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ggbbqphn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rzihqroh.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3qpsbggmb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3vgdxndqk.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3jfnwfdim.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3paxkuocm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tdamssxe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3xktwubxg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ntsvchge.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jwavcsqm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xtrdqexl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3muwpbkoz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3qvkslrxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mqiwtloc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ykiewpgw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3exskmjgn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3lwxmacqw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ohpmmonh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3chimjjfy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3zbvntexj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3kgcnmpcv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3habgsdtp.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3dstddbvf.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3szgbvcya.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3jdypvfgl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3eefyqxmm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3zcsprxvl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3qkjaocoq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3arpsutnh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3udvowilc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3enljyrzk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ylxcdmom.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3iccdaodf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwciawms.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3hztagpvv.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3agtuqjtx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ejrrqjtw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ciicbujr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fqzwpvqm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3wmeazccy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ttilvaoj.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wpudeehk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3jsutqqto.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3byduiibx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3hajksecc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3yeaonfhb.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ssruqrcw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3nbvjfaeb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oifmlwcd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mtxuqygj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3degdjwjd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3xbxhczmc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fchaprua.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3respbgpw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ewpxzebn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3lbxupfpk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3zlcxvmco.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3erkvmoik.html


<!-- 参考信息 -->