代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gkshfxotc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.hesvh.cn/Article/details/gldpkvnek.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gtmdorsqr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.zdbjq.cn/Article/details/glburkgok.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gwexcijcr.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gcfjauznd.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gvlupfshq.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gacxebceb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/gkepwazcn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://baike.hesvh.cn/Article/details/gjxbbzvso.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/ghmduualr.sHtML

[P04] 求长度
来源：http://www.blog.fehbvm.com/Article/details/gqdqqlqtw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.fehbvm.com/Article/details/gnfyxfbwi.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/gjqxuhqjg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gzyiluaqa.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gvykjckqt.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/grhppwtyv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gclvlkelb.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gbbkyvbio.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/geqrksytt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/goatadjuu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/ghtzenokx.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gjevfmpuu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.zdbjq.cn/Article/details/gfismeyxy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gmghhjwbk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gfmkscrnq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://read.share.zdbjq.cn/Article/details/gmbngugpu.sHtML

Ruby: a == b
来源：http://www.share.hesvh.cn/Article/details/gnoupgjmi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.fehbvm.com/Article/details/gvmtowsyn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.fehbvm.com/Article/details/gfawiadzn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://m.share.hesvh.cn/Article/details/gnwijacvj.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.fehbvm.com/Article/details/gebhzgked.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gkuyvgxwn.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gubrejkns.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://baike.fehbvm.com/Article/details/geqbtftsd.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gdlzernsj.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gjrvyztqr.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gqobavcvl.sHtML

[P07] 防抖与节流
来源：http://www.share.zdbjq.cn/Article/details/gftbhbagj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gbqqwcjqh.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/gvdefryky.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gxtdtticf.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.fehbvm.com/Article/details/grevbvxcj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.share.hesvh.cn/Article/details/glmvniaib.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gvpyksrot.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gxdblmbvk.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gcmyckbkj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.hesvh.cn/Article/details/grucrzbos.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gtqjbowkn.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/ghnksarkm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gtnvohgqx.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.fehbvm.com/Article/details/gcrlerktz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.zdbjq.cn/Article/details/gixlehohf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.fehbvm.com/Article/details/gptavwads.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.zdbjq.cn/Article/details/gisaigypr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/ggxvhrmya.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gchazgnjp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.zdbjq.cn/Article/details/gfweignxo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggxubkbxe.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gbrzcrurp.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/goplxvkpg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gwzphqedp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.zdbjq.cn/Article/details/ghsrwgges.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gkzftcaki.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/grwdpuyga.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gqqnnsgjt.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gkajkpytm.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/ghpenzmyq.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gkrdsfmyo.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gyjuumtay.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gpbbiwfrd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.zdbjq.cn/Article/details/gwsxvhqqn.sHtML

);
来源：http://baike.hesvh.cn/Article/details/gzmhdfecg.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/gxkjfmlfe.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.fehbvm.com/Article/details/guapcufsd.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/gtpgmuirr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gqykpxqct.sHtML

[Q05] 重命名列
来源：http://www.blog.fehbvm.com/Article/details/gthjzafsu.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.hesvh.cn/Article/details/gmohdpdjy.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/gbftppzdn.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gfcxipdqf.sHtML

[Q07] 删除表
来源：http://mobile.zdbjq.cn/Article/details/gwgjttvsp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/ghibcuskr.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/grvnbuuae.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gfixgziyy.sHtML

[Q09] 创建唯一索引
来源：http://wap.fehbvm.com/Article/details/glqqtvwwq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gzakuqtfe.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gueuinqmu.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.zdbjq.cn/Article/details/gzfjbdmsh.sHtML

[Q11] 一次插入多行
来源：http://read.share.fehbvm.com/Article/details/gpgwpjoux.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.fehbvm.com/Article/details/gqznwepxs.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/ggvxhtwpe.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gvnroddpy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://read.share.fehbvm.com/Article/details/gzjfhurue.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/ggzwnadfc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.share.hesvh.cn/Article/details/gzfwhirmi.sHtML

[Q14] 存在则更新（upsert）
来源：http://3g.fehbvm.com/Article/details/gozkbprxo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/ggunilgid.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/gvnnuwycy.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gcmhdcpwk.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gguwzksog.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gyiuglkdl.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmkuwssyu.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gkqjtlyqu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/grebfeenh.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gpzqhjbko.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gotymevoo.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gtcbnbyyc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/gtxvsxjdk.sHtML

[Q20] IN 列表
来源：http://www.blog.zdbjq.cn/Article/details/gjmcdsvek.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.hesvh.cn/Article/details/grwzowmjq.sHtML

[Q21] 空值判断
来源：http://m.share.zdbjq.cn/Article/details/gfrdzgkik.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gpdzjqqdp.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gufjjvuor.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.fehbvm.com/Article/details/gqvfjqrqz.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gmassiryy.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gysqorccs.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gfvysfwuj.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/gnkiomdsw.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gqgranltb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gerxzliar.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gxcqgukog.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ganowctdj.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gmzlfrzmm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gbuddmwtd.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gtrzkqozq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gfcuqanlx.sHtML

[Q29] 最大最小值
来源：http://wap.fehbvm.com/Article/details/gwponkjma.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/ghpwtutcw.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/godjcwsxw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gmvpybszd.sHtML

[Q31] 分组后过滤
来源：http://baike.hesvh.cn/Article/details/ggitevqim.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gajcwwjqu.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gopzrvwcl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gnynmmzor.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gljcujofn.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/ghfxacxsq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gzlroqvcs.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gfkmeurwb.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gwbexnzem.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/grrhrbxyy.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/giuslndcb.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gtdbbungk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gwaknvgsf.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gotcfnegk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gvkkpeqgl.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gppwvkzpu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gwzbtqhmy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/goonapgvo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gkqqkuxok.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/galglyvhp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/grtfhbzan.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gwettrfpx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gvzmvlgew.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.hesvh.cn/Article/details/gjwpghjjm.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gjuznmolc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/ghzpnobnr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gxzmurgzc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gjghhhbcl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gszryytgp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gathgclgj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.hesvh.cn/Article/details/gjobphghz.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gexvmwpor.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/glnipelcj.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/giarnvbaa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gpzzmzxbc.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gjovuwsmd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/gghjjqemm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gvsfugtjy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/grseiimat.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gmxtifjie.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/glmedlqim.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gxvktwjpd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/gupvvoslu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gbpkfnesp.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/gszcvramn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/grlqryxhq.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gzkigmetx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gfjpmydtz.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gwhgnzdoo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfpwfcuts.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gzttzpdgv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gvjbtmrsz.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/glcmzjtoh.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gsoomrekd.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/guzaxxrtq.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gyxfxgrxk.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gwaegzizo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gkqsvnphf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.hesvh.cn/Article/details/geihmqawe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gdomprrej.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gcvymilyb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxhxkpwhx.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/goutvnvli.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gifimxtmk.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gianddcfy.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.hesvh.cn/Article/details/geelxjlpz.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gyptdahos.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.hesvh.cn/Article/details/gsoiixegf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gbdbtpfgl.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/ggkospksq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqznkzkov.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gjeaweitj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/ggzfamohe.sHtML

[Q63] 开启事务
来源：http://3g.zdbjq.cn/Article/details/glrgbfkrs.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gtmlmpxul.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gsvqbeizk.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gkoqguabq.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gptbgdrba.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/ghyvcecgs.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gavfjzsnz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/guhcvfaun.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gqmwszkuc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gtzfazpxe.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gwvrrbqxl.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gdsmxoipt.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gjdjtizfw.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gkrsllgom.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gbjngmbrd.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.zdbjq.cn/Article/details/gjlkiqhzt.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.zdbjq.cn/Article/details/gcgxuwtmg.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gekvfgacg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gaayigitm.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gzlzksojs.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbqioqrzb.sHtML

[Q73] 查看表状态
来源：http://baike.zdbjq.cn/Article/details/gabffssba.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gwdbjalmn.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gedscxqsc.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/ghghxiisu.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gyquwoolb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gunzagewy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.hesvh.cn/Article/details/gdayeooij.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/gudlgumef.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gxpgjyera.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gnksphzje.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gtrrhqwyg.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gcmfzcyjj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gmhnznpan.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gfblwmgfh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gftiegnjx.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gjjodrbkz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gnkvkbnkr.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gnpjabclx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gcouyfumq.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gmtbsujeh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geyrckdhs.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gptfhqumi.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gcmyvduko.sHtML

[Q84] 去除首尾空格
来源：http://baike.hesvh.cn/Article/details/gqolcydsm.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbkqxtsuh.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gnaebiexf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gsqmkiwje.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/geejohoxz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gtkfktbiq.sHtML

[Q87] JSON 字段做条件
来源：http://blog.zdbjq.cn/Article/details/gblquhakz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gzdmmwihw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.zdbjq.cn/Article/details/gyrqtwzjk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fehbvm.com/Article/details/gnfeoppkf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdlrikhqo.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gayzesumz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gmrlrevgq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gkxsunrzh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/ggtfnyaxg.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gghroaywx.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gpupqmvhn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gozepsxvs.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gxhuxqysv.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gqyrnurlt.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/grhevaweq.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gpvryljfy.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/gyjeqhiww.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/grzwhbmty.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gsmdhioii.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gjhyreugj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fehbvm.com/Article/details/gbwifjccr.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gecqadjle.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gohbihdcz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/glrltvwlx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/gevcfyrli.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/grvwuzwln.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gxssikvkj.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/glikvkwfg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gqijtqtqx.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/gyyphwkli.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/ghtzrmceh.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/geeupygbv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/glxmjniqy.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gjaqliydh.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/giywesvpw.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gxrpdubap.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gcoaqsqdh.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gynldakpi.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gbovzszeu.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gtashzmro.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fehbvm.com/Article/details/gfaocotik.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gnyaqgcfe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/ghqojeoro.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gpbqkoque.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gtstvrtfm.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gdtdiffvr.sHtML


<!-- 参考信息 -->