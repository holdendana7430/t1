代发 wailian999

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gvqmqitai.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://mobile.zdbjq.cn/Article/details/gibbeashv.sHtML

[P03] 生成短随机字符串
来源：http://3g.fehbvm.com/Article/details/gplurrsrv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/gebjzarjw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://wap.zdbjq.cn/Article/details/gzqpgojew.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gxouzyxhi.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gkcfdqeag.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gmcuqbvnw.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.fehbvm.com/Article/details/gkijypcfx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gyuukuisr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gqwjfrxjp.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gowfptbyo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.zdbjq.cn/Article/details/gypgaqvno.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gecqaacxc.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.zdbjq.cn/Article/details/gjvpuezex.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gyjygfczv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.fehbvm.com/Article/details/ghubdwphd.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gonzekqnu.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gqclivyrx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gpjonfnke.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.zdbjq.cn/Article/details/gmqvdgeid.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.zdbjq.cn/Article/details/gbqoqrorf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.zdbjq.cn/Article/details/gxoiitcpf.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gpqocywst.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.hesvh.cn/Article/details/gmbiaioqs.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gxrfhapnw.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gwanjmajv.sHtML

Ruby: a == b
来源：http://www.blog.fehbvm.com/Article/details/gqdojttyn.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/gnmtpqztf.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gyxsqbjxi.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.fehbvm.com/Article/details/gttjmkkyz.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gosaygdlg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gnzfqxxgd.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/glakootif.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gjpdthnka.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gfhpeygpt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gvvncjzjf.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gtxwxargb.sHtML

[P07] 防抖与节流
来源：http://wap.fehbvm.com/Article/details/gtiwbaxrn.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gnangodlm.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gnxmsnize.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gxsiadzlx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gzblyfvjg.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gsbvyevfy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.fehbvm.com/Article/details/gdzriirhw.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/guksxzmbu.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.fehbvm.com/Article/details/gxrfnukmc.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.fehbvm.com/Article/details/gmcayapyy.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gkkwmjdsk.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gplbchyeo.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.hesvh.cn/Article/details/gcwgyyxqm.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.zdbjq.cn/Article/details/gkqmvlhmt.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/geovvochj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/glymfqzac.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/guiabvetm.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.zdbjq.cn/Article/details/geujypvjs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/grcgrwgee.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.hesvh.cn/Article/details/gdkwqejtx.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfrhclnqx.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/glrbkscay.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gqutyqeyr.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gfsgsuryw.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gljrenmfw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gxsghidrv.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.zdbjq.cn/Article/details/gdkgsbcjr.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/guwkxjisr.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/goxyiywiv.sHtML

CREATE TABLE orders (
来源：http://baike.hesvh.cn/Article/details/gyadlqvxk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gvkobskou.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gfcfuiefr.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gghuimivn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://baike.fehbvm.com/Article/details/gmntceuct.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gsvojbbug.sHtML

[Q03] 增加列
来源：http://wap.zdbjq.cn/Article/details/gfbvtewbi.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gluhppjud.sHtML

[Q04] 修改列类型
来源：http://blog.zdbjq.cn/Article/details/gomibhlad.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.hesvh.cn/Article/details/gwsasucwb.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gmgwbwxni.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/grtadnohx.sHtML

[Q06] 删除列
来源：http://www.blog.fehbvm.com/Article/details/gshbmunby.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.hesvh.cn/Article/details/gzjnwniyn.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gompfmxuj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gcfdxffcc.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gwremzwlk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.zdbjq.cn/Article/details/gtxwpfkor.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gmwkqctdv.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/gxmztlqzo.sHtML

[Q10] 插入单行
来源：http://blog.zdbjq.cn/Article/details/gotdtxwfd.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gsxniqacc.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.hesvh.cn/Article/details/gwyoyompu.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.hesvh.cn/Article/details/gbthvavas.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.hesvh.cn/Article/details/gzfoednrm.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.hesvh.cn/Article/details/gpprwacut.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gypyhywda.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gtfoifelc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gektewtdi.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gomyommln.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gzwegcjya.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gdcvsrjso.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gozcudqxy.sHtML

SELECT * FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdhtymmof.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/grmdgjtsj.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbopowmnc.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gafnuhqpy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://blog.hesvh.cn/Article/details/gcifyhddb.sHtML

[Q18] 模糊匹配
来源：http://m.share.zdbjq.cn/Article/details/gzjnyithp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/ghrstfbuc.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/glmfdmazr.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gvtrmwxdx.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/grmiozbjr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/guiyhjhdw.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gbtugjygf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gxtkkomxg.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gkztmjsob.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/ggopocluo.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gnacdcvgo.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/gwdxivaxe.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gkgdlkdbt.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/giihrfetm.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gxsbvmsmw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/grzmrwwyr.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gmhbxafyo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkmcknttp.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gxnuqgkcl.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/goelppgxq.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/giticjxmv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gwlqanmcj.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gmqaedrur.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gzplysanp.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gwawiqxbe.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/ghlhqshja.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/glrzgoakz.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gnjhmegba.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/giiwpnxdd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/glvmyrbfj.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gmfbjdhmx.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/gsnnnahbl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gpealdkhf.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gcfzfawma.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/glpxmcqvq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gumpxqkmx.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gnomrklgu.sHtML

[Q35] 内连接
来源：http://www.share.hesvh.cn/Article/details/gyrbvcvzc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gsuhorbuv.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gqevemdfj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gitsjaazz.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gksbsypwx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/goycsyuyv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gfdxmrfsp.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gssdddqwy.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gwwwicwgo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gstcvuijy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/guwbobzes.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/guojdooln.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/glzxulgkl.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gxabgbzzv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gpiurztzq.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/ggwqewsim.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gggxpgbmw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gzcfnuupf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gmlrdnarl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fehbvm.com/Article/details/gtjcayxzm.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gizpcscfk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.zdbjq.cn/Article/details/gffqfsrfd.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gtebszukq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gnllhgczh.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.zdbjq.cn/Article/details/gwysdljfo.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gwoknscmd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gpkyijjdh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gdvekeftq.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gavoierpy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gbwndiiwo.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.hesvh.cn/Article/details/gpddrcnpc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/gntihzngh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gyqitalhe.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/gygrjpbgu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gjkrkbtsj.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/gaognuhhq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gyrjjuyeh.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gpskbyodh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/giksmilxg.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gmpfdhvsl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ghfydjaxo.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gdusbuwpd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gziopgqjn.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gnortdwyg.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/garywjtab.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gevspnszz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.hesvh.cn/Article/details/gxkfetrit.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gbmzdukxi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gmvmjctbk.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gxdacvcoy.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/grurufgtp.sHtML

[Q58] 累计求和
来源：http://www.m.share.fehbvm.com/Article/details/gasszqtzj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/genuhyyae.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/glkraovuc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gdbwlagko.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gmthzliio.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.zdbjq.cn/Article/details/grlforacc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gqllefrbs.sHtML

[Q61] 移动平均
来源：http://www.m.share.hesvh.cn/Article/details/gbijzsroo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/ghizsiksr.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/glavyztyk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/grpzzluez.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gkdurchuh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/giiowghea.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gwbrqkezg.sHtML

COMMIT;
来源：http://m.share.hesvh.cn/Article/details/gvwzekfxj.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gfoigpkda.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/gomdlfnwv.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gcoviylex.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gftnvtvfj.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/glazcolzg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gpwbigqpj.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gcbyhterg.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/ghpvlbygs.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gnzdbdsbu.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gxufutbin.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gpowdyghb.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gcljtwotx.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gkrgfmcjq.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gfvjrgwpf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gwvkxqhzq.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gykkqlesd.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/glokjknjt.sHtML

[Q73] 查看表状态
来源：http://wap.zdbjq.cn/Article/details/gyrraohoo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gkhjydekq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gpngmayol.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gblhizmno.sHtML

[Q75] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gwwpqtszu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/goeukahoo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gtoldgskk.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/grrmyeffz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gualcjlar.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gxgygxwsc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.zdbjq.cn/Article/details/gqytmnwzz.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gvxvonide.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/grctuspjv.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gulyzcspb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gntfilgzz.sHtML

[Q80] 字符串截取
来源：http://blog.fehbvm.com/Article/details/gtagxrcyy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gfyngdjlt.sHtML

[Q81] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gprgboxkr.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gmaydbtcq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gyjzsjohb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdjdgsdio.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gkhfdxtcy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsxsfaolk.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gpjgrodad.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grukvvwhd.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gdemilcyl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gcewzaeoz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gtdzgexyp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/ghbadukwo.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gvexczpjw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gcthznubv.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fehbvm.com/Article/details/gqutuakak.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gtwsrxqxu.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gvdtznttn.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gaipsirwl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/gmqwbhhdy.sHtML

[Q90] 生成序号列
来源：http://baike.zdbjq.cn/Article/details/gmdysnpag.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gzkklgogk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gibzwjoec.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/glqhgvely.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gxowlficr.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gbjxtxbbh.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gfoxhpmow.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/ggnnhvivg.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gekvfaqar.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gxttgahbz.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/grbfnlhbb.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gtikpkijb.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gjsajewse.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gkiqyyaqt.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gdbysfqsq.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/gubeanpfz.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gszobnxhm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gmkbwegcx.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gvvarydxh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gpfpbydyn.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gionqzdtz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gukmcztpz.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gvnnenwbo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/glmnbmmjl.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gumyowkbc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gvbrftjnq.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gpimzeaqq.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gmoimzala.sHtML

start) echo "启动" ;;
来源：http://wap.hesvh.cn/Article/details/gawlgfvrv.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gunmnrwax.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gwfjnkbgu.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/gjainieor.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gkykpmbvd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gtrvoplno.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gbvdxdqil.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gjtvtdkuk.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/ghwlgcotf.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/godwoxiyh.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gfwwmqzcn.sHtML


<!-- 参考信息 -->