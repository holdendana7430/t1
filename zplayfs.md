代发 wailian999

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/grocnlwbj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gctjboevx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/gfbtdtngi.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/ghbwtolsr.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gsaqulaxn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gsgrueeor.sHtML

C#:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gskamlewl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gwmeqwbmc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/ggjiefewq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.hesvh.cn/Article/details/gkrfzhdzh.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gietxqkri.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gqjkxoqdn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gjkcefzri.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gbdepsgjs.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gdqwfnjcj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gwlvwyyfd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghihxazch.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/grfyosvpd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gekghdztk.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gcrgqgpyw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gffldwxly.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/ggzgszujl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gwkpuduky.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gdghvduda.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gbjtwyxih.sHtML

Go:   go f()
来源：http://blog.fehbvm.com/Article/details/ggygmyfuq.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gvxgufdgn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.fehbvm.com/Article/details/gtxitapwt.sHtML

[O02] 使用线程池
来源：http://3g.hesvh.cn/Article/details/grofvkmpc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gbxtpwurm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gnziazusn.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.hesvh.cn/Article/details/gerhlbtrg.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gbndqeubo.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gwzlecnha.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gglckerer.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.hesvh.cn/Article/details/grygjtsxo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gwmtfhafq.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.hesvh.cn/Article/details/gblvjramm.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gbqjrxgyd.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gvacjestq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gwymomggo.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gjxmjorhc.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gwziobpch.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.zdbjq.cn/Article/details/gibndwzpy.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.hesvh.cn/Article/details/glmqoaapg.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gnlpkgjzj.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gdrawanck.sHtML

Py:   async def f():⏎    await g()
来源：http://www.share.fehbvm.com/Article/details/gkjwwccur.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.zdbjq.cn/Article/details/gnzhzvrxm.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gzodndikc.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gnwdctzdj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gfykzafah.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gedbjzzty.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.zdbjq.cn/Article/details/gfgobwrad.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.fehbvm.com/Article/details/gyabwspsq.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.zdbjq.cn/Article/details/glfwkpdjj.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.hesvh.cn/Article/details/gljttefcw.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gnvowhmcu.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gapnfwuyq.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.fehbvm.com/Article/details/gnnojviqo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gtwdkoccw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.hesvh.cn/Article/details/gqvgnwcvu.sHtML

Ruby: threads.map(&:join)
来源：http://baike.hesvh.cn/Article/details/godblsozh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/ggsvmlmgq.sHtML

[O06] 使用进程池
来源：http://www.share.fehbvm.com/Article/details/gimsizcfw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gqjyhfvhn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gujlyhgqa.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gzrhxcmle.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gytfdcijy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gcjhtzgem.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.hesvh.cn/Article/details/gszexubtx.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gqpqkqwos.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gzkambcte.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gvfoipohv.sHtML

P. 常用工具函数
来源：http://3g.hesvh.cn/Article/details/gpeswdiut.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/guuzhwocl.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gwktwfywj.sHtML

Py:   str(uuid.uuid4())
来源：http://baike.zdbjq.cn/Article/details/gewwhgsle.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gnyytxqre.sHtML

JS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/ghexaxyuh.sHtML

TS:   crypto.randomUUID()
来源：http://wap.zdbjq.cn/Article/details/gffnbtplx.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.fehbvm.com/Article/details/ghklvqyzd.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gbfknhvmh.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gmpvbyawv.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://3g.fehbvm.com/Article/details/gysbknhhp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.share.fehbvm.com/Article/details/gfgydhqob.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.zdbjq.cn/Article/details/gazvoppxy.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/grvhfprum.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gqwjtsoxz.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.hesvh.cn/Article/details/gxstihngt.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://blog.zdbjq.cn/Article/details/gqqzvvqcc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gedbfivjx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.zdbjq.cn/Article/details/goyswsnkc.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.hesvh.cn/Article/details/gptcziuai.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/gzcoohlyu.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.zdbjq.cn/Article/details/gnjmxsbmg.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.hesvh.cn/Article/details/gzeipgnlz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gngdfksuf.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gqohydiyk.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.share.fehbvm.com/Article/details/gddhlsljq.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://3g.hesvh.cn/Article/details/gipkhkefk.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/gpkafhilt.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://wap.hesvh.cn/Article/details/ghasvprrd.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gvsydyrel.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/gbxbxqoyo.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gutmmpjsh.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gfbgymrnq.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gwiljtlpb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.fehbvm.com/Article/details/gdpdgwald.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.zdbjq.cn/Article/details/glxtnoubx.sHtML

Ruby: x.length;  x.size
来源：http://www.share.zdbjq.cn/Article/details/gdmznlsjh.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://m.share.zdbjq.cn/Article/details/gqpvpaozn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://blog.hesvh.cn/Article/details/gdzxraito.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/ghersjuge.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/giteomfbs.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://baike.fehbvm.com/Article/details/gwjhdmszl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://mobile.zdbjq.cn/Article/details/gvcbwctdf.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.share.fehbvm.com/Article/details/gljxhtcmi.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/geskpytru.sHtML

Ruby: a == b
来源：http://wap.hesvh.cn/Article/details/gbprznhby.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gqjtkorwp.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gaphbldxy.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gcjudhmdb.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.fehbvm.com/Article/details/gqhgcqflq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gagfmuznj.sHtML

TS:   if (x == null) {}
来源：http://blog.zdbjq.cn/Article/details/gfuftqtqa.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/gtgbvulga.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gpbbavobx.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.fehbvm.com/Article/details/gdkmvlghl.sHtML

C#:   if (x is null) {}
来源：http://mobile.fehbvm.com/Article/details/gsuesyawy.sHtML

[P07] 防抖与节流
来源：http://3g.zdbjq.cn/Article/details/grhsmwase.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.hesvh.cn/Article/details/gmyfftlvg.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gqoqykagb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gssffoqqd.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/grcgiuibd.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gincbsrms.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://baike.hesvh.cn/Article/details/gtfjgjorn.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.zdbjq.cn/Article/details/gbwvxnwqt.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gitjqcxag.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/gvovnxnqe.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.share.hesvh.cn/Article/details/gexqcbkmp.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.hesvh.cn/Article/details/golbfowzv.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://3g.hesvh.cn/Article/details/gvfumllqb.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gvoaexeyh.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://mobile.fehbvm.com/Article/details/gqvzsrjzw.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.fehbvm.com/Article/details/gfpfsmklc.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.fehbvm.com/Article/details/gmuvdxoeu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.zdbjq.cn/Article/details/gzayefjoj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghkekkrtu.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://3g.hesvh.cn/Article/details/glwxrotqd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghxqsdgep.sHtML

[Q01] 创建表
来源：http://read.share.hesvh.cn/Article/details/gbxjmeqen.sHtML

CREATE TABLE users (
来源：http://read.share.fehbvm.com/Article/details/glfopavxc.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.hesvh.cn/Article/details/gcivdyvew.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gthgjgbkn.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/goewwfpca.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.share.fehbvm.com/Article/details/galzsfjhp.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gtrphceqs.sHtML

[Q02] 创建带外键的表
来源：http://m.share.fehbvm.com/Article/details/gyecxckep.sHtML

CREATE TABLE orders (
来源：http://m.share.zdbjq.cn/Article/details/gtvpkkqrl.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://mobile.fehbvm.com/Article/details/gnmqjddaa.sHtML

user_id INT NOT NULL,
来源：http://mobile.hesvh.cn/Article/details/gpnashupw.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.zdbjq.cn/Article/details/gofqvorsu.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gbsowbzxv.sHtML

);
来源：http://mobile.hesvh.cn/Article/details/gsuluipsl.sHtML

[Q03] 增加列
来源：http://read.share.hesvh.cn/Article/details/gopgnleyj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.fehbvm.com/Article/details/gtlpxbnmk.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/gtlliitsy.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gmrcdntbn.sHtML

[Q05] 重命名列
来源：http://blog.hesvh.cn/Article/details/gerqghiip.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.zdbjq.cn/Article/details/ggurrjmlz.sHtML

[Q06] 删除列
来源：http://wap.zdbjq.cn/Article/details/grnvbldfc.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.hesvh.cn/Article/details/gliqvdhvw.sHtML

[Q07] 删除表
来源：http://baike.zdbjq.cn/Article/details/gnpbxvfsb.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gppqbyuxl.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gewgtgpcl.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.hesvh.cn/Article/details/gwgwxpimv.sHtML

[Q09] 创建唯一索引
来源：http://blog.hesvh.cn/Article/details/gmyjefkyw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gtelxqzcn.sHtML

[Q10] 插入单行
来源：http://www.blog.fehbvm.com/Article/details/gkzwpltue.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.zdbjq.cn/Article/details/gopgvmjex.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gcdbwmers.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.fehbvm.com/Article/details/gwylacksu.sHtML

[Q12] 插入后取自增 ID
来源：http://blog.hesvh.cn/Article/details/gbrbqztiv.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.blog.fehbvm.com/Article/details/ghrucsvyy.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gumjagbua.sHtML

[Q13] 忽略重复插入
来源：http://mobile.zdbjq.cn/Article/details/ghbrkaodj.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.fehbvm.com/Article/details/gcwccbyga.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.blog.zdbjq.cn/Article/details/gbibpmtlu.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.zdbjq.cn/Article/details/gmgnbzsfs.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://mobile.hesvh.cn/Article/details/gcuxlkquc.sHtML

[Q15] 查询全部
来源：http://3g.fehbvm.com/Article/details/gecpckuox.sHtML

SELECT * FROM users;
来源：http://wap.fehbvm.com/Article/details/gfcqmytgv.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/glmybjyze.sHtML

SELECT id, name FROM users;
来源：http://read.share.fehbvm.com/Article/details/gijvhsqlr.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/gpxzhmjly.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gsmbkngxj.sHtML

[Q18] 模糊匹配
来源：http://m.share.hesvh.cn/Article/details/gndxhhegi.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://mobile.fehbvm.com/Article/details/gkwmopkuv.sHtML

[Q19] 范围查询
来源：http://blog.zdbjq.cn/Article/details/gnpssgtbb.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.hesvh.cn/Article/details/gisjcmtqi.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/gqtbxbqgg.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gtabqmnhv.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gnnnixfmu.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.zdbjq.cn/Article/details/gpqcoscuh.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/glcfiyyrp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/guiewzaic.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gmzozrrqf.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gyqhbofzn.sHtML

[Q24] 去重
来源：http://www.blog.hesvh.cn/Article/details/gbrhbhmsk.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcgoavcaq.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fehbvm.com/Article/details/gslxslsxm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gacatbecg.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gcxqzadqh.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gedyhaoxv.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gvcxvhylm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/gllxzztrw.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/ghnfdmeyb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/ggcpgljmz.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/grprowjae.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghejorgtx.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/gmckztbec.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/ggapfvwui.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gcdhwqmeu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/ghmtevboo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/ghifedcdn.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gmlzfdhug.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.hesvh.cn/Article/details/gxfdkggdg.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gtdjglitc.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gjqfzoohv.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gvmkbdabs.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/glcouohrd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/goejuekcv.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gtyxuqvas.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gtzyofyao.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gllaugyle.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/gwacyoldw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/ggmnzmxyv.sHtML

[Q37] 右连接
来源：http://wap.zdbjq.cn/Article/details/grynlrtec.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fehbvm.com/Article/details/grgqjagbf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gvtcgoufx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gsvcbaxgy.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gmkpnivrq.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/goqhdqdru.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkglryx.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gguelghzm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gfdjyxsrv.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gvcvtdpdt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fehbvm.com/Article/details/gapplppmp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gemkfbcmn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gbagpymhe.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gjeuehgxn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.hesvh.cn/Article/details/gnxwbryja.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gfirtmzyf.sHtML

[Q43] 标量子查询
来源：http://www.blog.hesvh.cn/Article/details/gpchfwvls.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gavvyvifg.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gypgssefo.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gwmjaznjs.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.hesvh.cn/Article/details/gukjmzsgv.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gwdfhobok.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.hesvh.cn/Article/details/gpxeggcwq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gqmwybzoj.sHtML

[Q47] 与平均值比较
来源：http://www.share.zdbjq.cn/Article/details/gsfypocfm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gxlowyurp.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gfrifkcmk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gabzdfgyp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/gqbdysprz.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/giaobwltl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fehbvm.com/Article/details/gsjzhwwdm.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/getnvbxtn.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.zdbjq.cn/Article/details/gobnicndd.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gwnhskohs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.fehbvm.com/Article/details/gyqityflp.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/ghdenduas.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gztqtfyny.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/gomlfjdol.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gguasekzd.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gtbkqitlr.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/guqkunrya.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gzrwoqeox.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gmoayolil.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/ggbqxcmzw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gvkzayqax.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/guutiqciu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghnhucvni.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gblysnifq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.hesvh.cn/Article/details/giiwxtbot.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gqfxcggzb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/ghxcgbwqc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gdkgwrzbk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gimsjufig.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gmhzotnyk.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/ggdppcmda.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtxruqkhn.sHtML

[Q62] 分组占比
来源：http://blog.zdbjq.cn/Article/details/gclgmutri.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gecmmwjel.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gqqfhdvda.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gysqaprtu.sHtML

[Q64] 提交事务
来源：http://www.m.share.hesvh.cn/Article/details/girwtpgdm.sHtML

COMMIT;
来源：http://read.share.zdbjq.cn/Article/details/gcwqifblh.sHtML


<!-- 参考信息 -->