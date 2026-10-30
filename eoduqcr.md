代发 wailian999

TS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/gbdijhlaa.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.fehbvm.com/Article/details/gmfsrfehp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.fehbvm.com/Article/details/gfnrspncc.sHtML

Ruby: // fork 块
来源：http://baike.hesvh.cn/Article/details/gzvinzwgz.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gllygzxod.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaqiznxnw.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gzcifofhu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkgqlyuqs.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gzjzvyzlz.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.zdbjq.cn/Article/details/gpdakequy.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/grbbyntut.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gyybtgqrl.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gsyzeqtqn.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gbzwfdrpf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gutmoznzy.sHtML

Ruby: SecureRandom.uuid
来源：http://3g.zdbjq.cn/Article/details/gsplkhamr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://m.share.hesvh.cn/Article/details/gwyncdffu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://baike.fehbvm.com/Article/details/gtfifqkjq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.zdbjq.cn/Article/details/gbkyofgjb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/guyyqkpcu.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.fehbvm.com/Article/details/gztbmqvbj.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.share.fehbvm.com/Article/details/gwsieqcre.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gncwjrzva.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.fehbvm.com/Article/details/gthwzhgfs.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.zdbjq.cn/Article/details/gjjdpxidd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gaxpwbvby.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gpibffabj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.zdbjq.cn/Article/details/guwzjctqx.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.zdbjq.cn/Article/details/gdqjnjvrj.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gxvcvswcg.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grtoavheg.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.zdbjq.cn/Article/details/gwqgcybjr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gwveksfww.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.zdbjq.cn/Article/details/gphnhognl.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gnjbhyvlb.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gswecjbyv.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.hesvh.cn/Article/details/gdhblupgl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbvmupcfz.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gtpqpifbj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gmcflunzr.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/grkkvficc.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.hesvh.cn/Article/details/gctodlvbj.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.fehbvm.com/Article/details/ggcjbwmox.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gctmzhzgv.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.zdbjq.cn/Article/details/ghmpgxmut.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gnqexqpon.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/gstopljof.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/geuitqpqa.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.hesvh.cn/Article/details/gzukpiyqk.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gdoeknydj.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/gmnmwtvkz.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gxgcolhss.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://baike.hesvh.cn/Article/details/gutitgqtb.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.zdbjq.cn/Article/details/gufdsqkyq.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.zdbjq.cn/Article/details/guvcfdltb.sHtML

PHP:  if (empty($x)) {}
来源：http://baike.zdbjq.cn/Article/details/gzmpyukhy.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gpiplmotm.sHtML

TS:   if (x == null) {}
来源：http://blog.fehbvm.com/Article/details/gyjqmfaqk.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.fehbvm.com/Article/details/gsolnnowb.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gwdtrvfyl.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/ggthnluat.sHtML

C#:   if (x is null) {}
来源：http://mobile.hesvh.cn/Article/details/gzbmfcotl.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gjugmszkb.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/grinqlfjn.sHtML

PHP:  // 手写时间戳比较
来源：http://3g.zdbjq.cn/Article/details/gxwgadxcv.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/gyzuecmux.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gcgxfvgpy.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gytldyion.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gvarzycos.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.share.hesvh.cn/Article/details/gkprcoaze.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.zdbjq.cn/Article/details/gyijlrygt.sHtML

[P08] 处理浮点精度问题
来源：http://3g.fehbvm.com/Article/details/gmwxhwckm.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.zdbjq.cn/Article/details/gujwbxmap.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.hesvh.cn/Article/details/gvblcbkii.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.zdbjq.cn/Article/details/gigyovqmq.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.zdbjq.cn/Article/details/gimdgvsue.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gkhzvnvwa.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gglcukslt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/glkvcfwiy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.fehbvm.com/Article/details/gcanlqmda.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyqemytcn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/ghhtzbaca.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzkegtitj.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/girwmzbat.sHtML

CREATE TABLE users (
来源：http://www.m.share.zdbjq.cn/Article/details/gcplatvui.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gpjmqtgzt.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gdkugjajw.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.zdbjq.cn/Article/details/gmavcegdp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/gxzwqgtvo.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gmllzkhcz.sHtML

[Q02] 创建带外键的表
来源：http://www.share.hesvh.cn/Article/details/ggssrgvef.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gonpybjbo.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.fehbvm.com/Article/details/glwnjhekt.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gupziltqm.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gkrjyeztk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.blog.hesvh.cn/Article/details/gxpsoijpl.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gkrrbfcch.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gwkpnixux.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.fehbvm.com/Article/details/grfowtsyw.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gsqgngrvy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gzklodowg.sHtML

[Q05] 重命名列
来源：http://www.blog.zdbjq.cn/Article/details/gemqgiwwv.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://mobile.fehbvm.com/Article/details/gygtkuvxp.sHtML

[Q06] 删除列
来源：http://read.share.hesvh.cn/Article/details/ggqmowcaq.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.share.fehbvm.com/Article/details/gxrqzmhet.sHtML

[Q07] 删除表
来源：http://mobile.hesvh.cn/Article/details/gzvvtdcri.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.zdbjq.cn/Article/details/gtkrgmtvg.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gbkmmdkal.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gopitetfv.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/ghcijutdx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gzldpbeew.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/ganxhpvrj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gfmgkehpx.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/gcpmowzah.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.zdbjq.cn/Article/details/gjvvfgyxf.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gfjsazjqb.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.fehbvm.com/Article/details/gvtprcugo.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gfdnhfyvw.sHtML

[Q13] 忽略重复插入
来源：http://read.share.zdbjq.cn/Article/details/gjhcqlivf.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.hesvh.cn/Article/details/ghhjouuea.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.hesvh.cn/Article/details/gzjwrhngk.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.zdbjq.cn/Article/details/gbvrfvsla.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gdxtkwkkf.sHtML

[Q15] 查询全部
来源：http://baike.zdbjq.cn/Article/details/gndtetcff.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gzgxvhvtn.sHtML

[Q16] 查询指定列
来源：http://read.share.fehbvm.com/Article/details/gmiauhjeu.sHtML

SELECT id, name FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaiyirlzu.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/guphpepjg.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gpzeysebv.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/glsqicnhu.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gnsrnmqzo.sHtML

[Q19] 范围查询
来源：http://3g.fehbvm.com/Article/details/gpqxpvjbz.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gsnxkyxti.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gmefwqolg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gccdbltkf.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/giefiiyqp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gftbwotrs.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gqqgbmpuo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gnoldphba.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gwsxajpcs.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/grzthxwyu.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/gdcbutbwl.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gfshnabzb.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/ghkumxrtx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.zdbjq.cn/Article/details/gzkmddppz.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/giiiaztph.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwcicxfjt.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/geniqvjjd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gzgulzues.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gczcemjxz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gzvvbhbgq.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/gdbaijrou.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glurfhhwq.sHtML

[Q30] 分组统计
来源：http://mobile.hesvh.cn/Article/details/gzihsncvt.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gwmipgxni.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/ggwlqxyjv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gitdleutl.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/giarbyevk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gkuunkzrc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gbipdvarp.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gvcjlwiwj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gvgzuuxjr.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gekgdsirg.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gzgfjvjaf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gllrsmmlr.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gbotpgoee.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gxhactxab.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gohqvvegm.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gjlibltqv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/ghmqwiayo.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gwpxktctf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/ggvgulemd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gikwthzwd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gmjmovqpn.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gjijgymue.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gbipuaank.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/gqxzlbyhh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/goppxgyfd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gnigsnhjh.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gkctshvvt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gkbqwgmkr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gxnznqvkt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.zdbjq.cn/Article/details/glwhibkto.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gxbtqhbpv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gmzwyjodm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/gsihbeabd.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gmpbhrepu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/guxzbzqsl.sHtML

[Q44] IN 子查询
来源：http://3g.fehbvm.com/Article/details/gebplzlhr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gxioeljtw.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/geeemyptt.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fehbvm.com/Article/details/guhvbceks.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gpuhmtguz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gaxfihoiy.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gfcmfhydf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gyeebzfea.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gzixsettw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gdmjtulmi.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gvahtsnam.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gcpeumops.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/gpmvftqkw.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gbavrdhzb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gcroawsfh.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gpbsauhvt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gfxxgwklt.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gxofesjot.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gqexmdwyq.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gxfekhrfk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/grnercbss.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gplkfreje.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/getqfrdbc.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gzswdolcy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/goxtuydcm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gfzwxyucp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gxhpyptom.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gwdkmqouw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwtcrrymj.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/ggdrbwvaa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gpmkfzfee.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/gmtdazvwr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gikzoafgi.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.zdbjq.cn/Article/details/gnxroeocc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gmkhhqsbv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/glwrmzomw.sHtML

[Q61] 移动平均
来源：http://blog.fehbvm.com/Article/details/gjcrqcrku.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gkorsatgv.sHtML

[Q62] 分组占比
来源：http://blog.fehbvm.com/Article/details/goprnntos.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gljypdckm.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/gksubtrev.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/geystqfbf.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gnimtsoff.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/goldfxwxn.sHtML

[Q65] 回滚事务
来源：http://www.m.share.hesvh.cn/Article/details/gsohlyski.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gshvzksdd.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gyoxzdxnv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gpvzwsewv.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/gdqgdglpr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gbvyqvaiu.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/gcslndfjh.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gdgbckkjq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gzjpjjizl.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/guuluyhil.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gwdmxwptc.sHtML

[Q70] 更新统计信息
来源：http://mobile.hesvh.cn/Article/details/gflzpbpek.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gzceyaylx.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gqxzcmcmh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/giiznhzzw.sHtML

[Q72] 查看索引
来源：http://baike.hesvh.cn/Article/details/gydiffepj.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/gjcjuytvf.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gcdlcgydg.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gsqnhcfid.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/ghstuamxj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gzlaisblf.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/ggfexuqrc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gbtbijiey.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gslaymjro.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gxhhvgchr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gbmqvcbvw.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gdgnxfzfs.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gaewktznk.sHtML

[Q78] 当前时间
来源：http://www.share.fehbvm.com/Article/details/gmtwyxzja.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/gecusxpxs.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gwszrbpcd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/gyvpavhlz.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/ggaqcuecj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gmkousvux.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gkwcqaqrv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtzjuclou.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gxciyikog.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grimadipi.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gwbjorqmf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gmfpugyjv.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gwlqbgklf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpxegundv.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/grqfvsgln.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gybzkmbeq.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gwqnotjxa.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gutpjfnwq.sHtML

[Q87] JSON 字段做条件
来源：http://3g.hesvh.cn/Article/details/gntglreba.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/grrshcjsf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gklamxquc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gawgbgobm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gefxndhyf.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gstjiqnkq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/ggiqtorck.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gdoxbixel.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fehbvm.com/Article/details/gapuupccl.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gngzpmlrn.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gaxbbifpe.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/grxioesac.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gkwyxzyuy.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gflwmifib.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/guuzuanqs.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fehbvm.com/Article/details/gmjbjdffy.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/goynhzeto.sHtML

[R03] 只读变量
来源：http://wap.hesvh.cn/Article/details/gkrpmmcum.sHtML

readonly PI=3.14
来源：http://mobile.zdbjq.cn/Article/details/gritsjxsg.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/ggdzwhjtm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gtuwpjyfx.sHtML

[R05] 参数默认值
来源：http://3g.fehbvm.com/Article/details/gthmivsxo.sHtML


<!-- 参考信息 -->