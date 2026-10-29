代发 wailian999

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpzezacvo.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gxtivsiik.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gcklsfoha.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gxwrrnsvt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/goreqpljs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gkxnuxcff.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gdhezhlph.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gykkahjso.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gskqyfpvl.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gfsyemoos.sHtML

Ruby: Thread.new { f }
来源：http://wap.zdbjq.cn/Article/details/gpcicwxsp.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gymqtznsr.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gufgfmgxf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/guounjkvg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.zdbjq.cn/Article/details/gicqkpupr.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.zdbjq.cn/Article/details/gmfzpsvuq.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.hesvh.cn/Article/details/guhvdupwy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://m.share.zdbjq.cn/Article/details/ghpalhqmm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.fehbvm.com/Article/details/ghqwwehuo.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gfakoazpk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gnyowyyek.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.fehbvm.com/Article/details/gqbmdzgtn.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gwwkacsfb.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gblecljxi.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gmcfiwrgm.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/ggexzgeab.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzmevvgtq.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gncxvdmib.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/guehhhvcb.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gqrvwxwnq.sHtML

[O04] 定义异步函数并等待
来源：http://wap.fehbvm.com/Article/details/gtmderbju.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.fehbvm.com/Article/details/gtlcqixfs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.zdbjq.cn/Article/details/gomsrltrh.sHtML

JS:   async function f() { await g(); }
来源：http://baike.zdbjq.cn/Article/details/gjbkawfwg.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gmbunjytm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/ghrjbrqqq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gvaospssl.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.m.share.zdbjq.cn/Article/details/gyasmpagj.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gcjhbnjvs.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.zdbjq.cn/Article/details/gyfcheqeq.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.zdbjq.cn/Article/details/goevavtqj.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.zdbjq.cn/Article/details/gubbuswlc.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gixthbeam.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gjctcpmfa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.zdbjq.cn/Article/details/gnxexyarx.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/grrhigojx.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gmxedjxff.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gvpjpiwzv.sHtML

[O06] 使用进程池
来源：http://read.share.fehbvm.com/Article/details/gghanzgbk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gngukltjk.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gplrqrmjm.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/ggscxmxfp.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.hesvh.cn/Article/details/gkpcvwegu.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gzrrfpmbr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gctcwsoah.sHtML

Ruby: // fork 块
来源：http://www.m.share.fehbvm.com/Article/details/giuxzetwg.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gxzxnwpni.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/giovbsbrf.sHtML

P. 常用工具函数
来源：http://read.share.zdbjq.cn/Article/details/glblndevj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gizibirsx.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gauytlelo.sHtML

Py:   str(uuid.uuid4())
来源：http://3g.fehbvm.com/Article/details/gtdtxkjdx.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gkppxnyvb.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gnnwwsvlc.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gmsjkhfsa.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gfszaanyj.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gsgcyuxaq.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.zdbjq.cn/Article/details/gmpfpohtr.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.blog.hesvh.cn/Article/details/grpehggcg.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.zdbjq.cn/Article/details/gronxiijy.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://blog.zdbjq.cn/Article/details/gfxemmjbw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gmnwtkdrc.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.hesvh.cn/Article/details/gorgftbmf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/glypsztet.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gudijmykz.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.zdbjq.cn/Article/details/giydjqldv.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gaytmvver.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.zdbjq.cn/Article/details/gyyztbkep.sHtML

[P03] 生成短随机字符串
来源：http://www.share.zdbjq.cn/Article/details/ghbbxadsd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.hesvh.cn/Article/details/guhgokuva.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://mobile.zdbjq.cn/Article/details/gyxakjftx.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.hesvh.cn/Article/details/gfjmntlcu.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/gzgyvrtze.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.m.share.fehbvm.com/Article/details/gojykivsg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gbolizwpy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://mobile.hesvh.cn/Article/details/gkvxxidhf.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gtjkazvmv.sHtML

[P04] 求长度
来源：http://blog.fehbvm.com/Article/details/gstjoylcz.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gpbmbkney.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gerkchmeg.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gptklsljf.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.hesvh.cn/Article/details/grdwwmqqb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gznxisqac.sHtML

Go:   len(arr);  len(m)
来源：http://3g.hesvh.cn/Article/details/gvzsahclq.sHtML

Ruby: x.length;  x.size
来源：http://wap.fehbvm.com/Article/details/gqgtcldbv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/giaubitcy.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/ggmejpmmt.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.hesvh.cn/Article/details/gazriuwns.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.zdbjq.cn/Article/details/glhmracdj.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.zdbjq.cn/Article/details/giinnwsjy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://3g.hesvh.cn/Article/details/gzibgmgua.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gphcnroeo.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.hesvh.cn/Article/details/gefrjzpek.sHtML

Ruby: a == b
来源：http://wap.zdbjq.cn/Article/details/gltkqydxc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gfryyocmv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.blog.zdbjq.cn/Article/details/gzjnihowh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.fehbvm.com/Article/details/gelzhboxl.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gqgimutpe.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.hesvh.cn/Article/details/gowhyergt.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gvfmydwqn.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gznwgineo.sHtML

Go:   if x == nil {}
来源：http://m.share.hesvh.cn/Article/details/gfokdzdyc.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://mobile.hesvh.cn/Article/details/gjbpccaym.sHtML

C#:   if (x is null) {}
来源：http://wap.zdbjq.cn/Article/details/gkprhlowy.sHtML

[P07] 防抖与节流
来源：http://www.share.fehbvm.com/Article/details/gnnugplgi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.fehbvm.com/Article/details/gccshvwgf.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.hesvh.cn/Article/details/gygvwhayg.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gitbzporg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gxarohhvj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.fehbvm.com/Article/details/glpnoeehk.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gqtydrcwa.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gbutrvxgi.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.fehbvm.com/Article/details/gijnacgim.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.zdbjq.cn/Article/details/gxnnavstl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://read.share.hesvh.cn/Article/details/gygbaotip.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://3g.fehbvm.com/Article/details/gjokthlqe.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://m.share.zdbjq.cn/Article/details/ghflvaszh.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gvrahszbp.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.zdbjq.cn/Article/details/gswdotcty.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.fehbvm.com/Article/details/geuwzbwas.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.hesvh.cn/Article/details/gjqzrcagj.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.fehbvm.com/Article/details/gewwraklt.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/guhyzkwqw.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gygtrdfvx.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gpuckltzr.sHtML

[Q01] 创建表
来源：http://www.blog.hesvh.cn/Article/details/grpncswlv.sHtML

CREATE TABLE users (
来源：http://wap.fehbvm.com/Article/details/gdwgukosb.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gyytuakqe.sHtML

name VARCHAR(50) NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gwixqqifn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.blog.fehbvm.com/Article/details/gzwqnrnoe.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gexyhpxrn.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gcltqrbja.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/gluisnqcm.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gqyokwzyu.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.hesvh.cn/Article/details/gugpopqap.sHtML

user_id INT NOT NULL,
来源：http://wap.hesvh.cn/Article/details/gtrkuytjy.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gppzorqhp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://read.share.hesvh.cn/Article/details/gmvcnpflt.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gyxciordq.sHtML

[Q03] 增加列
来源：http://www.m.share.zdbjq.cn/Article/details/gjppchfog.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://3g.zdbjq.cn/Article/details/gorkkjoog.sHtML

[Q04] 修改列类型
来源：http://www.share.fehbvm.com/Article/details/gfxkxgcec.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.hesvh.cn/Article/details/gkifjpnqm.sHtML

[Q05] 重命名列
来源：http://read.share.fehbvm.com/Article/details/gfydrcqgg.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/goapwhcyu.sHtML

[Q06] 删除列
来源：http://wap.fehbvm.com/Article/details/gvpihrryd.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gzxpwarro.sHtML

[Q07] 删除表
来源：http://www.blog.fehbvm.com/Article/details/gyxhszzpf.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gwbypnqvp.sHtML

[Q08] 创建普通索引
来源：http://blog.zdbjq.cn/Article/details/gsohrlbjo.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.zdbjq.cn/Article/details/gtfgyfljw.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gfpluwrnw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.fehbvm.com/Article/details/ggoblxpro.sHtML

[Q10] 插入单行
来源：http://mobile.fehbvm.com/Article/details/gglredkrs.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gujggdqsv.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gzcnmyzjg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.hesvh.cn/Article/details/gjhxhmmmy.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gankeymkt.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://wap.hesvh.cn/Article/details/gckxgeyul.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.hesvh.cn/Article/details/gwmstyenu.sHtML

[Q13] 忽略重复插入
来源：http://3g.zdbjq.cn/Article/details/gmvtngmxe.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.hesvh.cn/Article/details/guvwwukzi.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gqcopcmnl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://3g.fehbvm.com/Article/details/gvbpwhnqb.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gftefvixv.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gtkyckcsq.sHtML

SELECT * FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gtrpnvubs.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gwxmuwqib.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gircoyqmm.sHtML

[Q17] 条件查询
来源：http://blog.fehbvm.com/Article/details/gofeqyduy.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/gbhwqtrpo.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/giceczeml.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gaospkmjh.sHtML

[Q19] 范围查询
来源：http://m.share.zdbjq.cn/Article/details/gvqgwdalc.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://mobile.fehbvm.com/Article/details/gmqqnadpo.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gknafjynm.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/girirqqsq.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/ghounzixg.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.zdbjq.cn/Article/details/gjjooumrv.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gprasoggk.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.hesvh.cn/Article/details/gurblkfnm.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gmlcdrior.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://mobile.hesvh.cn/Article/details/glturxwwx.sHtML

[Q24] 去重
来源：http://wap.hesvh.cn/Article/details/ghucusluh.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.hesvh.cn/Article/details/gynbzgfbl.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gkxtaqism.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gvhhezvxu.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gymcikccm.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gfbyhxfey.sHtML

[Q27] 条件计数
来源：http://www.m.share.zdbjq.cn/Article/details/ggnybafni.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gzrxiesbm.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/gxflzupll.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gbpdqudwq.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gvyxndwnd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmszujzcm.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gtshtivpi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gommajuhe.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/givutjouy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gzrsxthxa.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gadllzywa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gxopiyihr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.hesvh.cn/Article/details/gyeltlbah.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gfylsaorg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/grzpxcbhf.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gngsvpsxl.sHtML

SELECT * FROM (
来源：http://blog.fehbvm.com/Article/details/gtzpvfslq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gncujhxjq.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gqwzghcwo.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/goggnwxlx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gqryfhcvo.sHtML

[Q36] 左连接
来源：http://www.m.share.hesvh.cn/Article/details/gsfmmhyuy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gzlyzwhps.sHtML

[Q37] 右连接
来源：http://www.blog.zdbjq.cn/Article/details/guobmxghn.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gayigtkzv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gysiqeujd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gimlmdmaz.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gtuylmbsg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/ghxskojwa.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gzprareul.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gmpledswb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fehbvm.com/Article/details/gjroaphtw.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gvbqywkwt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/ghvjrmghw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gkecbnmjx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gmqlnkbge.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gbsywvmyp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gdkyvlcev.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gsfiuvqpy.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gahedysrr.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gbfmjndst.sHtML

[Q44] IN 子查询
来源：http://www.share.fehbvm.com/Article/details/gevjjnucy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gzpgjmhcq.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.hesvh.cn/Article/details/gnieoytap.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/geviuzine.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fehbvm.com/Article/details/gxvgqgbfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gphmisbai.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gxjdrjxvp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gxpwzztqm.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gdudrzphd.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.hesvh.cn/Article/details/ggmsverei.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gsrlzoyhy.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/getmsdgbm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gjrthyxkm.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gvwxgfekp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/glirpxjjb.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/ghortywet.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gdiaxrygx.sHtML

[Q52] 删除指定行
来源：http://www.blog.zdbjq.cn/Article/details/gdtsbiqhf.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gdbducaib.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gfcmjwela.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gfdttauox.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gjqprcslj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gogxwgwss.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gekbppriu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gfbtqjkhc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/grfrdlmqb.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gkvzvtgbd.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/ggyeazdjf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gkzpxxhyb.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/gfrsixigh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/grfebffuz.sHtML

[Q59] 分组内累计
来源：http://baike.fehbvm.com/Article/details/glewjhctx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gzxhbmjoc.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/ggqywlzxa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gyagsfvqa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gvfaaaxfk.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gunmbeyxx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmchlcwfb.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gkqsvszkk.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gtfyqczqf.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gyoxpxdyn.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.hesvh.cn/Article/details/gstfipixs.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gvbfmybne.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/gdjfxjwim.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/griximeml.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gbfdnobxo.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/gfqbyjcqh.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gwguvbpbi.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gqngohxoi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.zdbjq.cn/Article/details/gjjubulpa.sHtML

[Q68] 保存点
来源：http://www.share.hesvh.cn/Article/details/georgwjrd.sHtML

SAVEPOINT sp1;
来源：http://baike.hesvh.cn/Article/details/gqyruapiv.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gswwqpzqq.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gakryxqsr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/giumtgsbz.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/grsefljpl.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gcrjvelio.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gwenovuff.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gmbyhzwzk.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/gnbtkdscd.sHtML


<!-- 参考信息 -->