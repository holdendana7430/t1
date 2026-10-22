代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cjfjcyhg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2tjlbkneg.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2usxvjlmd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2shdrcvca.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2rrrvlzwv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hwtcxqsh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gxijeqsz.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qcnrqtps.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2boxgxnaj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hkmexzec.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dygmpddh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2fgbxvqyk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lndhxdil.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pkukcmqy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ghvaeuft.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2yctlmmbo.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2cjdmjloj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mxwcxizz.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2fzmxpgbz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jhwjjiww.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2hohzopdo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ravfjzsc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2eptizxyw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lppdysrz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2vndhxvdd.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2lqjzencv.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bpktjbwo.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qzpkevky.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2lfhhmguv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2njktnviz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gjedcxys.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fhchrftu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2penxzpif.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kosvbapt.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cwzinqcu.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2cqfetslv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2pgflxhsw.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jdlfjrew.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2vjsnikpu.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2gznjvpcs.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wmwlkqni.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2lwvemwkl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2ezdjmxyy.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gadhwufj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2iqbkioqu.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bkpwmyia.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fdebxncq.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pyawzclc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2hpngqatr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2tzqavdlx.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2ujzwwdnu.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hstysjue.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2uutujdiu.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2zfuzwqpx.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zgsnvowx.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2dirjcihv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgfopmev.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tdojefww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ulxrtcti.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2fsxxzqte.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2qualyrto.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sczxoumn.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qqqoxvbi.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2klrszdir.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2civbexkn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2iusshohq.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2lxjelcsq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2rtqobpeb.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mqvphkwd.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2mrmotese.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2wfpcjqfd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2twfiliyj.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2fvsryjhb.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2xtfxtsrw.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2nhnixwqf.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2ighyveik.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zsfstemv.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2kmdlmhiy.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2fjlvzolm.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2jrdpmsyy.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2zjzbrtwa.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2xpphfdui.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mjwtfftp.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2ycuumivw.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2xcjlhyfa.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2erbpoaix.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2drlmetnx.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2vxsdeyua.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2wogxuqgr.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2vwjzzwdy.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wzgfzczr.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2ohqcfwrn.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2izrotydv.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2cfwtnukf.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2rnpoctrw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kgfraajz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2gwgzaelz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2wizpipbm.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2clxxqovu.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2ntugdepr.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rxlrfyio.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2noeqsawx.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2noygzmmo.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2bprcytyw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2xxeuxumd.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wzmjksdc.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2klidutzk.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2dzuewfwx.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2zgoafwyr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2khprhzvl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2hdkcttzj.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2necuxbrl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tciqimfj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2klufxwtv.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zhulhmlp.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2aupiqpel.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2hfnmfcka.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2lktcdlaq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pxfzijkw.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2duhzwdre.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2kmqbainq.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fhfjcngz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2snzbhutq.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2seodainb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tjsmtpfk.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2nqhpwklc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tlomwpev.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2lfpjurgn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rkeuniiv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2ljwrbbrv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cnzkexox.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dqxoopnz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ezrllpnu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2yzfjkaab.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2pipcltse.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ruovuseq.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2idgcuuuj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ghrnmfgx.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uxcjfbma.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2dahjuewp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2qmfvqitb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rtprscdx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zsodityn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2fxdgxkxn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2oktevxax.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gtrhtujw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yvkitvqi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2izmykpsq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zwiqilbz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fahramby.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hkgumxbf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2scbcrpsr.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fylsxyxx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2uglhjmrd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vsvjmclr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2oqsxlsdb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cwomonqv.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2xqfcrdyf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2jlkyqgzx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2yoizrrga.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2uyfwfkkq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2slcjkefn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rltrhvzy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2kqardeie.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2xkkvkdgx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2coalmzch.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ijhjdszl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2gdyscezj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2xelvvzaw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dceoword.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2alggbnvx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2xaajhyhh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kyravhei.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2tcvguheh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2qbxrrowm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qafyprhi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yrxebfhk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jblhbear.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2yxarwycd.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2syohwujo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2volinylq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2usywagds.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2pselyfqw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gckwedek.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ltfbiqiu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fcsqbvfa.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jhvjhhmp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2utptncks.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ocvuhyio.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2mcvvhpis.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2nlwrlpcu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2auspxgzt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wxkkmkfz.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vkkruiuk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kmhdpjri.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2yanxtpuh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eggbdscq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hybbhjik.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ajwggsry.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cojjjtfj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ijuerhly.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yaevplyx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2msqgrolx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ulywcbve.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2dpqbprdr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yxyhywmu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kppbwlip.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2tphibauz.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pxqygvyu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mlavuubh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2kbmgxfps.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2fwkcwckz.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zzagvndq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2riczlofn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2uzkdnmsw.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2zyffcwvq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qczxtdfk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qtoqzkiu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vohtpwwc.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2pfbebvpk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2muexhgjy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2fohajwto.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2bfcbunhr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2croxviit.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tidzdkri.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hdhnyvfr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oenjoapv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2xzwpciik.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2ergygtiq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fiexnrvn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gmcbyikc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2xridiocq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tryjavcp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2amucudpv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dgrmqtep.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2nqashhhq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2aslslbga.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jzzjsypz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jwxunfvt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2sqplcsvf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hqchqzle.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uatzksyg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lileyqaa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zajbrhbe.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xpqpqbxb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlwidfia.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tixpusad.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pewacwsn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2yxkcptpg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2paejjzjs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ghsoabnu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kqtgbxxz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ayquznvt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2cthpjxti.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2uxyqjpby.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2jfpukoim.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dviyqnxh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2jyehvfwu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ykuntdwm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2xaqjpymx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2efoudwrb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hipiafjd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2swdjbovh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vmvzyqdk.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jrneftqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2srsrfyjb.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2sbkrbvpp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2rbbauryt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2mpxdvhzs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2evigzipt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lfgwsowm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2zwpnevva.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2uryfqczx.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2guttmaid.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fxwshgdf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2lkmsyvzg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2vyluhehm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2snovdrxq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpksumwq.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zpbpjhpe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2aefpyqlq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ouiyahrp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2otjrftgs.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2wvqysstv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ganzwlca.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bdnbjsem.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ghjbvfgq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2wqakepqn.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yafatlut.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2canhjzsx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2pmdddlix.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2odvfcmji.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lwjovzjh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nfckfdoe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2fmeczlob.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2wmgwgmaf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uqvtsggy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kvrbevjx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2aeaznksy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2pgszwdwu.html


<!-- 参考信息 -->