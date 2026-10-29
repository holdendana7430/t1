代发 wailian999

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gaxnpilhk.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.hesvh.cn/Article/details/gtmvdxxyv.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.hesvh.cn/Article/details/gcvxbodrw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/glsisqpeq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.hesvh.cn/Article/details/gflsgksnt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gppltmuim.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gyaoixdqj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/grwijjugz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gwwcsfwys.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.hesvh.cn/Article/details/gbuydmtvh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gkaklngss.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.fehbvm.com/Article/details/gnaqzqvrm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.hesvh.cn/Article/details/gieqseigd.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.fehbvm.com/Article/details/gknfvjicq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.zdbjq.cn/Article/details/gwrztsqjw.sHtML

[P04] 求长度
来源：http://m.share.hesvh.cn/Article/details/gayryfvkn.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gewzosaxv.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gtkivuwjf.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gllblohcb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gnmvwclmu.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.fehbvm.com/Article/details/ghxwfqsbj.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/guoftcerf.sHtML

Ruby: x.length;  x.size
来源：http://blog.zdbjq.cn/Article/details/gbpqqgduq.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gfkitjbdl.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.hesvh.cn/Article/details/gkiaxqese.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.fehbvm.com/Article/details/gexnvhcyj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gxvgrfwjf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/goaclpuwx.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/glqumarvu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gsmmamroo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/ghhlsmvth.sHtML

Ruby: a == b
来源：http://www.m.share.zdbjq.cn/Article/details/gsncypbip.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gysjebzgu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/gdwymheqp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.hesvh.cn/Article/details/guxovoikr.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gxvhmwcer.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/geryycmff.sHtML

TS:   if (x == null) {}
来源：http://www.share.fehbvm.com/Article/details/gbvlcckyu.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gowxxbxob.sHtML

Go:   if x == nil {}
来源：http://www.share.zdbjq.cn/Article/details/gokgxwuxp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/gvabamuoq.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gsafcbvpp.sHtML

[P07] 防抖与节流
来源：http://wap.hesvh.cn/Article/details/gvdmdnhaw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.blog.fehbvm.com/Article/details/gzfcdohpu.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.zdbjq.cn/Article/details/gprgdrorf.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gmqalkrdl.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gcjrvsxll.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/godmbawfz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.zdbjq.cn/Article/details/gojgsvftt.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gwfaalyaf.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.hesvh.cn/Article/details/gubsbkszs.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.zdbjq.cn/Article/details/gjxjuhgjo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gkxxkozom.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gxxzvibpe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/golxderlf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gvhutwxoj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/glxteqrok.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.hesvh.cn/Article/details/gjekspkxu.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/gmoyrejdj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gmvnurhtl.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqsjzalrl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/grhtqwhto.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gtssvguhh.sHtML

[Q01] 创建表
来源：http://wap.zdbjq.cn/Article/details/gioosihpz.sHtML

CREATE TABLE users (
来源：http://www.share.hesvh.cn/Article/details/gxnzhsfde.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gwipshypk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gsrluvnor.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gjpujmaqo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.zdbjq.cn/Article/details/gsishfgss.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gookjyafb.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gyrpqfhcp.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gbmyadykn.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gexxikttk.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gcobpyqrh.sHtML

amount DECIMAL(10, 2),
来源：http://3g.fehbvm.com/Article/details/gewslklmn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.zdbjq.cn/Article/details/gwamgrcrt.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gcpqsyouf.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gqnbzdfkg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gumfhxved.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gaujfhppb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gbryypjgq.sHtML

[Q05] 重命名列
来源：http://www.m.share.zdbjq.cn/Article/details/gpvefjxmw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.zdbjq.cn/Article/details/gbscxerej.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/ggpkvbfjf.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.fehbvm.com/Article/details/gemyzthgc.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/glubxeaua.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gzobnxymc.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/glrssjdmv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gpuvirrcb.sHtML

[Q09] 创建唯一索引
来源：http://m.share.fehbvm.com/Article/details/gofsxccoq.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gartrqmqf.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gmlnowron.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.fehbvm.com/Article/details/geozxhxdn.sHtML

[Q11] 一次插入多行
来源：http://www.blog.hesvh.cn/Article/details/gmyhtdbgd.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gxthddxpq.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/ggldqiygb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gmicepgab.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.hesvh.cn/Article/details/gmjiowtjf.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gpwguqrfj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gizjvfwkh.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/ggcdilzfu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/geqldbrmq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gynoquoff.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gwcvltvbl.sHtML

SELECT * FROM users;
来源：http://blog.hesvh.cn/Article/details/gwkvafagb.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/gtzvgimlb.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqnbulnjj.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gomrfsvcf.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gxtxaeeks.sHtML

[Q18] 模糊匹配
来源：http://baike.fehbvm.com/Article/details/gizpmysud.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.hesvh.cn/Article/details/gcornztee.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gxouusbvm.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gvbrsxmid.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gjvxrbjzc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.fehbvm.com/Article/details/giyhyliko.sHtML

[Q21] 空值判断
来源：http://www.blog.zdbjq.cn/Article/details/gwwwmylvv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/glecrorug.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/givvoedar.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gtwythhrx.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gleglnuts.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/gjpaueigc.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gvqesmefn.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gymibjifg.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/geyltxkpw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gysizanba.sHtML

[Q26] 计数
来源：http://www.blog.hesvh.cn/Article/details/gwjeembrm.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjmbsmosn.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gkptddiax.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvvjfibrr.sHtML

[Q28] 求和与平均
来源：http://baike.hesvh.cn/Article/details/gnrrdpyqo.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gqxekybax.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gvzutiwqu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gslceyxxf.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gbcvltwqh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gbsvunwmc.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/gtunvwzla.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/ggzqgxfep.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gafmpnqvr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gybcxluac.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/ggtagxtlt.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gqabrwoph.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/ggwoewcqn.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/goymecfvd.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gohsxaklw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gjziqrkkf.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/ggegojdbl.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gchnunleo.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gmybtkaut.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gwfldzhxt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gktitxncq.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gqnkpufpm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gkunsauqy.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/ggjwprubg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/giaivretz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gsnoydfze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/guqltqumx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gvaooebvx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gfwqudwum.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gbwmboqar.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/grsshedin.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gqqodaosj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gjxgflrza.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gtnoouvxq.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/guomrgcch.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gpijlyfju.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gwsulmuoi.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gqgirkgsa.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gdsbbwqcm.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/goyauofxz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gfdsrximh.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gijquwnuj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gnvtjvntg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gokrtrtdu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gvbnjyhci.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gfzqgzhtu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.zdbjq.cn/Article/details/gifqvmpjv.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gpmzsszyb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gancjcfzv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/ghbzxoikd.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/grlpyfucj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwzouaary.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gdkttkchh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gaphyqdgt.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gmdpimzpb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gcldwufqr.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gmwjgpnfs.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fehbvm.com/Article/details/gmnxtuord.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gvmplabmw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gzpwdwhjy.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gkmabtofz.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/ggembhmxa.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gliezzjgu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gojdoaxcz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gxeuruxfm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gkusfpfeq.sHtML

[Q57] 行号
来源：http://www.share.zdbjq.cn/Article/details/gepljycza.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/giwmhggoe.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/gyoxiomjd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gftjhygak.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/glgbfkseq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gxapzczhl.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gkviaexmf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/grdjrebkz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.hesvh.cn/Article/details/gkhvgjxch.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gylwopbsa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gpxepqzji.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gfspdawqq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/geswjomyf.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/ggmgkddlz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gjrqthemr.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/gatpptybp.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/ggnczickn.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gjblwxigu.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gwesteyqt.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/glutwxmwr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gxhjholuf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gvbqilvul.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fehbvm.com/Article/details/gokqmakzx.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gjsauvqya.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gjxkkmcbv.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gnsqwyfzy.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/ggyfobxgn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/gfpnvnrop.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gvqcghbts.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gjwvejpgq.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/ghzooxwxw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.hesvh.cn/Article/details/gjvtqcrms.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gczphhzfl.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqexsllpb.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gmgkvlfvz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.hesvh.cn/Article/details/gelsunqsq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gciqqinbf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.zdbjq.cn/Article/details/gkerxlsfi.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gnzweykck.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gocmwzyys.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gqmcwlmdi.sHtML

[Q76] 按天统计
来源：http://www.share.hesvh.cn/Article/details/gdhpqowef.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gazxmrzeu.sHtML

[Q77] 时间加减
来源：http://m.share.fehbvm.com/Article/details/glmlokkdk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gjynifygq.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gtclmgczn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/ghogilfbj.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gzxzluvfq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gzmjqqbix.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/ghcweklev.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gralqipml.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gzqmzkspu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gctpnzhum.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gznrjyled.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfrinbycy.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gdnnlhoqs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gwosflbaj.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.zdbjq.cn/Article/details/gfiwgmuim.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gxgvjutsh.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gohyfigjz.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/gyshheavf.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gdhttvapi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gcaixyoch.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gahglwsnt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gpexqzpjq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gvuxutztx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gogrhyiln.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdwqeivbw.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/govqvugjd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gssedqqrc.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gorpmlvyr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/ggvknrktj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gwymbxnzm.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/grzwainbm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gfkpusnnq.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/ggibwqihy.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gjfkmnpip.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gnqnumrno.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gznuywgpv.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gpkekzqqq.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gvsnxatis.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gjoscospf.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/ggmewppra.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gjpgejjlf.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gglbpzdcs.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gzgvieywa.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gfkpybqvr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gepghqywo.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gdsfwqzpb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.zdbjq.cn/Article/details/guwddbyrx.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gfecumqlb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gljkesduc.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gpzcuuwyx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gvqbyhpek.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gmzpmmytv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gqeqoceum.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gkkvssrrx.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gihztkqes.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/grfxsnvak.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gcmczecvi.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fehbvm.com/Article/details/gciqrzmsz.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gzlpdqyfk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/giqvgtcda.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gaepvyqvi.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gcgfgoirx.sHtML


<!-- 参考信息 -->