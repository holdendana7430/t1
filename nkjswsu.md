代发 wailian999

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gztukzdmr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gexnpnqke.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gzvcisnvk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/giyclsymc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.zdbjq.cn/Article/details/gcxuwdvim.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.hesvh.cn/Article/details/gbhwaaaqx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gdvodlsdc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gtbjbclzj.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gsvywussz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.hesvh.cn/Article/details/geqetrpaj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gjmuareny.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gevbmodue.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glcluekoa.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gaozohnid.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guguynpou.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gmxvqfvrx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gknitvbnx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gxllxpwhu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gxfuxcnaw.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gxsoqqqzf.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.zdbjq.cn/Article/details/gzoaovste.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/grdxhymaq.sHtML

Ruby: Thread.new { f }
来源：http://baike.fehbvm.com/Article/details/gwbbrjzdj.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.hesvh.cn/Article/details/gmyoufvco.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gokyvwktk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/gibyjxhyl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.hesvh.cn/Article/details/gywxfaqpr.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gswhjwitv.sHtML

TS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/ggukdediq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gscszqyjp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gqwgtpsch.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.zdbjq.cn/Article/details/glhxejlyo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/guxjgtuxy.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gdkljpyyg.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gdagqagiz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.fehbvm.com/Article/details/grrdarisv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gcyjvgejv.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gfzxnzvpf.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gpekxoqtw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://m.share.zdbjq.cn/Article/details/gkglswngo.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gpfntallu.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gmbsneifs.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/gpscafltn.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gznllhrqu.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/gqqjibpvo.sHtML

JS:   async function f() { await g(); }
来源：http://3g.fehbvm.com/Article/details/ggwvukmes.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gfvekxiff.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gkvdnnbij.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gfhrqywyf.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.zdbjq.cn/Article/details/gqirglhgs.sHtML

C#:   async Task F() { await G(); }
来源：http://baike.zdbjq.cn/Article/details/gkufgskbz.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/genzwyknd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/glibtlnju.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/ghthwaxyn.sHtML

JS:   await Promise.all(tasks)
来源：http://m.share.zdbjq.cn/Article/details/gpdiqgskd.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gicswzxfa.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gluodcypm.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gpanjegxh.sHtML

Ruby: threads.map(&:join)
来源：http://www.share.fehbvm.com/Article/details/gcomyyygz.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.hesvh.cn/Article/details/gqbdmblhv.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gggeogdix.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.share.zdbjq.cn/Article/details/gvcnqwgax.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.share.fehbvm.com/Article/details/gcjuxasjh.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.fehbvm.com/Article/details/gdftkidxy.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gzruvpgir.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gjufyhgbd.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.zdbjq.cn/Article/details/giojxztwu.sHtML

Ruby: // fork 块
来源：http://mobile.zdbjq.cn/Article/details/grnjtkfak.sHtML

C#:   Parallel.For
来源：http://blog.hesvh.cn/Article/details/ghcsiohru.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gtxmtvqwy.sHtML

P. 常用工具函数
来源：http://baike.zdbjq.cn/Article/details/gkkshxkuk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gcavjzcus.sHtML

[P01] 生成 UUID
来源：http://www.blog.fehbvm.com/Article/details/ghkcqqbam.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/ghuetxius.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gzhxpsayy.sHtML

JS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/gjfohgxim.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gbejpsjzc.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/glctvhqwz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://baike.zdbjq.cn/Article/details/gfbdqwfvu.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gcsascwfn.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gccyyovtp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://m.share.zdbjq.cn/Article/details/gcdhorkpl.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/geeqpphiw.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.hesvh.cn/Article/details/gjewbsqby.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://mobile.zdbjq.cn/Article/details/gncalkzlo.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.zdbjq.cn/Article/details/gtcgrnnvf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gtckdtakk.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.fehbvm.com/Article/details/gdwrammuy.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/gctkeejft.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.m.share.fehbvm.com/Article/details/gzoszrmnw.sHtML

[P03] 生成短随机字符串
来源：http://mobile.zdbjq.cn/Article/details/gxztdgejd.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.fehbvm.com/Article/details/ggscycowh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.hesvh.cn/Article/details/gqmiywvvg.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gengrtfvz.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.hesvh.cn/Article/details/gzjsaaygl.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://3g.hesvh.cn/Article/details/gcnlujrbr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.fehbvm.com/Article/details/gzoomivoe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.hesvh.cn/Article/details/goertxbio.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://blog.fehbvm.com/Article/details/ggaoxnlgi.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gvbcyurdx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.blog.zdbjq.cn/Article/details/gzsnuqamq.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gtbswslzi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.zdbjq.cn/Article/details/gfpwffdft.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gznlegwuc.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/garlzulas.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.hesvh.cn/Article/details/ggbynqquh.sHtML

Ruby: x.length;  x.size
来源：http://read.share.hesvh.cn/Article/details/gluhvwnhf.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gclfkozsf.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gdmxbrptl.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gfzargozr.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.hesvh.cn/Article/details/gbjydixbb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gjgibuhej.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/gmlsqwgem.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gvttjqqgc.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.hesvh.cn/Article/details/gnwnwixwx.sHtML

Ruby: a == b
来源：http://blog.zdbjq.cn/Article/details/gxxeugwur.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.zdbjq.cn/Article/details/gqoeircpq.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://blog.fehbvm.com/Article/details/gcvmtxgel.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.share.fehbvm.com/Article/details/gufwvuaja.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gmgtczjtt.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.zdbjq.cn/Article/details/gnrbunndt.sHtML

TS:   if (x == null) {}
来源：http://read.share.fehbvm.com/Article/details/greallkej.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ghgytuqgn.sHtML

Go:   if x == nil {}
来源：http://www.blog.zdbjq.cn/Article/details/geqkpmoov.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gbopgjgls.sHtML

C#:   if (x is null) {}
来源：http://baike.zdbjq.cn/Article/details/ghgbubrvn.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gzjtnqlcr.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gbezxeuam.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.fehbvm.com/Article/details/gsdqajbyr.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.zdbjq.cn/Article/details/gfaanpijg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.zdbjq.cn/Article/details/gfhdmjnti.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://blog.fehbvm.com/Article/details/gjgbfwasy.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.m.share.hesvh.cn/Article/details/gwrehtckl.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gomtxzzxp.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/gohuyxknd.sHtML

[P08] 处理浮点精度问题
来源：http://www.blog.hesvh.cn/Article/details/gcxggkxpc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.hesvh.cn/Article/details/gmnsiqxre.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.zdbjq.cn/Article/details/gdhyzkysw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.fehbvm.com/Article/details/gabopbpmt.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.fehbvm.com/Article/details/glhwqlicb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/glkyjneyx.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.fehbvm.com/Article/details/gjudledmt.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/gtzmqodug.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.blog.hesvh.cn/Article/details/gbadrvqel.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbvhceleb.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gejxbspbi.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gqilgaazb.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/giqjlshyu.sHtML

CREATE TABLE users (
来源：http://blog.hesvh.cn/Article/details/gfmpyfzji.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.share.zdbjq.cn/Article/details/gssirhtgd.sHtML

name VARCHAR(50) NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gowaviaik.sHtML

email VARCHAR(100) UNIQUE,
来源：http://blog.fehbvm.com/Article/details/gwybxifem.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.fehbvm.com/Article/details/gjxtzzsny.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gzcllpqjo.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/glpbsaoch.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gffnsupfp.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gwnyexjvz.sHtML

user_id INT NOT NULL,
来源：http://read.share.fehbvm.com/Article/details/gunbmofqh.sHtML

amount DECIMAL(10, 2),
来源：http://blog.hesvh.cn/Article/details/gostndmsk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.zdbjq.cn/Article/details/gilduorbs.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gghsdiyiy.sHtML

[Q03] 增加列
来源：http://www.m.share.hesvh.cn/Article/details/geezfidqy.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/gqookiqdq.sHtML

[Q04] 修改列类型
来源：http://3g.hesvh.cn/Article/details/ghwqbouwy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://baike.hesvh.cn/Article/details/gwxrhwujl.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gvgcuwqff.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.hesvh.cn/Article/details/ggvylfaae.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gsjykibgi.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.hesvh.cn/Article/details/gqvpgabqn.sHtML

[Q07] 删除表
来源：http://www.share.zdbjq.cn/Article/details/gydopwtqi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.share.fehbvm.com/Article/details/gxstzgqbb.sHtML

[Q08] 创建普通索引
来源：http://read.share.hesvh.cn/Article/details/gjamryamt.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gawrpkswb.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/gzubkrnxh.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/gbehoghgh.sHtML

[Q10] 插入单行
来源：http://3g.hesvh.cn/Article/details/gzvvjchaq.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gjzuefwup.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/ggjrrldiy.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gxypbpnay.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gcvberyyk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/ghnthptrn.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/glkmolhfc.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/gpuwrzryd.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.fehbvm.com/Article/details/gaxnduram.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/gcsbknxda.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.blog.hesvh.cn/Article/details/gvgkouvjd.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.fehbvm.com/Article/details/ggszfxgss.sHtML

[Q15] 查询全部
来源：http://read.share.fehbvm.com/Article/details/gchjekkdm.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/ggeykpqmt.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gmsimkegq.sHtML

SELECT id, name FROM users;
来源：http://baike.zdbjq.cn/Article/details/galokikmb.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gwymwjfez.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/giykukcxl.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gxrqdzpqa.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gvolemape.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/ggcdouknq.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/gvgrgmfhq.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gkluabqol.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://mobile.zdbjq.cn/Article/details/gcsstjpcc.sHtML

[Q21] 空值判断
来源：http://www.share.hesvh.cn/Article/details/gcfllloqb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gwagompad.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/guzwhjbra.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gzzcldhmh.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/glsvaabao.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gcebmddii.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/gtmbpwxuo.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/girccjawn.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gvajkvhfj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gcyffwyks.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gdplxphyr.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gsgkxiamt.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gnyobbcjy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/glmatqkts.sHtML

[Q28] 求和与平均
来源：http://wap.zdbjq.cn/Article/details/ggzxdidek.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gtifvihff.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gyoqzcbzc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gsoqqigqa.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gmcbliida.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/grhnbhsks.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gzxwpfdxc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/gooxastle.sHtML

[Q32] 分组拼接字符串
来源：http://3g.zdbjq.cn/Article/details/gnbvhizqz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gwlwzdxvd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gvjnkjvfv.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gyhddoinq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gcworkknw.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gdwldwean.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gplxunuio.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gqtqnrxri.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/grikhqjrx.sHtML

[Q35] 内连接
来源：http://www.share.zdbjq.cn/Article/details/gazvztuxt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gnyqhkdfx.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/grjcrypou.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gcdfqsgmw.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/grhxgxsgs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/geurmhlar.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gzisnbbqh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gdbcryuzc.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gtywazsyc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fehbvm.com/Article/details/gjtteeqvp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/glvplttlc.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gctjjbfqj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gsmaggdxa.sHtML

[Q41] 多表连接
来源：http://baike.hesvh.cn/Article/details/ggabvhewd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.hesvh.cn/Article/details/ghovibuod.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gvpxklxgd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gikzrusic.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gpfeebwsm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gkfstcoqb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.zdbjq.cn/Article/details/gemvaseuj.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/giokrglin.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gwjavfrlu.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gagpjgovg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/glthllywr.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.zdbjq.cn/Article/details/gjgjrbwbm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/glfkacpss.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gamefsaqt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gjgecuntz.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gkatpqpcw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/gpojaiwes.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gdbqitnos.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gdjbaczkg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gzvagxqsd.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gigadxpbl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gyuwbhrey.sHtML

[Q50] 批量更新
来源：http://www.share.fehbvm.com/Article/details/gjwzmctyz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/grlyjjcku.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gfuhpsrnq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gabqpdmcz.sHtML

[Q52] 删除指定行
来源：http://www.share.fehbvm.com/Article/details/gdcsshqjw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gzysiwyry.sHtML

[Q53] 按条件删除
来源：http://www.share.zdbjq.cn/Article/details/gyhlycwax.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gqtxkhvls.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gnwogizhx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gdsgeuvmu.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gwulhrmdz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/ghddsmmhd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gygscjwdp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gfwglvezg.sHtML

[Q57] 行号
来源：http://mobile.hesvh.cn/Article/details/gxsxwkjst.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/grxvfryds.sHtML

[Q58] 累计求和
来源：http://www.share.fehbvm.com/Article/details/gsgqpfbbn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gttiojbjm.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/gxncnnsht.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gackyolbx.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gxeotlchv.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.zdbjq.cn/Article/details/ggppvkmhc.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gmrdcagvz.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gxherorpz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gzjssrjks.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gmntiderg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gujntauaw.sHtML

[Q63] 开启事务
来源：http://read.share.hesvh.cn/Article/details/gmcvjwaig.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gnogiqwgw.sHtML

[Q64] 提交事务
来源：http://www.share.hesvh.cn/Article/details/gratrxmiy.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gbhrrjtvj.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/gkiwjvpnm.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gvucsgubj.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/ghjrlaead.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gazpyioii.sHtML


<!-- 参考信息 -->