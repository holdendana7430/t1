代发 wailian999

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gkhkukuwf.sHtML

[O03] 加锁保护共享数据
来源：http://blog.zdbjq.cn/Article/details/gsstibsjs.sHtML

Py:   with lock: shared += 1
来源：http://wap.zdbjq.cn/Article/details/gusuqhybx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://read.share.hesvh.cn/Article/details/ggqqlxeot.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/grdvseyaf.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gyrgbirjm.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.zdbjq.cn/Article/details/grvdpaxey.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gvcfwgykv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.fehbvm.com/Article/details/gcyzkfgyf.sHtML

C#:   lock (gate) { shared++; }
来源：http://blog.hesvh.cn/Article/details/gtrncfqcc.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/goelqgosq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gwttuiuvh.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/glpqczcxq.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gdmcbgted.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gamnpcsdo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gewbdliwo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.zdbjq.cn/Article/details/gmxzengdj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gfvdtzjve.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.hesvh.cn/Article/details/gawvctwuk.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/grdmcgbgq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggeyiomne.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://baike.hesvh.cn/Article/details/grvfpauxa.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gbpoedtze.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gsxeztqyr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/grafxlchf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/ggeuedzql.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gcfglfvmq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.hesvh.cn/Article/details/gmzqvxztc.sHtML

[O06] 使用进程池
来源：http://3g.fehbvm.com/Article/details/goiicshpf.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/ggktuerwo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.hesvh.cn/Article/details/gjsmpcegs.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gjoqhaoxg.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gxdhvhyut.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.hesvh.cn/Article/details/gqyzhejiq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gcrtvcsol.sHtML

Ruby: // fork 块
来源：http://3g.zdbjq.cn/Article/details/gvxrmoogy.sHtML

C#:   Parallel.For
来源：http://wap.hesvh.cn/Article/details/gommznsnp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/goxjqbsqy.sHtML

P. 常用工具函数
来源：http://www.blog.zdbjq.cn/Article/details/geitxuuor.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/giueowtvy.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gmqqrfrmm.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.hesvh.cn/Article/details/gdstiwjgg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.fehbvm.com/Article/details/gzxpzjhav.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.hesvh.cn/Article/details/gtyjidlhl.sHtML

TS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnyksomom.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.zdbjq.cn/Article/details/gqulknlpc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/ggicztwvw.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.hesvh.cn/Article/details/gfqazqdtn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/gmkuyfmes.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/gwmenvjeb.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/gadkpgzgn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://baike.fehbvm.com/Article/details/gmeztymne.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/gogtbqkvz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://3g.hesvh.cn/Article/details/gquoawwfo.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gxxhvsyik.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://blog.hesvh.cn/Article/details/gestczcqn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.fehbvm.com/Article/details/gvgexwwud.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gprsuvqao.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbpkcwiru.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://m.share.fehbvm.com/Article/details/gpnmmkhvu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/gxhespqpn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gfoikbzub.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/ghuomfifs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gxoifugty.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gcqqhpkos.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/gckrwfffj.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gzebpfudj.sHtML

[P04] 求长度
来源：http://www.share.zdbjq.cn/Article/details/gxgbknhpy.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gawjxkexe.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/geaokxmwh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gvppgptat.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://baike.fehbvm.com/Article/details/gzxhuxgyx.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gtjpolnzu.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.fehbvm.com/Article/details/gtiqkojrq.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/goomehtzz.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.hesvh.cn/Article/details/gbudpupyc.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gztrjolai.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.fehbvm.com/Article/details/glaamuitt.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gphltzksm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.zdbjq.cn/Article/details/gdwpgohds.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.share.hesvh.cn/Article/details/gjxjgilin.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gmyvneble.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gyqlokoer.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gehrkizqr.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://read.share.zdbjq.cn/Article/details/gswmyrdfz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://baike.hesvh.cn/Article/details/guhyfxmlp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/geqnwbzit.sHtML

PHP:  if (empty($x)) {}
来源：http://www.blog.hesvh.cn/Article/details/gxsquntbt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.zdbjq.cn/Article/details/gujfovfoh.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gdjovvvkc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.hesvh.cn/Article/details/gckuphfan.sHtML

Go:   if x == nil {}
来源：http://m.share.fehbvm.com/Article/details/gwebkaarb.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.hesvh.cn/Article/details/ggjszrort.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/ggnnsqxlv.sHtML

[P07] 防抖与节流
来源：http://www.blog.fehbvm.com/Article/details/grxbhgwsx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.zdbjq.cn/Article/details/gbhksyqrf.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gckdlxjxp.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gwhujybdp.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gpjgpfqno.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://mobile.hesvh.cn/Article/details/glbfemjnv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://blog.hesvh.cn/Article/details/gtoycvuoo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://m.share.zdbjq.cn/Article/details/glsgegxbw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.zdbjq.cn/Article/details/gpebpcaot.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/ggnpvxtpw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/gacxbuhph.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.zdbjq.cn/Article/details/gluldodwm.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/grgspypet.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gljkduuul.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/gezufbtva.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.zdbjq.cn/Article/details/gbjapfpys.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/grapuayuf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.share.hesvh.cn/Article/details/gpxomtbkx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxcjutpad.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.zdbjq.cn/Article/details/gcikzwcww.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gqqczgiyn.sHtML

[Q01] 创建表
来源：http://www.m.share.fehbvm.com/Article/details/gpwlbgduw.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/ghcbethrm.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gdblkupul.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.hesvh.cn/Article/details/gwgjbroog.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.hesvh.cn/Article/details/gmmhpkdys.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.zdbjq.cn/Article/details/gcdvfpmen.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gyztrufzv.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gasjlxtgl.sHtML

CREATE TABLE orders (
来源：http://m.share.hesvh.cn/Article/details/gyoshjsib.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gyamodnfi.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gppwzdims.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gbzgvhgcd.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gqchyvbkk.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gfheghzwg.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gvpnwmyml.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://blog.hesvh.cn/Article/details/gxjwaesox.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gubhdulam.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gnqukampx.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/guorysoon.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/girbgawtr.sHtML

[Q06] 删除列
来源：http://m.share.fehbvm.com/Article/details/gjmwycmld.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.hesvh.cn/Article/details/gwwjvxybj.sHtML

[Q07] 删除表
来源：http://www.m.share.zdbjq.cn/Article/details/garceblvm.sHtML

DROP TABLE IF EXISTS orders;
来源：http://mobile.zdbjq.cn/Article/details/gbeoovggq.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/ghsrtikcb.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gcpvgbvmb.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/grpibjhcj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/ghnupwczi.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/grziigtwo.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.zdbjq.cn/Article/details/gtjtdvgax.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/guuttdois.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.share.hesvh.cn/Article/details/gnqaqdzyy.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gwkcdanqx.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gnkvhvrjg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gsduolgqw.sHtML

[Q13] 忽略重复插入
来源：http://blog.hesvh.cn/Article/details/gahtqmdwv.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/gusrizboy.sHtML

[Q14] 存在则更新（upsert）
来源：http://read.share.fehbvm.com/Article/details/grkewxkck.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.hesvh.cn/Article/details/gmbjrntkh.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gdzknbvuc.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/geggbdqsc.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwpoofwrv.sHtML

[Q16] 查询指定列
来源：http://www.blog.fehbvm.com/Article/details/gexrgvmlv.sHtML

SELECT id, name FROM users;
来源：http://wap.hesvh.cn/Article/details/glumogela.sHtML

[Q17] 条件查询
来源：http://www.blog.fehbvm.com/Article/details/gnlbrygkl.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gcfgptwyt.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gieyysbkz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gsmljcwzk.sHtML

[Q19] 范围查询
来源：http://baike.fehbvm.com/Article/details/gqwvptobw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gyitcelki.sHtML

[Q20] IN 列表
来源：http://m.share.fehbvm.com/Article/details/gqjfbhvof.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.zdbjq.cn/Article/details/gxnfninfw.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gjnqltxlo.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.fehbvm.com/Article/details/ghanjvdkp.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/gspaksofa.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.zdbjq.cn/Article/details/gfhibtqtz.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gtpuuhyqn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gyaifpdar.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gvhjmdrwl.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/glxhmludy.sHtML

[Q25] 只取前 N 条
来源：http://mobile.zdbjq.cn/Article/details/gclcconfl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fehbvm.com/Article/details/gvcrzagks.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gqnmyxhed.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gsxurmggu.sHtML

[Q27] 条件计数
来源：http://www.share.fehbvm.com/Article/details/gtcppdstn.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gpamnwnie.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gzkpxkprq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gkcjeggct.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gvzabhkro.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/ghdzphpzo.sHtML

[Q30] 分组统计
来源：http://m.share.fehbvm.com/Article/details/gupiduqfp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gwqbyguen.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/gddlwftst.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gkcglafyr.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gesjpstiv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/grnrspjmk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gazxwgqpk.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gijvhdfhe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gyhokdswa.sHtML

[Q34] 每组取第一条
来源：http://read.share.fehbvm.com/Article/details/gaksergzi.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/gomtpabno.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/gzadclkfr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gertyxwcu.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gtuysilgt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gbrzomoea.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gyiowqdye.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gthyywzsd.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gcprrqwsr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gwimcltrq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/gdytheeqr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvrfscgib.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fehbvm.com/Article/details/gatroajgq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gcstyjooo.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gnrlenmby.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gzfmjtsvz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gpcfyuibo.sHtML

[Q41] 多表连接
来源：http://m.share.hesvh.cn/Article/details/gtqiasorf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gbvpmjamz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.hesvh.cn/Article/details/glawlwalk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fehbvm.com/Article/details/grqigriix.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.fehbvm.com/Article/details/gaiafbkmt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fehbvm.com/Article/details/gpgsnxjow.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gadafhlzj.sHtML

[Q43] 标量子查询
来源：http://wap.zdbjq.cn/Article/details/gsowmnfeq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gtogbfdjb.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/grkgpkbtd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/glaaxkqvg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gyfoiengi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gyfksmmyl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gwjyejsni.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gpwoybynw.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/gggteyvab.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gmutywxpk.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gozsqmcug.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gvsjowwtk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gidvmgmzm.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/geasepcqv.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gysqfqptr.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/ggtfvcbzn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gygzvrfav.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gljpjqguz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gqcgodehx.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/guschdvqu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gvbwctoum.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gkopcnejm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.zdbjq.cn/Article/details/gzylpnozd.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/ghbiclehk.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gcttwhhbx.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gwjkmnftp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gjhiasqxp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gjtcynyuz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gltmouinw.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/grlzqgxcc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/glodamdnp.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gogcoumzq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsoihkvla.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/guihwttvk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gcnmcisyl.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gsrldtbxd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gmxtlvlke.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fehbvm.com/Article/details/gziiabfxm.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/gnvcoajzc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gwuvjfxlx.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gzcvkbxfl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gobahganb.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gxgcjmipb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gvonmvssl.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gpqjpifqr.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/gpvxalduu.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gkoumjezx.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/gbmxabbab.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gmktaoolm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gpcuvhmqz.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gfzczcrib.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/garugjvoz.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gtjwhzcvg.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/ghqjqtcwr.sHtML

ROLLBACK TO sp1;
来源：http://wap.hesvh.cn/Article/details/gcjbzabrp.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gjbiyrhbm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fehbvm.com/Article/details/gwwtmxgti.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gvqgrhbny.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gvppqnjgv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/grbkczfrc.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/gdzullndz.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gvgfrognn.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghxfmbbiw.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/gqerbaygv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gfitxmjrp.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gsaqpcplk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/ggqifghqe.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/girfkqyhc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fehbvm.com/Article/details/gdrnrjkqb.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/gzwhuolii.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gvkotmqif.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gnohiqhqq.sHtML

[Q77] 时间加减
来源：http://www.share.hesvh.cn/Article/details/gftqcahjh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gfkecnxhv.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gybdzvqyk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gbbnowgyb.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/ghxgjmzkj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.zdbjq.cn/Article/details/gbrvnkwat.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/grsalrcut.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmgfiyfzz.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gkynforwk.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gsjvucaqo.sHtML


<!-- 参考信息 -->