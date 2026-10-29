代发 wailian999

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gzlgbrfaw.sHtML

Go:   go f()
来源：http://blog.zdbjq.cn/Article/details/gvdryztqy.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gijkkomib.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/grxwtjjvt.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gevpkrxkl.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gjspnlmrt.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gdbfdsuck.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.zdbjq.cn/Article/details/gyjarwfcn.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gwkqxtwlj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gcxeelznw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gikkvmflr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.zdbjq.cn/Article/details/gcbuwniev.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.zdbjq.cn/Article/details/gibvnfubh.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.hesvh.cn/Article/details/gjqovdhyn.sHtML

Py:   with lock: shared += 1
来源：http://3g.zdbjq.cn/Article/details/gdmzcllwo.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gcotdjajv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.hesvh.cn/Article/details/gkxvprgan.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gtkxjjhwi.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.fehbvm.com/Article/details/gxurtwfgb.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/glhlzyhqj.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gynurieig.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ghptjxvcv.sHtML

[O04] 定义异步函数并等待
来源：http://3g.fehbvm.com/Article/details/gpvmkstrd.sHtML

Py:   async def f():⏎    await g()
来源：http://baike.fehbvm.com/Article/details/gggttrlco.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.fehbvm.com/Article/details/gsglmulaz.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gtpkhvcty.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gkhtpwlks.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gdbfydeoe.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.m.share.hesvh.cn/Article/details/gtyzebgui.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gtlkpwpjs.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/gfwqqbclx.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/geuwmgohm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gfwjrztlj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gphycaplk.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gkxzvcblm.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.hesvh.cn/Article/details/ghfyhnhle.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gklwonkmj.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.blog.hesvh.cn/Article/details/glofkxgvu.sHtML

Ruby: threads.map(&:join)
来源：http://blog.zdbjq.cn/Article/details/glvqlhqbq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.fehbvm.com/Article/details/giafrnqns.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gaxxbkthe.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gtfvnaboq.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://read.share.hesvh.cn/Article/details/gxvznosrf.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/ghufvplzr.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gpuqfgqzx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gxmrsvqwd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/gszlyxflc.sHtML

Ruby: // fork 块
来源：http://mobile.fehbvm.com/Article/details/ggdriocmp.sHtML

C#:   Parallel.For
来源：http://baike.zdbjq.cn/Article/details/gcwpvevur.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gkcimzyud.sHtML

P. 常用工具函数
来源：http://www.share.zdbjq.cn/Article/details/gryjkajyl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpxzgarkf.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/gtglgydws.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gbrgolwwp.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/giwziguge.sHtML

JS:   crypto.randomUUID()
来源：http://blog.zdbjq.cn/Article/details/gzwlwasar.sHtML

TS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gbbvcxhox.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.zdbjq.cn/Article/details/gqprrpksi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.zdbjq.cn/Article/details/gcftshxho.sHtML

Ruby: SecureRandom.uuid
来源：http://read.share.hesvh.cn/Article/details/gmvatuyzu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/grcvbvqwd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gyomkfrna.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrvfqmd.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gebtfycxy.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://3g.hesvh.cn/Article/details/gdfubhlws.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.fehbvm.com/Article/details/gtcjheygm.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://m.share.fehbvm.com/Article/details/gyswoxsht.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://3g.zdbjq.cn/Article/details/gnudyxfph.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/gexlcnpno.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.hesvh.cn/Article/details/gjkbfpufy.sHtML

[P03] 生成短随机字符串
来源：http://baike.hesvh.cn/Article/details/gvretxxmv.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.fehbvm.com/Article/details/gcgrubnnz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.zdbjq.cn/Article/details/gdownomgo.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gkqsloifw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gbxqccgrw.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/ggreoegqd.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.zdbjq.cn/Article/details/gmovnjgcs.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.fehbvm.com/Article/details/gbmfairea.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/golipjfds.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gohbizanf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.share.zdbjq.cn/Article/details/glaoktfzg.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fehbvm.com/Article/details/gdnczxwqn.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gmcctxbmk.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gmyjvbhmf.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gegxludls.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.fehbvm.com/Article/details/gjvqpuxxy.sHtML

Ruby: x.length;  x.size
来源：http://wap.zdbjq.cn/Article/details/goofdrztt.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://wap.fehbvm.com/Article/details/gmrbnljcd.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.zdbjq.cn/Article/details/gyiknjvqi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://blog.hesvh.cn/Article/details/girsipsmo.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.fehbvm.com/Article/details/gfsikznvp.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.hesvh.cn/Article/details/gevujcfet.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gczzzhayv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://read.share.hesvh.cn/Article/details/gkjakinmq.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gputkpkvd.sHtML

Ruby: a == b
来源：http://read.share.zdbjq.cn/Article/details/gbhhjczbh.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.fehbvm.com/Article/details/gwawmkaoc.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gdxwatdbx.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://3g.hesvh.cn/Article/details/gwbisocqt.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.zdbjq.cn/Article/details/gjudlkhic.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.zdbjq.cn/Article/details/gqshsedix.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gbyvgpfbd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghrqcvcnn.sHtML

Go:   if x == nil {}
来源：http://baike.fehbvm.com/Article/details/goxidoeuv.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.zdbjq.cn/Article/details/glqevprbo.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gpqbknhof.sHtML

[P07] 防抖与节流
来源：http://mobile.fehbvm.com/Article/details/grvyurzok.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gaiybetcb.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gauiwyzhs.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.zdbjq.cn/Article/details/gupkmodno.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.zdbjq.cn/Article/details/gadjpjaim.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.zdbjq.cn/Article/details/gsrkojeon.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/geujbfpon.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gglyuzcji.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.m.share.fehbvm.com/Article/details/gmuawwape.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gtiwuvdkl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gonsazjrh.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gxvdpvhcp.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gijerrkhj.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.hesvh.cn/Article/details/gubjmfkjh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.hesvh.cn/Article/details/gdggdhudc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://m.share.fehbvm.com/Article/details/gpcsqsmyc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.hesvh.cn/Article/details/gdukujewr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/gvlaywonn.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guqwnijue.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.zdbjq.cn/Article/details/gagnnopjz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaeqihtyd.sHtML

[Q01] 创建表
来源：http://www.share.zdbjq.cn/Article/details/gkvqbxacl.sHtML

CREATE TABLE users (
来源：http://3g.hesvh.cn/Article/details/gjdwgenjh.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gghxjddpj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gylkcgynt.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.zdbjq.cn/Article/details/gmcbqnnrc.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gditemkwj.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/ganovoswd.sHtML

[Q02] 创建带外键的表
来源：http://blog.zdbjq.cn/Article/details/gsifvphas.sHtML

CREATE TABLE orders (
来源：http://3g.zdbjq.cn/Article/details/gjdbjusrb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxiluoacw.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gixkvxffa.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gqcfqlpwr.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.fehbvm.com/Article/details/gkdunkyuj.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gfnyebvmx.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/gumouuxhk.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.hesvh.cn/Article/details/gvztvvrme.sHtML

[Q04] 修改列类型
来源：http://www.m.share.zdbjq.cn/Article/details/gykqzfznp.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/geftowcyb.sHtML

[Q05] 重命名列
来源：http://blog.fehbvm.com/Article/details/gnckiqgif.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gliswxmkg.sHtML

[Q06] 删除列
来源：http://www.m.share.fehbvm.com/Article/details/grvldlffx.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/ghpnuuxbq.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/gorocrmcq.sHtML

DROP TABLE IF EXISTS orders;
来源：http://blog.zdbjq.cn/Article/details/ghtrikonw.sHtML

[Q08] 创建普通索引
来源：http://mobile.hesvh.cn/Article/details/gvrziymkh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gklhpfaks.sHtML

[Q09] 创建唯一索引
来源：http://m.share.hesvh.cn/Article/details/ggketbpzj.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/glwaoykhx.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gprazpwix.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gmpunvhje.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/ghgvqezdb.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://blog.hesvh.cn/Article/details/gkickxunw.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.fehbvm.com/Article/details/gdnxwddei.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://3g.fehbvm.com/Article/details/gqsoptxhb.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/glmqkxyzq.sHtML

[Q13] 忽略重复插入
来源：http://www.blog.hesvh.cn/Article/details/gpbojmdxc.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/glgemwlgc.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.fehbvm.com/Article/details/ggsbqqioe.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gjcbvbyzq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/guoouhfde.sHtML

[Q15] 查询全部
来源：http://3g.hesvh.cn/Article/details/gdewplmpk.sHtML

SELECT * FROM users;
来源：http://baike.hesvh.cn/Article/details/gwbebjjkg.sHtML

[Q16] 查询指定列
来源：http://3g.zdbjq.cn/Article/details/gzxrevdil.sHtML

SELECT id, name FROM users;
来源：http://blog.zdbjq.cn/Article/details/gftpvqzga.sHtML

[Q17] 条件查询
来源：http://wap.hesvh.cn/Article/details/gzpvmxmsi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gvgaekmpp.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gjxthspui.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/glmrlfpvq.sHtML

[Q19] 范围查询
来源：http://mobile.fehbvm.com/Article/details/gcdxhhkib.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gtjivqrgj.sHtML

[Q20] IN 列表
来源：http://wap.fehbvm.com/Article/details/gkbmgpwgp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/giinlavgv.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gmcefmpay.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gbratwcqg.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gdujkwjhp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/gojugjhdg.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/garaeushu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gwhporqym.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gnpmzrymi.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggknvdjad.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gwktwivey.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gczmdvqhv.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/gyvrhgskh.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gekxntjyh.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/gkfxixhti.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gnvuhvqmg.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/grzjqiliu.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gtyekewkp.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gywpapkym.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gzurroeer.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gzxvtheyh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gcgnfsulu.sHtML

[Q31] 分组后过滤
来源：http://wap.zdbjq.cn/Article/details/grbuaflcx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/guywzpzha.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gbkthypwc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/goyzrxbqt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fehbvm.com/Article/details/gspcpkifu.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gyewbonem.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/gbodeoixn.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gzyczyjly.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gqbfnxcdv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gqcpcfrnw.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gmkncgtqv.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gxtubkxrt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmcceehfm.sHtML

[Q36] 左连接
来源：http://3g.hesvh.cn/Article/details/gvfogbmrr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/ghnplslch.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/grkyrwget.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/grxjxcmbv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fehbvm.com/Article/details/gktsyxwgk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gcwxjkpas.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gueqpdeya.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gohobweba.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/gvkfkoiuv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gvybzfyes.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/glmabhvrp.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gcntedsdg.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gekjcevoz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gndynmusg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gzrpbjizz.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gtcdvfayj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/gvinyaypf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gcppnqapt.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gaszzitzy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gflwvqsue.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gedlpzefr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.zdbjq.cn/Article/details/gjtumsdtc.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gvxrbvupa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/gjzmhwjza.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gnmijktaq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/grcfbmwri.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gyebwnqio.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gejiugdwj.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/grpdgzgzc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gdaiectlk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gckdsenzh.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/grkqfseps.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gjmoqnzge.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/gmwqnufkw.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gsqzszppg.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gdwvffngr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gbscogaua.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gvjntvsuq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/gycnbyzsp.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/grntaijsq.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gvejmjzvw.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/giqioymst.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gjgnpxdzt.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/guzqvirpo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gokiurbsu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/gowqmoplk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gadhyrqfk.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gackkmrwx.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gezyyobjl.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gzuovrgdo.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/grudsaudu.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gurxenarj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gorpwwguk.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gdwzxhzmu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.zdbjq.cn/Article/details/gczijmvmk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gewhtjpzb.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/grdbkrzeb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/grqwivoft.sHtML

[Q62] 分组占比
来源：http://wap.zdbjq.cn/Article/details/ghfixpffi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gkdemltwr.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gpmhfevxe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gaxufggfq.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gooxlbxuv.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gyrlrjpil.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/guwceceey.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gojulvsss.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gqdhuptge.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gpqyysynx.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gwmslkpyo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gsqnudqge.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/ggnxebcao.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/gajzdudmi.sHtML

ROLLBACK TO sp1;
来源：http://3g.fehbvm.com/Article/details/gbedsqhle.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gvhkxawlt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/geqantxln.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gfyudsyrj.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gcvdasxzc.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gpfvyomue.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/ggwkqvjfw.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gjboojbze.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjbuptbek.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gbwvvzyrq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/gwaagzyjb.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gghjdjsio.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gojvffotg.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gtmetqbnb.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/ghvjtutop.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gpxoqckdt.sHtML


<!-- 参考信息 -->