代发 wailian999

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/ghybgvevr.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/gnapnqzyx.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gvrymybmy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/grqikbnac.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/grfxhenzm.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gbqmwdzmx.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gdgqfvsns.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.zdbjq.cn/Article/details/guebltxos.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.hesvh.cn/Article/details/gfclvgrwe.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gkmzguroa.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gltxphevd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gkqjjgwsa.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/gbheesrqc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gkphaqvqr.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gyglvkwoc.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/goqmqcods.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.fehbvm.com/Article/details/gjkfzmycb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.zdbjq.cn/Article/details/grqtqislc.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.zdbjq.cn/Article/details/gvlafzquu.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/ghjbsxgfp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/ghidhfpir.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://3g.zdbjq.cn/Article/details/gsvjqqcpw.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gjuibsmys.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gxhbntowa.sHtML

[O06] 使用进程池
来源：http://baike.hesvh.cn/Article/details/ggiftfhwk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://blog.zdbjq.cn/Article/details/guzshoiac.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/galjvselk.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gpfpbbisf.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gfumnssbs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.hesvh.cn/Article/details/gptqzzhxu.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gnuqdbpdt.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gjoyotind.sHtML

C#:   Parallel.For
来源：http://www.m.share.fehbvm.com/Article/details/gwrsobiwq.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gotdlivcc.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gtrhsmsoh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggdxtdrup.sHtML

[P01] 生成 UUID
来源：http://3g.fehbvm.com/Article/details/guwxjsjaz.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gwoatvohg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/goguqcafy.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.hesvh.cn/Article/details/gmsowfwhl.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gjpbdkvtm.sHtML

Java: UUID.randomUUID().toString()
来源：http://mobile.fehbvm.com/Article/details/gnvarpckm.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.zdbjq.cn/Article/details/gvyylbntm.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.zdbjq.cn/Article/details/ggbcbvpru.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/gunoyzafp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gocmrtlbq.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gdduqsebq.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://wap.zdbjq.cn/Article/details/gtaefpfdo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/gzhbnusfe.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.zdbjq.cn/Article/details/grltqvjnw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/gfcjqyuyz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/gzlvctjwq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://3g.hesvh.cn/Article/details/gzehtjcgf.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.share.zdbjq.cn/Article/details/guvymjilf.sHtML

[P03] 生成短随机字符串
来源：http://wap.zdbjq.cn/Article/details/gksymmwbv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/gdjliqcyc.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.fehbvm.com/Article/details/gyeevgztp.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/gcqxzzcbu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gwipvrcvd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.fehbvm.com/Article/details/gymftwvaq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gnwsbcbfn.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://blog.hesvh.cn/Article/details/gwvfvevex.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.fehbvm.com/Article/details/gyqfpqqgo.sHtML

[P04] 求长度
来源：http://blog.zdbjq.cn/Article/details/gejgxgdtg.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.fehbvm.com/Article/details/gbxbistre.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/ghwvrbirx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gydgcrdgy.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gimaibtks.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gzbpnvtfb.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gwyfuqphv.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gmppvngvt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gyjozmpzj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.zdbjq.cn/Article/details/guvlirsrp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.zdbjq.cn/Article/details/gyefiuxyf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.fehbvm.com/Article/details/ggfzuczqb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gtdromjsv.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gaajxruoy.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/glpuzkhan.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gjqnjjyev.sHtML

Ruby: a == b
来源：http://baike.hesvh.cn/Article/details/gphjodkil.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/goosmfqda.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/ggrfmbprz.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/gmgjtsvje.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gmlpzrgtq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://mobile.hesvh.cn/Article/details/gdcttsulm.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/glcsrobjo.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/grwdbfpom.sHtML

Go:   if x == nil {}
来源：http://www.blog.fehbvm.com/Article/details/gkjyufvea.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/grkdnfzop.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gqoyvmalp.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gdcysravd.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/ghwdwdquy.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gkgkfotvo.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gzvsrbykm.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/ghatxcbax.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/gakshswrs.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gxgwsqymj.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.zdbjq.cn/Article/details/glyxztvmz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/gqmbtvhrr.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/gcsnslfdc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.fehbvm.com/Article/details/ggxsrffum.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.fehbvm.com/Article/details/gnhcaentj.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/gqshzhogc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gecjpbpyw.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.blog.fehbvm.com/Article/details/gepizyxjq.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/gwuwebnqe.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gchmkhcwi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gphnfqpsy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzhlnbikl.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.zdbjq.cn/Article/details/grraqqlrb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzrmkgtgu.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/gqqznmgfl.sHtML

CREATE TABLE users (
来源：http://mobile.zdbjq.cn/Article/details/gnwosloep.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gxdwuyujj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gcszhbgkd.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gbzagwkwp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.zdbjq.cn/Article/details/gqeaqjhak.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gaqrgivoe.sHtML

[Q02] 创建带外键的表
来源：http://www.share.zdbjq.cn/Article/details/gixoyrdxv.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gylgzyceh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://blog.zdbjq.cn/Article/details/gnqhjbzhg.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.fehbvm.com/Article/details/gvedrdfch.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.hesvh.cn/Article/details/gnowsajzj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.hesvh.cn/Article/details/gcyajzpvn.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gmszcrpvz.sHtML

[Q03] 增加列
来源：http://3g.zdbjq.cn/Article/details/geutiygmr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/geqpbyczs.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/gdqoashsr.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.zdbjq.cn/Article/details/grfgrfuhw.sHtML

[Q05] 重命名列
来源：http://www.blog.hesvh.cn/Article/details/gmgcbxfff.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.m.share.hesvh.cn/Article/details/gxcfdahcr.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/grcewzytt.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gmmjmibra.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gpgypbctn.sHtML

DROP TABLE IF EXISTS orders;
来源：http://wap.hesvh.cn/Article/details/gpbaeoljj.sHtML

[Q08] 创建普通索引
来源：http://m.share.fehbvm.com/Article/details/gwdlrqidp.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gewzpbkqo.sHtML

[Q09] 创建唯一索引
来源：http://3g.hesvh.cn/Article/details/gfrtgpokn.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gilofmbxr.sHtML

[Q10] 插入单行
来源：http://baike.hesvh.cn/Article/details/gcrybiqis.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/ghtneswcg.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/gytyjjess.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gzocwfetb.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.zdbjq.cn/Article/details/ghxuxxoom.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.share.fehbvm.com/Article/details/gjjmpsbnq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.hesvh.cn/Article/details/gnhngcpxz.sHtML

[Q13] 忽略重复插入
来源：http://baike.zdbjq.cn/Article/details/gtreacive.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gwqqlivws.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/gayiqoauo.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.hesvh.cn/Article/details/gffzyvvru.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gxqrbavhi.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/gxkdgmfyh.sHtML

SELECT * FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gqskrgndr.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gcozfkhxe.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqylmroas.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gagehzyxv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzosdkupn.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gniaaqyvp.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/ghatemyfa.sHtML

[Q19] 范围查询
来源：http://mobile.zdbjq.cn/Article/details/gqtrcmixc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.fehbvm.com/Article/details/gtbkgjbsk.sHtML

[Q20] IN 列表
来源：http://baike.zdbjq.cn/Article/details/gzynitxfh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.hesvh.cn/Article/details/ghoerwout.sHtML

[Q21] 空值判断
来源：http://wap.hesvh.cn/Article/details/ggvslyhgk.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/glnseoblm.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/giymtvihb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gzuvlklxa.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/gxjkrcvqu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.fehbvm.com/Article/details/gnsqerffb.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gqfslhwxe.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gnsowjidm.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gxpgjdxhq.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/gkdomkrum.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/gycpirfyk.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gptsqpwso.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gftdcxaly.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/geiinfqpa.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gteflxwsx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmemgasxu.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gpeujpcdb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grwesjfkz.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/ggbwjkzud.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gdguxzwue.sHtML

[Q31] 分组后过滤
来源：http://m.share.hesvh.cn/Article/details/grlenxbcd.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gxvfkiore.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gwrydboxt.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gtefrfdfo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/gdlmkjryt.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/ghtffarca.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gmmwveoap.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gwewykivw.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/guwlezwcg.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/ghybdfaaa.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gfllghfgg.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gohzcttpu.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gexbqvcxp.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gnofwuijy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gvdplvopl.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gnmmtngcr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gjdyysgrc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gnbdptmnm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/guxscuhjx.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gqsouogmc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gjfnowxwl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gdmrrbzub.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gcwqohqdz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gbcloseqr.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gqnitukmk.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gtboxjith.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gixrqwdnt.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fehbvm.com/Article/details/grutdjsob.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fehbvm.com/Article/details/gkbgvjpsl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gmlmsbgcs.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/goqbhccan.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/glwaskeoq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gdgjkblcn.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/ggpvfyyqt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gjicyvthq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gevbitlrm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gxybcxwhn.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gumtupxln.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gjbnylong.sHtML

[Q47] 与平均值比较
来源：http://read.share.zdbjq.cn/Article/details/gtpkfsuvf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gjnonflxx.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/ggbwcvenw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gdaeswnkj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gskdgfnfc.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gglzqaajt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gdzlsrmsa.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/glxkelakn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gowcpebho.sHtML

[Q51] 用子查询更新
来源：http://3g.zdbjq.cn/Article/details/glbzkuejt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gwxhzsnju.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/glxmbgsnc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gpsuzgmcn.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/geylzbgil.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fehbvm.com/Article/details/gndtphndy.sHtML

[Q54] 清空表
来源：http://baike.hesvh.cn/Article/details/gublbhecj.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gnggqtjcu.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gbyvdxczv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gjkzelbex.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gemuhhoad.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gtruqjvcn.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/geesftqhp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gourqalzi.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/gzzusklap.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gkksubiii.sHtML

[Q59] 分组内累计
来源：http://www.m.share.zdbjq.cn/Article/details/gnrajvdpl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gglhcuccd.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/ghxmyqqwh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gghvaomoz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gcutckddx.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gsacpdhdl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gljrbhhug.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gzartmcuv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gehmlignn.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gljxndvxu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gcmtumtny.sHtML

[Q64] 提交事务
来源：http://m.share.fehbvm.com/Article/details/gbsmhcguv.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gwvinwysy.sHtML

[Q65] 回滚事务
来源：http://m.share.hesvh.cn/Article/details/gimfzpiya.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gzbhjsizf.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/ghlsmhmpg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gowfzbzlk.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/guvfzekkp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fehbvm.com/Article/details/gmbpfarwb.sHtML

[Q68] 保存点
来源：http://wap.fehbvm.com/Article/details/gvnciybnz.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/grkxdvizx.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/gzxmvtcdy.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gbdmtltpy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gpesvafnz.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/ghlrgnwbn.sHtML

ANALYZE TABLE users;
来源：http://wap.zdbjq.cn/Article/details/gvxcjxqwc.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gcxccoudr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gbfucpqok.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/ghvuyhspk.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmqnawhja.sHtML

[Q73] 查看表状态
来源：http://read.share.zdbjq.cn/Article/details/giknjyyyf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gkpezaboi.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/grsygqmsp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gsxyonbdw.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/goqkqkkzh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gzqjvwiti.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gzqwuxlrc.sHtML

[Q76] 按天统计
来源：http://blog.fehbvm.com/Article/details/ggsxbvrea.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gdlyadams.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/grhtcgxry.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gsmfiiddi.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/ggaguxfew.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gwdnpdnwp.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gasfqhtfb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gldbloygt.sHtML

[Q80] 字符串截取
来源：http://3g.fehbvm.com/Article/details/gbzecfhmq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.hesvh.cn/Article/details/goanyemhs.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gqhbjylrb.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gvjklnnah.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gcnvovyfq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/geupnepbf.sHtML

[Q83] 大小写转换
来源：http://wap.hesvh.cn/Article/details/glubijcto.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gqhotsgxp.sHtML


<!-- 参考信息 -->