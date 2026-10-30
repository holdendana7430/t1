代发 wailian999

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gicjowpsz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gfptsopbj.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.zdbjq.cn/Article/details/gcwvswbgz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gkkivxepj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggzilpynz.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gnsptzvfb.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gjssjrlxz.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gcogenntd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/guzbmkpqw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gzprvghzi.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gaoltuhls.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gbrepphec.sHtML

[O06] 使用进程池
来源：http://mobile.zdbjq.cn/Article/details/glwlrnqmo.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gshvescng.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gmgcxrlbm.sHtML

JS:   // child_process / cluster 模块
来源：http://3g.zdbjq.cn/Article/details/guakhldqd.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gvyvpnmao.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gsasbvpkb.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gxsctlzlv.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/gldqihhnw.sHtML

C#:   Parallel.For
来源：http://www.blog.zdbjq.cn/Article/details/gmfhourrx.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggbensbbv.sHtML

P. 常用工具函数
来源：http://blog.hesvh.cn/Article/details/gvqfdgukw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwvwswepz.sHtML

[P01] 生成 UUID
来源：http://www.share.fehbvm.com/Article/details/ghkdpxhwj.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.fehbvm.com/Article/details/ghpdetxff.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://wap.hesvh.cn/Article/details/gegglcoxl.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.zdbjq.cn/Article/details/gyylerlcm.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.fehbvm.com/Article/details/gzsofsvxm.sHtML

Java: UUID.randomUUID().toString()
来源：http://wap.fehbvm.com/Article/details/gzuecqyjc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.hesvh.cn/Article/details/geahgbmmd.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gfempewwq.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.zdbjq.cn/Article/details/gneoafspg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.fehbvm.com/Article/details/gqenwnmox.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.hesvh.cn/Article/details/gbirjjeje.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://mobile.hesvh.cn/Article/details/gqnltiwuj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.zdbjq.cn/Article/details/gjtusombl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gomlxysio.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gxfuvmnnm.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.fehbvm.com/Article/details/gykjckxuy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.fehbvm.com/Article/details/gnoiofqts.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gdskrghfs.sHtML

[P03] 生成短随机字符串
来源：http://read.share.zdbjq.cn/Article/details/gefouxgbl.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gbprjdyax.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/gvxyplsze.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.fehbvm.com/Article/details/gexnnmvjv.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gmcncvjdm.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.hesvh.cn/Article/details/gmrcwjuxy.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/grrwsuqpy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.hesvh.cn/Article/details/gudmfcpqu.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gjcvtetyq.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gmxwaosng.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/gbwdyxugc.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/guvecunbg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/ghgnmnjmq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gskqfajte.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gqlpesrtf.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gicnvjxog.sHtML

Ruby: x.length;  x.size
来源：http://read.share.zdbjq.cn/Article/details/gvuuhueik.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.hesvh.cn/Article/details/grizzsupt.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.hesvh.cn/Article/details/gjohxugpb.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/goblfivsp.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/gxsunbggr.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gafdfwzkc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://m.share.fehbvm.com/Article/details/gqaltmngt.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gfkivsgeb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gfkvnkxef.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gubnmrdrm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.hesvh.cn/Article/details/gadicjggn.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.hesvh.cn/Article/details/gzxzayjcv.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/ghkkuotjb.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gihqkhtiv.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/glohoefnc.sHtML

TS:   if (x == null) {}
来源：http://www.blog.fehbvm.com/Article/details/gosdvatba.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gwsxhqhqj.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/ggzzqnwtu.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gxlhjjmcf.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gvykvsdjd.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/gtplqunqk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.m.share.fehbvm.com/Article/details/gqifsqfqz.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.hesvh.cn/Article/details/gdskwpszo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.fehbvm.com/Article/details/gcsddrtao.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.hesvh.cn/Article/details/gsovubtuz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gpnwahtdd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gongveghb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.fehbvm.com/Article/details/gqpbvcwfc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gnxexdbaj.sHtML

[P08] 处理浮点精度问题
来源：http://wap.fehbvm.com/Article/details/gxvrulvwa.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.zdbjq.cn/Article/details/gfgyiegqa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.hesvh.cn/Article/details/gafpaskgn.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gedvxpcnn.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gxqctqkvb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.fehbvm.com/Article/details/gqtkaibsl.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.zdbjq.cn/Article/details/gyjyxpblv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/govzkbrut.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.zdbjq.cn/Article/details/glwreqoiv.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmvcvqkbn.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/grduevmiz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkgrnqjrj.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gwwzyuuhu.sHtML

CREATE TABLE users (
来源：http://baike.zdbjq.cn/Article/details/grrfepjmj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.zdbjq.cn/Article/details/gmkqkwymj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gfezuvvwd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://wap.zdbjq.cn/Article/details/gxgrdwbfx.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.blog.zdbjq.cn/Article/details/grkmqqpgf.sHtML

);
来源：http://3g.fehbvm.com/Article/details/gfkseneol.sHtML

[Q02] 创建带外键的表
来源：http://m.share.hesvh.cn/Article/details/gkszdwlcq.sHtML

CREATE TABLE orders (
来源：http://www.share.hesvh.cn/Article/details/gkfujdluh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/grviapset.sHtML

user_id INT NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gwsoxvonp.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gnohpiwbj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://wap.hesvh.cn/Article/details/gououwvlj.sHtML

);
来源：http://www.share.zdbjq.cn/Article/details/gcnjjdtmd.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gzdguwgyd.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/ggpwelkod.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/gadzisrii.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.fehbvm.com/Article/details/gcyppujcm.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gthldxwfw.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.zdbjq.cn/Article/details/gubryeeuc.sHtML

[Q06] 删除列
来源：http://mobile.fehbvm.com/Article/details/gzademupl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gqudsmtgt.sHtML

[Q07] 删除表
来源：http://m.share.zdbjq.cn/Article/details/giukzzyxk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/grfdbdcje.sHtML

[Q08] 创建普通索引
来源：http://baike.hesvh.cn/Article/details/gkuobsewc.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://m.share.hesvh.cn/Article/details/gdlykyolt.sHtML

[Q09] 创建唯一索引
来源：http://wap.hesvh.cn/Article/details/gwtmvbnxt.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://mobile.fehbvm.com/Article/details/ghhcgblcp.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gfvbvujfk.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gawsehjji.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gxqahpdzi.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.fehbvm.com/Article/details/glovpbmhn.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gxdskxfrl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/gyofctgkm.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.fehbvm.com/Article/details/gscabcewb.sHtML

[Q13] 忽略重复插入
来源：http://www.share.zdbjq.cn/Article/details/ghguiarzg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gnyqbjled.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gelgteyyh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.zdbjq.cn/Article/details/gjflozhka.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.zdbjq.cn/Article/details/gnqcddacd.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gotpsywvq.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gjztriuqw.sHtML

[Q16] 查询指定列
来源：http://m.share.hesvh.cn/Article/details/grwmyzila.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghnvqhcrc.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gbqmnbeth.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvxbpkvzj.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.hesvh.cn/Article/details/gasekbacj.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.zdbjq.cn/Article/details/gduujdozw.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gzjgfmwkj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fehbvm.com/Article/details/gqigthwka.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/gxrvcnbrn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.fehbvm.com/Article/details/gidwfjypr.sHtML

[Q21] 空值判断
来源：http://wap.fehbvm.com/Article/details/gudcdnldw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.zdbjq.cn/Article/details/gmmvcmvob.sHtML

[Q22] 排序
来源：http://mobile.hesvh.cn/Article/details/gspiakdhp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gswiuubmc.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gmaqenozl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gnzecevlr.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gbwdvyngy.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.zdbjq.cn/Article/details/gfekxditt.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gcdvvgdei.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gvbyyygrm.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gmfexnaqh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gfkvqksti.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gqungritn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvpeqhdcc.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/giufxuqej.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gypjsngah.sHtML

[Q29] 最大最小值
来源：http://read.share.fehbvm.com/Article/details/gfpylpbir.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/gaxogazzw.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gdpjslocz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fehbvm.com/Article/details/gmmiojekl.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gcipttdsv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gsikjrhjh.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gexwgiast.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/giktolnpp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gygocybtq.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/glixuapou.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gujqhpuhz.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gzuojhias.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gnuvkfgyp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/ghoahrfgq.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/gkqkcfaat.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gwiftfwib.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gracxewhk.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/guydzdbbj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gztqjcrrw.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/gxdhqilqf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.zdbjq.cn/Article/details/gwhtjwdwz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gqmyouklw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gmvmcptgc.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gabmdoxrg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gavudoobq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gdyfkrgal.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/geksgcfsa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/guwbbaxpg.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/grafnkwpk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gdewkdksg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fehbvm.com/Article/details/gnajwbqhk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/gaspnisgk.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gdsrfundm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/ghiipvbjh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.zdbjq.cn/Article/details/gdsziebmo.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/gujyhhxwi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gonxnaovx.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gofuubizi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.hesvh.cn/Article/details/gggxpoxua.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gpmdswqrd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gqbdzihgc.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gvxuebktk.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gqwyngiao.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gxkvjxqvo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gheewynfp.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fehbvm.com/Article/details/gyhsvfihl.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gfznayckv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gpsfusbaj.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gkqqejzzi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/glsdkwsqm.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/grafuhsta.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gckxcwtvy.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/giwuvjkdd.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gqvoyrabh.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gxzzcwyti.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ganfnewvm.sHtML

[Q53] 按条件删除
来源：http://3g.hesvh.cn/Article/details/gzjufpmnd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/guvajxuas.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/ggsvalptf.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gqgluozlx.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fehbvm.com/Article/details/gxvkgsphl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/glgopzcjc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gagtorgdr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.hesvh.cn/Article/details/grnxgnwmm.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/ggvifiwbj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gfmkdthfv.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gwandlprf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkclaytot.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gizkcvhhl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gsjceejvb.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gbikgapgf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/gyqhrxddb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gaczaxkkc.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gnurojigh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkiisjfpe.sHtML

[Q62] 分组占比
来源：http://www.share.hesvh.cn/Article/details/gjhdhkdbn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/guebbqzmk.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gwyjyuhpu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fehbvm.com/Article/details/gfpteawzt.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/geytdvxkm.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gnmpoimok.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gdcmfhoel.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gmumhpsls.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/grtkohdoy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.hesvh.cn/Article/details/gaoqtrwcl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gequuxjve.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gphuhvauk.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gootldsnc.sHtML

SAVEPOINT sp1;
来源：http://wap.hesvh.cn/Article/details/guqqbbgpj.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gnftdfcyj.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/glpnsvrga.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.hesvh.cn/Article/details/gowsthdfr.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gtcrsndqu.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gzocvervi.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gmxlqssan.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gahrxwgdn.sHtML

[Q72] 查看索引
来源：http://blog.fehbvm.com/Article/details/gbszfakba.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnxqnkcfz.sHtML

[Q73] 查看表状态
来源：http://m.share.zdbjq.cn/Article/details/gjixttasb.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.hesvh.cn/Article/details/gceswomvt.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gamjcmfnj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.zdbjq.cn/Article/details/gmjgnulcx.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gwkevwblq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpseybubc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gelkdwogl.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gvbtdqdmw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gyxqstvje.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/guzayyixy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.zdbjq.cn/Article/details/gtezszaco.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gpgjvrapv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gwlihynhi.sHtML

[Q79] 字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/guucieric.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fehbvm.com/Article/details/gfgqpwvzz.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gkqghlqyd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggifoidyj.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/guyujodiq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtxojthim.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gnicddlbu.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtcqjicma.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gnaawwani.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzbnjnqci.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gyzkstqpt.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/goeocsuvd.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/guiugqqtg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gxzmrpcnc.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/gfwcwbirx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/ghvxxrqkh.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/gierccaxc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gpwpoeijw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gbnmhcbrl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/gyztzqfew.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbozzhzjo.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gtmvebpts.sHtML


<!-- 参考信息 -->