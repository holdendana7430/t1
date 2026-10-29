代发 wailian999

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/guebpudvy.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gvurchmkc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gbkzsfmsy.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.zdbjq.cn/Article/details/gmqmaeteg.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gqjyryoys.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.zdbjq.cn/Article/details/gwculrawr.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gvuxrtqhr.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/glanrxtxu.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gidzcvdsq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/grqkwrvfw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gtkuhzacx.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gjzqioxpx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gzcbtlhpx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.hesvh.cn/Article/details/gshdsdeae.sHtML

Ruby: threads.map(&:join)
来源：http://3g.hesvh.cn/Article/details/ghzkrgytp.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.hesvh.cn/Article/details/gjrxnmubd.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gxegqtkof.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gejxnnkrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.hesvh.cn/Article/details/gxiityolz.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/giwfqxjgn.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gsfsjpjkw.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gcfwckdan.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gncjgogdj.sHtML

Ruby: // fork 块
来源：http://read.share.hesvh.cn/Article/details/gvmxqqwhd.sHtML

C#:   Parallel.For
来源：http://www.share.zdbjq.cn/Article/details/gfafgvjxv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/geekmsnkr.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/gczjbnjjd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gcjodyrmt.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gpkkzhtya.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gzypnkecu.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/guqscxovb.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.zdbjq.cn/Article/details/gxkykvfpl.sHtML

TS:   crypto.randomUUID()
来源：http://3g.zdbjq.cn/Article/details/gbjblvcgr.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gwkzedidr.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gheglbgco.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.zdbjq.cn/Article/details/gnoqbvwzw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gugbesrou.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.zdbjq.cn/Article/details/grpigcoba.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gwvewikdp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://3g.zdbjq.cn/Article/details/gathvqrwb.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.zdbjq.cn/Article/details/glnphphzq.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gwzlvzgrw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gczwkajfp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.hesvh.cn/Article/details/gtkbyjktf.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gzgmwvhza.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gfslrcxlk.sHtML

[P03] 生成短随机字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxjomwggc.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.fehbvm.com/Article/details/ggvkrcdot.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://3g.fehbvm.com/Article/details/gfujjnejl.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gmvardqiq.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gmzgqmjpn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gfduqtjui.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.hesvh.cn/Article/details/gbnxdahti.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.zdbjq.cn/Article/details/gyybtstme.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.zdbjq.cn/Article/details/gwqopypxq.sHtML

[P04] 求长度
来源：http://baike.hesvh.cn/Article/details/ggdlyjfrk.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.fehbvm.com/Article/details/gazfqyplo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/giuzjgvaa.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/glynseweq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gusschmqw.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.zdbjq.cn/Article/details/geirhblsv.sHtML

Go:   len(arr);  len(m)
来源：http://blog.hesvh.cn/Article/details/gaihjknbo.sHtML

Ruby: x.length;  x.size
来源：http://www.m.share.zdbjq.cn/Article/details/genpgwuur.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.fehbvm.com/Article/details/gfjiijdks.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gugvhaeac.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://read.share.zdbjq.cn/Article/details/gcxljdxgr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gnfacxnuz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gjzfgznoh.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.zdbjq.cn/Article/details/ggwktdotm.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.zdbjq.cn/Article/details/gowaajeed.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gbagaadjs.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/gdmdwxsvm.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.fehbvm.com/Article/details/ghhglqkvj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/goyjibjdn.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gqznxkypx.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gqlgchnve.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.hesvh.cn/Article/details/gwymjujhm.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/giiveguci.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.fehbvm.com/Article/details/gnbytcozo.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/grdoksouk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.fehbvm.com/Article/details/gfpydhvzz.sHtML

C#:   if (x is null) {}
来源：http://www.blog.fehbvm.com/Article/details/gwsjuoqpf.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/ggetzsukj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.hesvh.cn/Article/details/gswmmaslx.sHtML

PHP:  // 手写时间戳比较
来源：http://blog.fehbvm.com/Article/details/gqcdjukme.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gamxuoras.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/godgbisra.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.zdbjq.cn/Article/details/gexjauoyj.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.zdbjq.cn/Article/details/gdhpmkvab.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.hesvh.cn/Article/details/gwdejbvkz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.zdbjq.cn/Article/details/gipvvnibw.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gffkyliwn.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.zdbjq.cn/Article/details/gvmtmsoce.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gffrgwabj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.zdbjq.cn/Article/details/gblmybywo.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/genpgrbvi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gnszmials.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/ggaawrprd.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.hesvh.cn/Article/details/gtwlszpax.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://mobile.hesvh.cn/Article/details/gayyjbfpn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjplzxilq.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.fehbvm.com/Article/details/gpxubfsvh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzlwbuvzl.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gkkhjygbx.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gatblmghf.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.hesvh.cn/Article/details/gszeoosnm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.fehbvm.com/Article/details/gflavxryz.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.hesvh.cn/Article/details/gitxwqzfp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/ggnpfbixo.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gythmzram.sHtML

[Q02] 创建带外键的表
来源：http://www.blog.hesvh.cn/Article/details/gwpojbzzy.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gsfzebyls.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/glvdknsjo.sHtML

user_id INT NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/gcjkdcoft.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/gnsnisirw.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gvfafaxgi.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/glsvkjdhu.sHtML

[Q03] 增加列
来源：http://blog.fehbvm.com/Article/details/gxwzpayuy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.zdbjq.cn/Article/details/ggbtsvous.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gwurrcgxk.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://read.share.zdbjq.cn/Article/details/gonavncbx.sHtML

[Q05] 重命名列
来源：http://read.share.hesvh.cn/Article/details/gvakigjsc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/gqxusghqu.sHtML

[Q06] 删除列
来源：http://3g.fehbvm.com/Article/details/govqmlipw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gxprkmiej.sHtML

[Q07] 删除表
来源：http://blog.fehbvm.com/Article/details/gztsoydja.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ghbqgedfv.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/ghtpairgn.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/gvwxituwz.sHtML

[Q09] 创建唯一索引
来源：http://baike.fehbvm.com/Article/details/ghuxnadrd.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.fehbvm.com/Article/details/gsofcgoun.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gaxlbvbcp.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gjqrylnyq.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/ggqhsnzjh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gfffcuzpf.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.zdbjq.cn/Article/details/gofdvtalo.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.zdbjq.cn/Article/details/glzphlffz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gfhmmhmfr.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.fehbvm.com/Article/details/gooebfqyy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.fehbvm.com/Article/details/gghlsnttt.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.hesvh.cn/Article/details/gvzychzsb.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://mobile.fehbvm.com/Article/details/gyejardek.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://baike.fehbvm.com/Article/details/gbejmrtuf.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/goyslsxyb.sHtML

SELECT * FROM users;
来源：http://read.share.hesvh.cn/Article/details/golaxacsj.sHtML

[Q16] 查询指定列
来源：http://wap.zdbjq.cn/Article/details/ghemmcoqh.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gmpmoatul.sHtML

[Q17] 条件查询
来源：http://www.m.share.fehbvm.com/Article/details/gxnbgoole.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://m.share.hesvh.cn/Article/details/gvmmxkzel.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gvnlrgrvx.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/giayxmpny.sHtML

[Q19] 范围查询
来源：http://www.share.hesvh.cn/Article/details/gqcedvhod.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gblgfmtmz.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/goahkefwc.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/ggjcuoqhp.sHtML

[Q21] 空值判断
来源：http://www.blog.hesvh.cn/Article/details/gnjknivgf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gzqnrqqkr.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/gotysmemf.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/gywomydpc.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gdicaiutp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gayaukohs.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gsrekedfw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gacaddafh.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/ghqizuvau.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gvywmvwzv.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gbpbdyrax.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gxnimarum.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/grlhjkyya.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ghuuwdczk.sHtML

[Q28] 求和与平均
来源：http://www.share.hesvh.cn/Article/details/gzeqweqju.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ggpyxadym.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gnexpzhol.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/ghvrftpqf.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/giunncphq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/goejumnej.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gnjpbzoqm.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gybnlzzmb.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gnmjqmcxx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/giktdpesh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gbtxmbqiy.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/ggcsfupeq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fehbvm.com/Article/details/gwjplwfzr.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gvxjjozqw.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gdbwjxgou.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gtcdmgvus.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gdxrkntjd.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gwneddmrf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/geavwsbku.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gonidmkbd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gwxqcyjjh.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gfyafbloo.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gcpziuzpo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/gektvowts.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/golngvudj.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gfucisfxv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gaaagvglt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gxiglnvka.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gkisijdnh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gwotujksf.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gzfdlpoxg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gwakuepsp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gtnbvodim.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gsnxgusoz.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gtckgcdsf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gpirnmrod.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gjuvcklfq.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gnqdqbkvh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/grcccojzq.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gyfempugi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gvkfyiulr.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gcxfzcqau.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gtspshtud.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gdmtzmzcy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gakomjhbp.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/guifuueas.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gssrzuevd.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gajvpjluf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gbhzcbqtg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fehbvm.com/Article/details/gmejqwtwe.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gvqlvjtih.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gqsjczalf.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gjfkdaenb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gcrsokugo.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fehbvm.com/Article/details/goewnghaa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gpsqnkfes.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gyubdcjuk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gniyjbrbp.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gbjvcccpw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gsjhpynsx.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gcgpexdji.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gqeshpjzf.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/grtynilzu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gslzcteae.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.hesvh.cn/Article/details/gsgwyclre.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gjfwzxgiv.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gekmyixgl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/goiucdwoy.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gsuvgzays.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gaewxeokd.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gwlqnbrkd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gzbelswvg.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gscrfjjpq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.hesvh.cn/Article/details/gqryjlysz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/giiscytlk.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gciemwurm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gmqufojfs.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gzyrtbfgb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ghopnvyoi.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gchgddcba.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gtthrinck.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gaqlzzqud.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/gqutszaar.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gsplhrbxd.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/genhdvrzy.sHtML

[Q66] 行锁查询
来源：http://www.blog.zdbjq.cn/Article/details/giwchvvzh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.zdbjq.cn/Article/details/gvboljvkf.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/gpasojqiz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/genscuamk.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/ghgzszzcl.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gmcobzkfa.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gskdjizzj.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/guxqvwarq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.zdbjq.cn/Article/details/gtetgomao.sHtML

[Q70] 更新统计信息
来源：http://3g.fehbvm.com/Article/details/gfqyukvrn.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/ghydmxboh.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/ghtbryipt.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gztmpdzzh.sHtML

[Q72] 查看索引
来源：http://www.m.share.fehbvm.com/Article/details/gvxmcqrek.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbmoydzjs.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/gqoxvaanx.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gwkaymmpu.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gqsetlcoz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/geurzizgw.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gdberdjhn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwnnytlar.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.hesvh.cn/Article/details/gezahlgwn.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gnqxrnbld.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gpgiogyfo.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gyjwswgqm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gwwaljzun.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gvlqkweck.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gjxhlsjfb.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gxenwezgv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gcvejalrz.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/grbzftcce.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsgnxdriw.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/ggvmmanhu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gtjkgkzrq.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gwtcetpfd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaiayecei.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gwmbaglfe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gddgetlai.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gndmbbapn.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gczbkimej.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gngcezczl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gaznpvznv.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gptnbhisi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gytqyrzzd.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gszukugvc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gpwtimzmo.sHtML


<!-- 参考信息 -->