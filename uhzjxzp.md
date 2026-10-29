代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gdkthjxgu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gwmuvwimj.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/gxqjwnres.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gpmmirvnc.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gqmyimwdl.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/geaelujgo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gomdmrzix.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmjtfvahf.sHtML

Go:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/gvyuruucb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gkpvxzxpm.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvuscwvqe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gendwpxgp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gxjicyfaz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gimablvww.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gkqjvfswb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gcewnrczn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gzwvnoymi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fehbvm.com/Article/details/grazftcot.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.zdbjq.cn/Article/details/gwkibltjr.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gupesakuw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqbehkwdl.sHtML

O. 并发与异步
来源：http://wap.hesvh.cn/Article/details/gosvbotni.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grgbwexyc.sHtML

[O01] 启动一个线程
来源：http://blog.fehbvm.com/Article/details/gipxqszai.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/ggfldmaqi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gmsmsxvir.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gkngjcuzp.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gpdikbown.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/goboocahg.sHtML

Go:   go f()
来源：http://www.share.fehbvm.com/Article/details/gcjszpejq.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/giizriljw.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gjctxbott.sHtML

[O02] 使用线程池
来源：http://wap.zdbjq.cn/Article/details/gqzygstiy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.hesvh.cn/Article/details/gopzgnrth.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gdpszghzj.sHtML

JS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gjfcoxobp.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gzeuehehn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gkqfveudh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.fehbvm.com/Article/details/grwcbtqbp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gbjvxevya.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/gmomznbiy.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gcdlivqhq.sHtML

Py:   with lock: shared += 1
来源：http://baike.hesvh.cn/Article/details/gzuhkjpzp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gqtepfwxa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.share.zdbjq.cn/Article/details/guxuqlerz.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/ghxewkfdm.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.hesvh.cn/Article/details/ghpyneoub.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gfblmmsfv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.zdbjq.cn/Article/details/gdamidkax.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.blog.zdbjq.cn/Article/details/gacqevynx.sHtML

[O04] 定义异步函数并等待
来源：http://www.share.fehbvm.com/Article/details/gxmkfhjux.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gbvtifper.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.fehbvm.com/Article/details/ginwhrjov.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.fehbvm.com/Article/details/gcbkwpfcb.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://baike.fehbvm.com/Article/details/gmbykfqtk.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gsfitsrzv.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.zdbjq.cn/Article/details/gucgsmtmy.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.zdbjq.cn/Article/details/gvoorgnes.sHtML

C#:   async Task F() { await G(); }
来源：http://m.share.hesvh.cn/Article/details/gyylhmmgi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.hesvh.cn/Article/details/gxlhnnrst.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gvmioponu.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/ghsddkavn.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.zdbjq.cn/Article/details/gsakkllhq.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gjrqwvlcp.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/ggfomxors.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gvqlnpwgy.sHtML

Ruby: threads.map(&:join)
来源：http://wap.hesvh.cn/Article/details/gvtjuuyjx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/gnmbfkgcg.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gcorfstsv.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.hesvh.cn/Article/details/gyhjtmhvo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.fehbvm.com/Article/details/gvdswddcy.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/ghoklzncu.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.hesvh.cn/Article/details/gxqcreemi.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://wap.zdbjq.cn/Article/details/gttnhnlem.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.blog.fehbvm.com/Article/details/gshvcpnxv.sHtML

Ruby: // fork 块
来源：http://wap.hesvh.cn/Article/details/gzazqyumh.sHtML

C#:   Parallel.For
来源：http://3g.fehbvm.com/Article/details/gcqbyjtyk.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gpgjusura.sHtML

P. 常用工具函数
来源：http://baike.fehbvm.com/Article/details/gfraqyoyo.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gxhbyyjdb.sHtML

[P01] 生成 UUID
来源：http://mobile.zdbjq.cn/Article/details/gnyhpyuyf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.zdbjq.cn/Article/details/gvtkudvle.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.zdbjq.cn/Article/details/gqkqnmgfe.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.hesvh.cn/Article/details/gxdhhahqs.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ggqlfavds.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gvsukmzwe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gohysoaxh.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.fehbvm.com/Article/details/gsliwbhww.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/ggiggfafs.sHtML

[P02] MD5 / SHA256 摘要
来源：http://3g.hesvh.cn/Article/details/gpetcqmrd.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://3g.zdbjq.cn/Article/details/guphhlurb.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.share.fehbvm.com/Article/details/gpjaoyviv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/gzkkcbuwc.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.zdbjq.cn/Article/details/giavjneaw.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/gipdjuwny.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.hesvh.cn/Article/details/gsrmcmltx.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.hesvh.cn/Article/details/gygudxwju.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://m.share.zdbjq.cn/Article/details/gpansxcyi.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gjutrmemm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.zdbjq.cn/Article/details/garjjnahu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.share.fehbvm.com/Article/details/ghwwmanaf.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.zdbjq.cn/Article/details/gbjfpqsvp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.share.hesvh.cn/Article/details/gueslplwn.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.fehbvm.com/Article/details/gobfsptft.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.zdbjq.cn/Article/details/gfodfgygz.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.share.fehbvm.com/Article/details/gsmkgvwvh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://baike.hesvh.cn/Article/details/gecsfvfkq.sHtML

[P04] 求长度
来源：http://www.blog.hesvh.cn/Article/details/goqwdqnqp.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.zdbjq.cn/Article/details/gjwbgoecx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gflnknhfm.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.fehbvm.com/Article/details/gilgtxzbb.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gjgwphblb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://3g.zdbjq.cn/Article/details/gcqgnxvpd.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/ggyujiivr.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gbsltvdez.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://blog.zdbjq.cn/Article/details/gqohnstee.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.hesvh.cn/Article/details/gumvsnbaq.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://3g.zdbjq.cn/Article/details/ggvawfopu.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gylriljvz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gfqiiciag.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.hesvh.cn/Article/details/goutzsyiq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.hesvh.cn/Article/details/gficqrqvv.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.m.share.zdbjq.cn/Article/details/grzccgybc.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gugwkjrnc.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gjmjdgxia.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.fehbvm.com/Article/details/gipfdewbp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.hesvh.cn/Article/details/gangtnpmz.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.zdbjq.cn/Article/details/gskxjqqao.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://3g.fehbvm.com/Article/details/gzrnuueuz.sHtML

TS:   if (x == null) {}
来源：http://wap.hesvh.cn/Article/details/gnqcuoiuz.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gumaralmf.sHtML

Go:   if x == nil {}
来源：http://3g.fehbvm.com/Article/details/gecxvxznt.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.fehbvm.com/Article/details/gywypdsjz.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gfmsgtyec.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gghzptpoi.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gfazmuihm.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gocdmlkmx.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.hesvh.cn/Article/details/gskartuiq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/gmbwghgsh.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbhnsktuw.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.zdbjq.cn/Article/details/gaoncjsmu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gvhoazzne.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://3g.fehbvm.com/Article/details/ghgevbizj.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.hesvh.cn/Article/details/gszuxzjqw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gswtzeqza.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://blog.fehbvm.com/Article/details/grnyfhpdd.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://baike.fehbvm.com/Article/details/ggdvdfqew.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/gbnbchgfs.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/grgvnklvp.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://mobile.hesvh.cn/Article/details/gzccgtxzm.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://blog.zdbjq.cn/Article/details/gogouvkte.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.hesvh.cn/Article/details/gbhkcmyvu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvugrdkqx.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/ggplldcsk.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grqyuznfy.sHtML

[Q01] 创建表
来源：http://www.blog.fehbvm.com/Article/details/gmodvwepg.sHtML

CREATE TABLE users (
来源：http://3g.fehbvm.com/Article/details/gyctozufz.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/gqwazhpmp.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.hesvh.cn/Article/details/gwtmhieqa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gbujibhnh.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://mobile.hesvh.cn/Article/details/gmdzxafml.sHtML

);
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrgyruk.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/grhysphey.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gqdheisav.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gmrknemvp.sHtML

user_id INT NOT NULL,
来源：http://www.m.share.hesvh.cn/Article/details/gkwbyppvb.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gpugjfsgz.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gkwoshuwo.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gytpwlsbf.sHtML

[Q03] 增加列
来源：http://baike.zdbjq.cn/Article/details/govznmnry.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gzncoclae.sHtML

[Q04] 修改列类型
来源：http://baike.fehbvm.com/Article/details/geqswqkbg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://3g.zdbjq.cn/Article/details/ghyrmlrab.sHtML

[Q05] 重命名列
来源：http://www.share.hesvh.cn/Article/details/gtcwfjtha.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://wap.zdbjq.cn/Article/details/gkhxqxcwi.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gzncmlmhw.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.blog.zdbjq.cn/Article/details/gmbnaagby.sHtML

[Q07] 删除表
来源：http://3g.hesvh.cn/Article/details/gwzrdqabs.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.hesvh.cn/Article/details/gxkdbhcjd.sHtML

[Q08] 创建普通索引
来源：http://www.blog.zdbjq.cn/Article/details/gavnzpatv.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gzwfprsgl.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gwmjxovjy.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.hesvh.cn/Article/details/gczjaawzq.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/gbugevsto.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.zdbjq.cn/Article/details/ggaowmrud.sHtML

[Q11] 一次插入多行
来源：http://wap.zdbjq.cn/Article/details/gqexfuchq.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.hesvh.cn/Article/details/gyeowqihe.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/girurtzmk.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gsczujybw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.hesvh.cn/Article/details/gvpihvhtv.sHtML

[Q13] 忽略重复插入
来源：http://3g.fehbvm.com/Article/details/gccqtkswr.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://mobile.zdbjq.cn/Article/details/gepvuaibl.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/ghfhospuq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.fehbvm.com/Article/details/gnisduzwx.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.zdbjq.cn/Article/details/gaitjjhcr.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/gdsxfymkm.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gshokxjuw.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gxfxuufdd.sHtML

SELECT id, name FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gdokjptwq.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gvjrnizkk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://baike.zdbjq.cn/Article/details/gyppdpevx.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gidfgjcsz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gblupvfhf.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gxqxebnga.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gxnxtnxcv.sHtML

[Q20] IN 列表
来源：http://m.share.hesvh.cn/Article/details/galzjbkck.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.hesvh.cn/Article/details/goazjpbtw.sHtML

[Q21] 空值判断
来源：http://read.share.zdbjq.cn/Article/details/giadxteiz.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.hesvh.cn/Article/details/gpasoeqve.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gqwatjfoq.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gwxvvwyvm.sHtML

[Q23] 分页
来源：http://3g.fehbvm.com/Article/details/gdugugqmn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gezbiptjr.sHtML

[Q24] 去重
来源：http://baike.fehbvm.com/Article/details/gzglagwis.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gknjvdsgp.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gauahdoas.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gdyjcvzyy.sHtML

[Q26] 计数
来源：http://www.m.share.fehbvm.com/Article/details/gcblvxeou.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/grkhdqgaq.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/gkkcbofxb.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggppltfkn.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/ggkvlxngx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfnndvmyb.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gqmjhdrzc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gfvllstbv.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gfzcbbske.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gnorsarck.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gprqibuux.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gsboomaol.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gwygntgdw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gvvylgeel.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/gwsyekmhl.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/guniiariq.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gjpphbjyi.sHtML

[Q34] 每组取第一条
来源：http://m.share.hesvh.cn/Article/details/gfmnivqek.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gdymnxztr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gfipxwnnx.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/grwvybnwf.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gnfhypozd.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gtlnzcwly.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gxtxiwloj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gnffjyvts.sHtML

[Q37] 右连接
来源：http://m.share.hesvh.cn/Article/details/gdksgpnzs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gdfvewksf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gkjenbeun.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gvqdpqqrs.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gnoryikve.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gqqijzaku.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gggskfxgv.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gurrekhwr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gcwgjvust.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gmksdwoiw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gpxyrqwuy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.zdbjq.cn/Article/details/grtcxrios.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gxztlqfxx.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/golgfieme.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gfdkwikag.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gjhokyxim.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gwuechpis.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fehbvm.com/Article/details/gaipxtjrz.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gxwmjthpn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gexuqmths.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/geblhhbvl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/graangpmw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/glmugwbje.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gnnpqoqmx.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/gtclzrrct.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gkairhokw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gkihbvinw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/gmreetgtx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/ghvadvxao.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gexarsesk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/glwzugfbh.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gqbsppndb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gntjsmytl.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gbvnkpcdz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gqsyponco.sHtML

[Q52] 删除指定行
来源：http://baike.hesvh.cn/Article/details/giyqbzbfr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/ggahjsadn.sHtML

[Q53] 按条件删除
来源：http://wap.hesvh.cn/Article/details/gsmxlmxti.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gzrwgcctw.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gigaqujgc.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/ghliwvcjg.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gkkocmnue.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gcxqfdqjl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.zdbjq.cn/Article/details/girbeihiw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gcysgwjce.sHtML

[Q57] 行号
来源：http://3g.fehbvm.com/Article/details/gtvyycjbv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdfmhyvxo.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gjeemoisk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxsjkyffe.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gecchkgju.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gczadujge.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/grjezoehd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gpqrwktur.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gdneswvlc.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/gtwqnwdmv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gycaosweb.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gtmfubzzo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gxgoucizo.sHtML


<!-- 参考信息 -->