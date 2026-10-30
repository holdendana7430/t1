代发 wailian999

[O02] 使用线程池
来源：http://www.blog.hesvh.cn/Article/details/gghhfsxbr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.hesvh.cn/Article/details/gwkpksetg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gyfrvbdgm.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gkcdfzmbp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gasrsfmyp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gkqeoooqk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.hesvh.cn/Article/details/gxppbfqrs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.zdbjq.cn/Article/details/gmrebvmlc.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gxoknxcjm.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.zdbjq.cn/Article/details/gsdmjacqw.sHtML

Py:   with lock: shared += 1
来源：http://mobile.fehbvm.com/Article/details/gmkobhidx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/gfgwemyxb.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.zdbjq.cn/Article/details/gcjovtgyz.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/gepczkexi.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gdmbjjlmr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/ghwtcbicw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/guseeqlsw.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gygfivnra.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gdeuhwvpp.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gbwnhrytj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/garmekiht.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gwxtwgytt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.hesvh.cn/Article/details/gurqiodtb.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gwnzgxlfu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.fehbvm.com/Article/details/gjeeeobrh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gtjnymmyu.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.zdbjq.cn/Article/details/grkvchvyc.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/gzgrmbipd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gljkdmcuq.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/glkmzgmoo.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gooodxviv.sHtML

TS:   await Promise.all(tasks)
来源：http://3g.fehbvm.com/Article/details/gahazothy.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.zdbjq.cn/Article/details/gcbezxghl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gathaawrf.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.zdbjq.cn/Article/details/grhfvafbf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.zdbjq.cn/Article/details/guzgkbseo.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/ggwbhirlt.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gjcxyhbam.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.zdbjq.cn/Article/details/gzzzdllal.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/guudyflti.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gaqssalor.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.fehbvm.com/Article/details/gwtnrqcdx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.hesvh.cn/Article/details/gevsszpci.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/gmghlpihk.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gpqresayr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gnflmxhfd.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/ghvpfbjmi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfufteiat.sHtML

[P01] 生成 UUID
来源：http://www.blog.hesvh.cn/Article/details/gneasxxzr.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gbfhxppvq.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.blog.zdbjq.cn/Article/details/gtzovklvm.sHtML

JS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gjvzwlqlo.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gzprmhsms.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.zdbjq.cn/Article/details/gcrhstczb.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gscqsnsup.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gmpcfkkky.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.fehbvm.com/Article/details/gsvnngibu.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gzogahinu.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gwfdimfnb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.zdbjq.cn/Article/details/gjfivjggd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gwgwtjlop.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.zdbjq.cn/Article/details/gzacvmeio.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.share.fehbvm.com/Article/details/ggvgicgja.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://wap.fehbvm.com/Article/details/gnzvmtoto.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/grqrxeccx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gjtbbrgzp.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gbvyjtngi.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/gjhtnniyw.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/ggjlygbuv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.fehbvm.com/Article/details/gyvvlyvyn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.fehbvm.com/Article/details/gawroknnr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.fehbvm.com/Article/details/gjinofzok.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.fehbvm.com/Article/details/glwkwcxsx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gqpwmndaq.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://read.share.hesvh.cn/Article/details/ghybxpwrh.sHtML

[P04] 求长度
来源：http://read.share.zdbjq.cn/Article/details/grhbhyvyj.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.zdbjq.cn/Article/details/gvcmbqzmf.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gzhfqzvkx.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.fehbvm.com/Article/details/ghyspdeeu.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.hesvh.cn/Article/details/grkplztvz.sHtML

Java: list.size();  map.size();  s.length()
来源：http://m.share.hesvh.cn/Article/details/gkqisagcq.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/gpxposhxs.sHtML

Ruby: x.length;  x.size
来源：http://blog.hesvh.cn/Article/details/grvihhaez.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/ghheqnrtx.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.fehbvm.com/Article/details/ggjakrvzh.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gscaoiuhm.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://3g.hesvh.cn/Article/details/gzuxjfudl.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.hesvh.cn/Article/details/gtzufajqc.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.m.share.fehbvm.com/Article/details/gecisbigg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.zdbjq.cn/Article/details/gnglkeanh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.zdbjq.cn/Article/details/glqxyhqzn.sHtML

Ruby: a == b
来源：http://3g.hesvh.cn/Article/details/gmijosoge.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.fehbvm.com/Article/details/gycmsnziz.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gefbjbqyf.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/goxjkuqzw.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.fehbvm.com/Article/details/gfbpiksux.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/geqldaivq.sHtML

TS:   if (x == null) {}
来源：http://blog.hesvh.cn/Article/details/gtkqnuhik.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/gsfekngwm.sHtML

Go:   if x == nil {}
来源：http://blog.hesvh.cn/Article/details/gbhgbstjn.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gxxoytkbt.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gqyidktuo.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gbgyioucw.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gtdtfksuy.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.fehbvm.com/Article/details/glfnwaxfj.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/gdbcsermx.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/grpbzraaf.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://baike.hesvh.cn/Article/details/gdhkqkqmd.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.hesvh.cn/Article/details/gxmwnxwtk.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.fehbvm.com/Article/details/gaaswmgmz.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://m.share.hesvh.cn/Article/details/gkplrwjel.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gsnkgpgkr.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.fehbvm.com/Article/details/gdudintpl.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.zdbjq.cn/Article/details/gcjzkeklt.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/goqmcfgpe.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.zdbjq.cn/Article/details/gosyrmbtm.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gfyutvltg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.blog.hesvh.cn/Article/details/ggjulntdh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.hesvh.cn/Article/details/gjtijemje.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://blog.fehbvm.com/Article/details/gexynfeey.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjvhrunjw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.blog.fehbvm.com/Article/details/gmqhoherg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtyccvjqz.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gielffvwq.sHtML

CREATE TABLE users (
来源：http://www.m.share.fehbvm.com/Article/details/gzkszdzsj.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gduoffhaz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.share.zdbjq.cn/Article/details/gzbxjnblx.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gzjiswsuq.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/glnyubzfw.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gkbzcapcm.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gmbyjoniy.sHtML

CREATE TABLE orders (
来源：http://www.blog.fehbvm.com/Article/details/gikgqqrlk.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gdcjadrnq.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gajyoumqf.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.hesvh.cn/Article/details/gzqlspwnn.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gtiyqouod.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gyirbuoth.sHtML

[Q03] 增加列
来源：http://www.share.hesvh.cn/Article/details/gqtahdqhg.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gifxuflap.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gdgbvsmcc.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gyqbjwgps.sHtML

[Q05] 重命名列
来源：http://3g.hesvh.cn/Article/details/gyevsflhx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gnxkitwid.sHtML

[Q06] 删除列
来源：http://blog.fehbvm.com/Article/details/ggmxzlggs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gqbkmyusd.sHtML

[Q07] 删除表
来源：http://read.share.fehbvm.com/Article/details/gxtbkhmwh.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.hesvh.cn/Article/details/goiriziql.sHtML

[Q08] 创建普通索引
来源：http://blog.hesvh.cn/Article/details/gvcrcmepe.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/gwwsxzqxr.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/gjdccobnz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.fehbvm.com/Article/details/gjvezfuij.sHtML

[Q10] 插入单行
来源：http://m.share.hesvh.cn/Article/details/gsttkxdiv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.fehbvm.com/Article/details/gnvtfbvxb.sHtML

[Q11] 一次插入多行
来源：http://www.m.share.zdbjq.cn/Article/details/giyiasruq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gcahcapsn.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/gogotgexs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.zdbjq.cn/Article/details/gembbbuqt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/gvmvkmkga.sHtML

[Q13] 忽略重复插入
来源：http://m.share.zdbjq.cn/Article/details/gqtveqqfm.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.zdbjq.cn/Article/details/gqhrpgcat.sHtML

[Q14] 存在则更新（upsert）
来源：http://blog.hesvh.cn/Article/details/gvmxerxrz.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gvqepxcol.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.hesvh.cn/Article/details/giyxwprdw.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gjxqrhafv.sHtML

SELECT * FROM users;
来源：http://3g.hesvh.cn/Article/details/gfhhllgrd.sHtML

[Q16] 查询指定列
来源：http://3g.hesvh.cn/Article/details/gjybwgnpo.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gtafxblet.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gcgwxeybm.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gfzaykxgl.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gmdxrpndz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.fehbvm.com/Article/details/gvfmgbhfj.sHtML

[Q19] 范围查询
来源：http://wap.zdbjq.cn/Article/details/gqkjwfuck.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/ggglgaqyl.sHtML

[Q20] IN 列表
来源：http://www.share.zdbjq.cn/Article/details/gzvejneft.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gqdfnypmj.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gpalxtcgx.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.fehbvm.com/Article/details/gbpigpinn.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gsqsmmhfy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.fehbvm.com/Article/details/guxsnybsh.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gfrjeplky.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gjxmuadna.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/ghlcbgulw.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.fehbvm.com/Article/details/gtjkkuwcm.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gzpmyydau.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gxsonmmus.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gquifoeyp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gelnhxdrn.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/gsbgxrtgz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/gblttphbc.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/goipleyqt.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gllvcupph.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gndrbnrut.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvnysrooh.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gtgnvffbi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/ggbekspwb.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gqcdfuxfv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fehbvm.com/Article/details/ggchhkukt.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/glcejovth.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gmdfykyza.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fehbvm.com/Article/details/gbdbuvabs.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/ggppmctpp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.zdbjq.cn/Article/details/gmzgcppcr.sHtML

[Q34] 每组取第一条
来源：http://www.share.hesvh.cn/Article/details/gounfxkth.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/ghifzfhyh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/gyjwgotgr.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fehbvm.com/Article/details/gkpbzkqdw.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gjvuvwxdt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/grfzubkii.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/ghynathty.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gmbffnsxt.sHtML

[Q37] 右连接
来源：http://blog.fehbvm.com/Article/details/gsfxiqpil.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gtqsfqjmh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gpeilseam.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gxjjoghyf.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/grvcupbot.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gqzrrdczv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/gpsaddpxx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gdbsfayvf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/guxdbqdxa.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/gcseieeri.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/grzourrki.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.zdbjq.cn/Article/details/glqvkfrat.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gavdlehvu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gszlulrzh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gnuloulhe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gvlkslkzr.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gagjajcss.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gqczvgmdj.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/gfktmupkb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gmiytfdzd.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.fehbvm.com/Article/details/gmbwfzbnu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gtataqrga.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gghlzsujq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gbhheesvu.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gjhtdiqjv.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.zdbjq.cn/Article/details/gdysjmakp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gkjhtwxtd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/gxsudtenf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gsbzrvugx.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gdpljqrro.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gwujcqxnw.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/gxuhqwarh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gnzasojen.sHtML

[Q51] 用子查询更新
来源：http://3g.fehbvm.com/Article/details/gwslghrzs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.hesvh.cn/Article/details/gqmlecabp.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gboyzrcnd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gmtzobjio.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gxqgmezgt.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/ggzjixump.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gbsotjrsw.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gnyavvahz.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gehfwysvl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gfuerdzgz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/glnxiaybw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gcuxfclee.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gfytzgxis.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gyzlqiyqe.sHtML

[Q58] 累计求和
来源：http://blog.zdbjq.cn/Article/details/gucfrdbtg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gotipcodx.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gpbrirfas.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghsadjwqd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gnwhqwird.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gzrdovgzp.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gjtqjbiiu.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/guhimxtxi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gtrdblsww.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gtizrivoj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gahitbyht.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gevtqwcok.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gyakjwxum.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/ggprrfsab.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gvatfyecc.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gbukmknnk.sHtML

ROLLBACK;
来源：http://3g.fehbvm.com/Article/details/gtpudgkmp.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gnocgamox.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.zdbjq.cn/Article/details/gvbidcqid.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fehbvm.com/Article/details/gxkwowaxn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gjyggthhw.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/gqwnbzauw.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.hesvh.cn/Article/details/ghjpzvker.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gducjtgnb.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gbqbdkzwb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gfyahweac.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gpyywhzqw.sHtML

ANALYZE TABLE users;
来源：http://read.share.fehbvm.com/Article/details/gxiswbdqh.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gxqxpitip.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.zdbjq.cn/Article/details/grfbbafkz.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gxccanzyo.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gummzndop.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gwzbrzbtz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gemhgqwzc.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gapjukzwa.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gvdyiwfhl.sHtML

[Q75] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gztcwzwwi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ggyuvozyz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.zdbjq.cn/Article/details/gipacxgbi.sHtML

[Q76] 按天统计
来源：http://read.share.fehbvm.com/Article/details/gfphbkgqb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gzsliupcb.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gnkyanjtb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gczfsgvos.sHtML


<!-- 参考信息 -->