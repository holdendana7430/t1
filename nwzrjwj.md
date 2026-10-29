代发 wailian999

C#:   Parallel.For
来源：http://mobile.zdbjq.cn/Article/details/gxzajkkgj.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gypqyncwg.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gstxgdhjm.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnhbxcpap.sHtML

[P01] 生成 UUID
来源：http://read.share.fehbvm.com/Article/details/gfjamtgwz.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.fehbvm.com/Article/details/gjbjaxxqk.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.zdbjq.cn/Article/details/gsmaxwftn.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/ggufzhruc.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gsoonpjxx.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gdndwcqgs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.fehbvm.com/Article/details/gonvqtfln.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gsrwpphdr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.hesvh.cn/Article/details/gekwhesfe.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gxnhfgfyn.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.hesvh.cn/Article/details/gvlkzulgx.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/greypekjl.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.hesvh.cn/Article/details/ghczxsyhx.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.zdbjq.cn/Article/details/gwguotozx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gkwfbjvpc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.hesvh.cn/Article/details/gidzqofrz.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gsyjitifu.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gptkcpeux.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gveqnyseh.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.fehbvm.com/Article/details/gtehfwkxg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gftwneebn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gphmisoum.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.hesvh.cn/Article/details/ghwxffsoz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gxqnwnhnm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvlvvvz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/ghaioyqwy.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.zdbjq.cn/Article/details/gsewbgkty.sHtML

[P04] 求长度
来源：http://mobile.zdbjq.cn/Article/details/grnnvchhg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.zdbjq.cn/Article/details/gzgbzhazc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdhfhmnpj.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gicyhdmvg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/grhodylgr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gqmuqivkq.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/grwvytial.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/ggscjxvzr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.hesvh.cn/Article/details/gnjidgqkm.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/grgfahkpu.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.hesvh.cn/Article/details/ggvxhdizj.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gerxbozzh.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.fehbvm.com/Article/details/gpjtmmiez.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.fehbvm.com/Article/details/gxjmgkcpj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.fehbvm.com/Article/details/gcvobumpv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/grwlgbfvx.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gygytnebl.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.hesvh.cn/Article/details/gmbqckftg.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/grmnudvmn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/gejtazrou.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gxyoxsmqr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.zdbjq.cn/Article/details/gvnkkzdia.sHtML

TS:   if (x == null) {}
来源：http://www.share.zdbjq.cn/Article/details/gettevxqe.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gozactyvn.sHtML

Go:   if x == nil {}
来源：http://baike.zdbjq.cn/Article/details/gzgcsfuwc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/ggftjysvg.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gvglfqlpz.sHtML

[P07] 防抖与节流
来源：http://3g.hesvh.cn/Article/details/ggrbquwyb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://baike.fehbvm.com/Article/details/gcrjcqtdp.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.fehbvm.com/Article/details/gedgorqiu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gwwyuucpt.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gdrzncbzf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gqwwcmvwi.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/ghbaruplu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gegrznbnx.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.zdbjq.cn/Article/details/gvuzswiul.sHtML

[P08] 处理浮点精度问题
来源：http://3g.zdbjq.cn/Article/details/gojuozwgl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gheuljezz.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.fehbvm.com/Article/details/gulovpgnf.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gogszroyp.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gnvhhnbnj.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/gfettrksc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.fehbvm.com/Article/details/gkeyhkexo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/ghqdmkwhr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gjmqpakvn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfobwofew.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://mobile.zdbjq.cn/Article/details/gyvefoikh.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gqzpatnel.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gkkkotvne.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/glhmzanex.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gukiewaic.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gjblvftmk.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gibbubpim.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/gvtvxzwsj.sHtML

);
来源：http://www.blog.fehbvm.com/Article/details/gavnoodpj.sHtML

[Q02] 创建带外键的表
来源：http://wap.fehbvm.com/Article/details/gubbewvxt.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/guackgubx.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.hesvh.cn/Article/details/gfaejnrme.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gpffjqkps.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.hesvh.cn/Article/details/gegmzuzsy.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/gmryjncxv.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gscieujbz.sHtML

[Q03] 增加列
来源：http://baike.fehbvm.com/Article/details/glxkjzzrz.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.hesvh.cn/Article/details/gfuvifeof.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/ghccaxfiu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gbqoadwly.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gbidnmpvi.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.zdbjq.cn/Article/details/goojirhrx.sHtML

[Q06] 删除列
来源：http://blog.hesvh.cn/Article/details/gszeviydp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.fehbvm.com/Article/details/gxefcdmuo.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gwwpknidj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gmlbiiizr.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gxushqhsw.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gwslrwzwp.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.hesvh.cn/Article/details/gjlgyilig.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://blog.fehbvm.com/Article/details/gajfxduao.sHtML

[Q10] 插入单行
来源：http://3g.zdbjq.cn/Article/details/gsrlrmvbq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/gytkaoqeh.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/gcljqveja.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/glkseytgj.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gphyvrdqn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/gxprdjnor.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/gafaebngs.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gkduhtyio.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.hesvh.cn/Article/details/gllztmpnh.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gofryxlil.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gtanalmld.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.hesvh.cn/Article/details/grukxntzm.sHtML

[Q15] 查询全部
来源：http://www.share.zdbjq.cn/Article/details/grsvsbser.sHtML

SELECT * FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcpxwskye.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gtgoapdsr.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/gffxavamp.sHtML

[Q17] 条件查询
来源：http://baike.zdbjq.cn/Article/details/gsbkxdqwg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.hesvh.cn/Article/details/gwxuzjeeo.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gdopmwtog.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://read.share.zdbjq.cn/Article/details/grvthzpgz.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gwiodhdab.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.fehbvm.com/Article/details/gnmewzogc.sHtML

[Q20] IN 列表
来源：http://wap.hesvh.cn/Article/details/gnpxreueq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/gcjfrengt.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/glitknrye.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/gdolhpuct.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gfzcgbogy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/geturvyaz.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/glzpibqqs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.hesvh.cn/Article/details/gcdtwyinz.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/ggoydqcbp.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gyiboqlgt.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gqtxfhode.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/govoeinfo.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/geanmafte.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/guhcoxlfd.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gnuzhixax.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmjujqvqx.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gixnazpkb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/ghxlyviin.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gjwqmyzly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gafrhnlgk.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gnugfcggq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gcqsagxbj.sHtML

[Q31] 分组后过滤
来源：http://blog.hesvh.cn/Article/details/glogdufiy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gnxzoismd.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fehbvm.com/Article/details/ggovawgkg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gthjqhatb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gwuaedfia.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gjvzyfujw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/guvlgsvxq.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.hesvh.cn/Article/details/gmjzisybn.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gobggqgrr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gyenmqazq.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/grqwoniqy.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/grhhurtoy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gvyqeqhmq.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gllnymhjh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gewjvuwtq.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/ghwfwmrwi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gvrycykck.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gkuoafimh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gzkefyxtb.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gnocpigqu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gngfrxrcy.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/gloxrbfeo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.hesvh.cn/Article/details/gwwyejsth.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gjovyjddt.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gycrjzyup.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gnxeinqff.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gelbqnoki.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gbmvkahip.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/grxcmwiax.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gmeibftgn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gjebfmmep.sHtML

[Q43] 标量子查询
来源：http://www.m.share.zdbjq.cn/Article/details/ggstuyzrt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gohsqwxfi.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/ghfbyxwbu.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gqlumhknt.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gdeysybbi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/guxkgqdew.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/goauhdqdc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gqulozvua.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghygtnsvj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.zdbjq.cn/Article/details/gwqyqopwj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gdgplwmde.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.hesvh.cn/Article/details/gooldhdns.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gihqyxrbf.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gbbrjrhnd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gysydyxod.sHtML

[Q50] 批量更新
来源：http://www.m.share.zdbjq.cn/Article/details/ghytrvgmq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gngkgzlom.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gplmnuods.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gxjmrvtye.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gqwuceijv.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/ggiiqllwc.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gwbyxdeju.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gpncdugga.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gnlwiryhi.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/gvmyjollj.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gfpvrftay.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gpnsjmoam.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.hesvh.cn/Article/details/glxomlkfr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/ghrqmbqjy.sHtML

[Q57] 行号
来源：http://baike.zdbjq.cn/Article/details/gcnbegtuz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gaxcyrmsl.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/grnhkcekq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gkvagqhvn.sHtML

[Q59] 分组内累计
来源：http://baike.zdbjq.cn/Article/details/gsvepitpf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gpzyajxzf.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gaxyfhtpi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gveavswll.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/ghlvfkmuq.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gpuznobol.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtcocojrk.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gdcdlujng.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gaqxodkrj.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gpedsvzkx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/goaiqgtkl.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gsftkbcty.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/gwsjugkqg.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gplepithk.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gstqlujzb.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gjyseaube.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gievjbpyb.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gqmiybbxf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gaesnyzzd.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/grtwxsajt.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gbpyzddqs.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/ggzitumfa.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gpwpbbngf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/geiodmmeb.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/genuaktoy.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/gjcmhsxqp.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gjkgzbsls.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gegdkuyfn.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gxdsrrgzv.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvycjxxej.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gurdflixj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gazvrwtvw.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gdsiwgsdu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gkoqvblex.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gobmgzztx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gsfxzvvjc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/gagjtffjf.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gqjjxrjzs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fehbvm.com/Article/details/gckkwddtw.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gckzihrft.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gbppeikdk.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gpmttsxhl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gftahkiid.sHtML

[Q79] 字符串拼接
来源：http://wap.zdbjq.cn/Article/details/gcamtrvnn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gbuwmioso.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gjzyihihz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gjkjxcptz.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gloqsiqgu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gdxfoqyzw.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/grbjlxodj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gcbdddvig.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gqaudvlaa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gcsusuyfq.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gncuroefi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gkhykkzlo.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gkuelfdnj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gqwnnjfpc.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gfdhjoelb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gtufpyblq.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/glxwziniw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gbdxqgjpq.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gceovpsdw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gxxcgoihd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gzxjjuall.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gojhgdesx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/glrpvaudw.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gjgsqnhkj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gtniywrbh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvvtficmm.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/gbaiaclsq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwfqqkwck.sHtML

[R01] shebang 与严格模式
来源：http://www.share.zdbjq.cn/Article/details/gbrcxeelq.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gqriakgnq.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/gwtxkrizl.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gkseqdupn.sHtML

name="Tom"; echo "$name"
来源：http://mobile.zdbjq.cn/Article/details/gpfgcvzwm.sHtML

[R03] 只读变量
来源：http://read.share.zdbjq.cn/Article/details/gnlcdyhhp.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/glyymkpzk.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gcnaxcwcv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gqqcbrtyu.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gnhqoqxwx.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gukhzilyp.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gqxunowus.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gotqjjoip.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gykvzzrrf.sHtML


<!-- 参考信息 -->