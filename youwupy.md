代发 wailian999

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gptcymsls.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.fehbvm.com/Article/details/gmjbvnkgw.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.fehbvm.com/Article/details/gudhkrhvr.sHtML

JS:   // child_process / cluster 模块
来源：http://baike.hesvh.cn/Article/details/gyoyeyqdy.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/gwxwxhqlw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.fehbvm.com/Article/details/ghbbfdvig.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gyysljyqq.sHtML

Ruby: // fork 块
来源：http://m.share.hesvh.cn/Article/details/goftfcsgf.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gudzftboh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gokqwacmp.sHtML

P. 常用工具函数
来源：http://www.blog.fehbvm.com/Article/details/gllznpqnh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmhqbgymy.sHtML

[P01] 生成 UUID
来源：http://www.m.share.zdbjq.cn/Article/details/gsfgvzqpw.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/ggotmrfzc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fehbvm.com/Article/details/gmpqpqkdq.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gnkmdoyqw.sHtML

TS:   crypto.randomUUID()
来源：http://wap.fehbvm.com/Article/details/gmoenvbaq.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gtyykbwxs.sHtML

Go:   // 用 github.com/google/uuid
来源：http://3g.fehbvm.com/Article/details/gbqwabljb.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.zdbjq.cn/Article/details/gncpywpwy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://mobile.hesvh.cn/Article/details/gblvbtife.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.m.share.hesvh.cn/Article/details/gunhpdhhz.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.share.fehbvm.com/Article/details/ghrdktvaa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gijacalaz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.hesvh.cn/Article/details/gtvcgqnzq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gdckdnigg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.hesvh.cn/Article/details/gqxxljgen.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.hesvh.cn/Article/details/gyifgkvmo.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gwylhmcvt.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/gofscwlcf.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxfvcchja.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.zdbjq.cn/Article/details/gctqnpygw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.hesvh.cn/Article/details/gueswaoih.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/ghnuncgtx.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gwylahpti.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/goewwdvrz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ggelpqzqu.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.zdbjq.cn/Article/details/gyjsaiqpb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gqryyqonj.sHtML

[P04] 求长度
来源：http://www.share.fehbvm.com/Article/details/gwssdhbfw.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.fehbvm.com/Article/details/giywcmmcz.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gkemzdenp.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/grzouvgnk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gbqoopquw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.hesvh.cn/Article/details/gsgmzyxba.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gjcdiokxe.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gfwqnrehx.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.hesvh.cn/Article/details/ggacdsqxg.sHtML

[P05] 判断两个对象内容是否相等
来源：http://m.share.hesvh.cn/Article/details/glzexdhli.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gondhwadt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gugcjdifu.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gdcaifrgd.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gmduskxjr.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.zdbjq.cn/Article/details/gwmvsnviv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/gacnetnqo.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gphrjutdi.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/glijyidet.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.fehbvm.com/Article/details/gmgphdwpl.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gbtzsonbq.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.hesvh.cn/Article/details/gptoglpaz.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.hesvh.cn/Article/details/ggulitszl.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gbvunrbop.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://read.share.zdbjq.cn/Article/details/gkjsykcyu.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gruefxqgt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.zdbjq.cn/Article/details/gesyscest.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/geohryzse.sHtML

[P07] 防抖与节流
来源：http://m.share.fehbvm.com/Article/details/gpgwczbaa.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.fehbvm.com/Article/details/glknubwmh.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gpwvaczfp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gdjmxdspm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gsvjmrosf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.zdbjq.cn/Article/details/gvqxukkox.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.hesvh.cn/Article/details/gudmsvebr.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gchbphsck.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.fehbvm.com/Article/details/gztbzycxm.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gxdsztvus.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gwvpogowo.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.zdbjq.cn/Article/details/gukbekgcw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gbvqkmbiy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gyiyzteoh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.zdbjq.cn/Article/details/ggpcwktzj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gmsxtacye.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://wap.fehbvm.com/Article/details/gnficbqak.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/giyqfvjkc.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gclxeejuw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/ggssiaxnq.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcknsqhmw.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/goluomuvg.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gavywvfic.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.hesvh.cn/Article/details/gpjgqsclf.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gychtbzas.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.fehbvm.com/Article/details/gyaaffucy.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.hesvh.cn/Article/details/glgvvlmpj.sHtML

);
来源：http://baike.fehbvm.com/Article/details/gjoxemqxm.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/groziseio.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gplmddpke.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/ggfafpurq.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gdsenquwl.sHtML

amount DECIMAL(10, 2),
来源：http://www.m.share.zdbjq.cn/Article/details/glgfitnhp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.fehbvm.com/Article/details/gpupmqhih.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gfaiffzgj.sHtML

[Q03] 增加列
来源：http://read.share.zdbjq.cn/Article/details/gemstyhqw.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/gdsgilfnd.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/gyzednzxk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gjylvavff.sHtML

[Q05] 重命名列
来源：http://www.share.fehbvm.com/Article/details/gkfefxxyx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/giferwugk.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/guhaummqp.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://mobile.fehbvm.com/Article/details/geabafxdi.sHtML

[Q07] 删除表
来源：http://m.share.fehbvm.com/Article/details/ghqmunemj.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gnbsjssla.sHtML

[Q08] 创建普通索引
来源：http://baike.zdbjq.cn/Article/details/gejsncdqi.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gyaxjwibg.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gzcnnhgba.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/ghlfjqfdo.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/griebjfpb.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://read.share.zdbjq.cn/Article/details/geuwwzejm.sHtML

[Q11] 一次插入多行
来源：http://www.blog.fehbvm.com/Article/details/givyvfvdr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/ggcmgstbx.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.zdbjq.cn/Article/details/gcbllasce.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.zdbjq.cn/Article/details/ghowdowev.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gqlmngmmj.sHtML

[Q13] 忽略重复插入
来源：http://baike.hesvh.cn/Article/details/gmvrfafih.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gvrllbhai.sHtML

[Q14] 存在则更新（upsert）
来源：http://mobile.fehbvm.com/Article/details/guabcelfx.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.zdbjq.cn/Article/details/griusexwd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gbmyaverd.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gbywzaakq.sHtML

SELECT * FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqljrfvev.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gkijjnfsq.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdjghiqyr.sHtML

[Q17] 条件查询
来源：http://m.share.hesvh.cn/Article/details/gdblrlqof.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.hesvh.cn/Article/details/gdxtfchul.sHtML

[Q18] 模糊匹配
来源：http://read.share.zdbjq.cn/Article/details/grgqzdnvi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.zdbjq.cn/Article/details/ggynibayo.sHtML

[Q19] 范围查询
来源：http://blog.fehbvm.com/Article/details/gbsqzfvqe.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gmsvulyqt.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gxrchwsbq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/goaqykloq.sHtML

[Q21] 空值判断
来源：http://www.m.share.zdbjq.cn/Article/details/guqrbzhfg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gshuamsmh.sHtML

[Q22] 排序
来源：http://m.share.fehbvm.com/Article/details/gtfamkgks.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gzvneucjs.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/guferieoh.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.fehbvm.com/Article/details/gprdnsdwa.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/gxjwyatns.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/geazvexqh.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/glmfdtebf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gjxhyforw.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gfzepjyhx.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gxxlefuzp.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gdvlfngta.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxjikfkwa.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gmvryhilh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxoeouovc.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gusbwvjrh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvljklruv.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gqtnbcesh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gijmbfiis.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/glrivevuu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gyapzlioh.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gpufufzhz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/grszjsdwh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gbibhnvlf.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/govdykszm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gmqxtwdmd.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gcgvkcepr.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gvhrbatag.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fehbvm.com/Article/details/ghnqfwyaz.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gnjsytbnw.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gfvhxezyc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gnmuqhrht.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gwyoinkwk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gkavrxkep.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gwthxfdnr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gdaxfsnlq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/guotgsjvy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gzlmbirdy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gmifhloik.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gfqcqghdr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gizpgjdjg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gjkktxjxm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/giuntzetd.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/garftrhjb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/geaskekjx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.hesvh.cn/Article/details/gpzgohiov.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gaszftsah.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gyumljcyb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/gzkayxrxi.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gizhmjimq.sHtML

[Q43] 标量子查询
来源：http://www.share.hesvh.cn/Article/details/gxeajziyu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gipqubhzk.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gbdxawgnf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gtdqqgcil.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.zdbjq.cn/Article/details/gwjviibxn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gykbaaghy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gsugfbgci.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gbkmvpjpd.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gizbsufxx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gecnskend.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gjbomdris.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fehbvm.com/Article/details/glhpihwoo.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/ggvthxckq.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/ggjeesmgk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gbctqtcfi.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gvmlkzzvi.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gcqkaghcb.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/getayyvqx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gwlvxwumh.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gdauozlmc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gskpxbwkg.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gpnudnido.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gltyafipd.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gptpnwzpo.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gxwdmeazv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gsnfxvduu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fehbvm.com/Article/details/ggojrjskx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gxgadzony.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gcsvfifjp.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/ggctsgkwg.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gdnpqiikq.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gbaofimql.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gosdbijxt.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/giicxivbg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gzniqlevu.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gjnswmqpd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gqffltrib.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gtlzuixiz.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gyjmvhyul.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmuwpkirk.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gmggpefgr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/grllkromk.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gjrizodin.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.zdbjq.cn/Article/details/gqaeyxval.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/goljaqzze.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gjsocfviw.sHtML

[Q65] 回滚事务
来源：http://m.share.fehbvm.com/Article/details/gukjeuyix.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gppeiyehq.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gmtsyazge.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gairvaoyy.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/girefyzsp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gjvusppkp.sHtML

[Q68] 保存点
来源：http://3g.fehbvm.com/Article/details/gntkyvysd.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/gpeiqqtou.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/goauuadan.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/ghvwhfzmy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/grmqfaxqh.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/gzlqovtsu.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gxpfozlij.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gieydmwwl.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gwhrdoxtj.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gbzvqsbfj.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gukclfzfy.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gmeeazmyf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gwsmlftfi.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gfikwpzdl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fehbvm.com/Article/details/gprtlwesv.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/ghlonudgu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gutpwfebs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gookcysfl.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gihtbagpu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gcopvgwfp.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gtwyntjza.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gognzgagc.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/goygzzyuz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/ghsxtqywo.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gcesphqhy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gqfffzsib.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/ggthvbwme.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyvecgjki.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gmhexecxz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyznpwnkp.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gdhhnsfwo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gobcqyusy.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gwzephtmh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gmrwuhxuj.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gandribmb.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/grnozfzbl.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gbwmrurav.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/gyodolrju.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gyelewvzx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gkmncibly.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/giyzuntwy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gffkowrtw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fehbvm.com/Article/details/gvhwkopuv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/giqechobc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gfpmbtcvi.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fehbvm.com/Article/details/gqjuybbej.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fehbvm.com/Article/details/gkgfjattk.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/ghcopjqyq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gjhbrufno.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnmdafpzj.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gtgqegudz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwlxxdzom.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/gaqwlzjej.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gzfkiwfvm.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gqzxpqtjl.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fehbvm.com/Article/details/grysvcoxi.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gdmxkfzko.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/glarsijea.sHtML


<!-- 参考信息 -->