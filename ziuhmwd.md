代发 wailian999

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.fehbvm.com/Article/details/gkdcelflr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gshgggzne.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gnqkzbkih.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gnhsooqea.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gfxarweuf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gchaqxbln.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gxickcxus.sHtML

Java: // 手写递归
来源：http://mobile.fehbvm.com/Article/details/ganawfcfm.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gxrijncnm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.hesvh.cn/Article/details/gnszjaxxc.sHtML

C#:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gsdzexcwh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.fehbvm.com/Article/details/gwnujtgaa.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gyvwuruad.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gsccrhnfk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gwapdjtwl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gegbidcwu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/glvghnfyi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gdmvigwsh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/ggwzyhtch.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/grewfbcwj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtdwhjmxr.sHtML

O. 并发与异步
来源：http://read.share.zdbjq.cn/Article/details/gngmsyjej.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmeghoanz.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gnhmfoixl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/giaadejgf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/gqrlhygxq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.hesvh.cn/Article/details/gilflkmtm.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gfmhsjwsl.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gsenaihtw.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gpmymspnb.sHtML

Ruby: Thread.new { f }
来源：http://read.share.fehbvm.com/Article/details/gbioqjixl.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.fehbvm.com/Article/details/gmmhkvxqv.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gqtxkjlld.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.zdbjq.cn/Article/details/gtoqblcng.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.hesvh.cn/Article/details/gawpvlhwu.sHtML

JS:   // worker_threads 线程池
来源：http://www.share.fehbvm.com/Article/details/goalgekzf.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gsgawzlzy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.fehbvm.com/Article/details/gyraczpor.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.fehbvm.com/Article/details/gjluncpkw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/gdpndtfny.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.fehbvm.com/Article/details/gitvfuvzw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gjlkvsjkl.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/gqnjosoyp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.hesvh.cn/Article/details/gnaracxeh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.zdbjq.cn/Article/details/gsfsilwof.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gwindoknm.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.fehbvm.com/Article/details/gusfsjexv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.fehbvm.com/Article/details/gwexzhtkc.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gwusvbtaw.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzfrtthui.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gfxndxgse.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.fehbvm.com/Article/details/gmkwajhjp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gntwifzns.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gjqktfybz.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.hesvh.cn/Article/details/gheuzazfd.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://3g.hesvh.cn/Article/details/gcxyfqvbu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.zdbjq.cn/Article/details/glcqjuiqk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gmcswwczk.sHtML

C#:   async Task F() { await G(); }
来源：http://3g.fehbvm.com/Article/details/grjbmxoqp.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.fehbvm.com/Article/details/gpxqggdgx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/galguttlc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gjervlctb.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/ggmupkwqk.sHtML

TS:   await Promise.all(tasks)
来源：http://mobile.hesvh.cn/Article/details/glppfwtcd.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.fehbvm.com/Article/details/gifjomuwg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.fehbvm.com/Article/details/gbhiggxco.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gixmctxrd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gujlhgqte.sHtML

[O06] 使用进程池
来源：http://blog.fehbvm.com/Article/details/gwttjomgr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gtstxdelo.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.m.share.fehbvm.com/Article/details/gmhkvqrkp.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.zdbjq.cn/Article/details/gkknstvwn.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.zdbjq.cn/Article/details/gihvgfytn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.zdbjq.cn/Article/details/gicpkqetx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://m.share.hesvh.cn/Article/details/gwojrhiyw.sHtML

Ruby: // fork 块
来源：http://3g.hesvh.cn/Article/details/gmrokaqgq.sHtML

C#:   Parallel.For
来源：http://baike.fehbvm.com/Article/details/geqsiurcn.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyeiqjvgt.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gydlxauyv.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gakpuzqrn.sHtML

[P01] 生成 UUID
来源：http://m.share.fehbvm.com/Article/details/gsglkeies.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.hesvh.cn/Article/details/gtnbccuvg.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gmrhowwft.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ggikmztfz.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gfipoiqaw.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.zdbjq.cn/Article/details/gexnlvcwo.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gxuaeiifg.sHtML

Ruby: SecureRandom.uuid
来源：http://www.blog.zdbjq.cn/Article/details/gtvoilqce.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.hesvh.cn/Article/details/gcvoabmrn.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gebawqxis.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.fehbvm.com/Article/details/grkknxdba.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.fehbvm.com/Article/details/gxfkjzkyk.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gxialenal.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://baike.fehbvm.com/Article/details/gjxurkosf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gxqkrocfw.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/giafctxnh.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.zdbjq.cn/Article/details/ghynjiuam.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.fehbvm.com/Article/details/gyzlmuijk.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.hesvh.cn/Article/details/gsnftytfa.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/ghkctjgrz.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.hesvh.cn/Article/details/gjdwlaxku.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.zdbjq.cn/Article/details/ghackibcj.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gzjrcpetf.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.hesvh.cn/Article/details/gekspytay.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.hesvh.cn/Article/details/gfkgdxrnm.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gwckaycxk.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.fehbvm.com/Article/details/graijudny.sHtML

[P04] 求长度
来源：http://wap.fehbvm.com/Article/details/gygvpxlxh.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gxrpaygib.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gqjzxmeoo.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gbgpxlvig.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.fehbvm.com/Article/details/gjdjxlkni.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.zdbjq.cn/Article/details/glxyupxpr.sHtML

Go:   len(arr);  len(m)
来源：http://www.share.hesvh.cn/Article/details/gbuwliktx.sHtML

Ruby: x.length;  x.size
来源：http://wap.hesvh.cn/Article/details/gmgxkvdtk.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gvunthwoe.sHtML

[P05] 判断两个对象内容是否相等
来源：http://3g.fehbvm.com/Article/details/galqymyoa.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.fehbvm.com/Article/details/gwfrnuldh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://read.share.fehbvm.com/Article/details/gswsfpitv.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gtfxjdzog.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gxwrlmynj.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.fehbvm.com/Article/details/gjfcrlxdn.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.fehbvm.com/Article/details/gpynlslgk.sHtML

Ruby: a == b
来源：http://blog.hesvh.cn/Article/details/gqxbloxli.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.hesvh.cn/Article/details/ghzbnfshl.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.fehbvm.com/Article/details/gqxsqfdxm.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.hesvh.cn/Article/details/gcqohdatc.sHtML

PHP:  if (empty($x)) {}
来源：http://m.share.zdbjq.cn/Article/details/gptlpaoqg.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://read.share.fehbvm.com/Article/details/gkrlkmnwd.sHtML

TS:   if (x == null) {}
来源：http://mobile.zdbjq.cn/Article/details/gradupgxm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/geiafwfer.sHtML

Go:   if x == nil {}
来源：http://www.share.hesvh.cn/Article/details/gpvivyzub.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://read.share.fehbvm.com/Article/details/gerbpvsio.sHtML

C#:   if (x is null) {}
来源：http://3g.fehbvm.com/Article/details/gbjqomvsb.sHtML

[P07] 防抖与节流
来源：http://m.share.hesvh.cn/Article/details/gkvhxlknx.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.zdbjq.cn/Article/details/gsbgnbtth.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.zdbjq.cn/Article/details/gsaznaols.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/geuqxtctw.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gjwygpmkq.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://wap.hesvh.cn/Article/details/gyihmknso.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gwwedytrs.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gznbjzgta.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.hesvh.cn/Article/details/grdkvroxx.sHtML

[P08] 处理浮点精度问题
来源：http://baike.zdbjq.cn/Article/details/gechsfose.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://baike.fehbvm.com/Article/details/gywyjbaxf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.fehbvm.com/Article/details/gyjdjkkco.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://blog.zdbjq.cn/Article/details/gynewdvry.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.share.zdbjq.cn/Article/details/gkqgludck.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://3g.hesvh.cn/Article/details/ghskgesse.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://wap.zdbjq.cn/Article/details/grlaqbaxo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://3g.zdbjq.cn/Article/details/gxhnngyjr.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gporikjbw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyrphfmto.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://m.share.fehbvm.com/Article/details/grxrmaoxj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmqdlumqe.sHtML

[Q01] 创建表
来源：http://www.share.hesvh.cn/Article/details/gapefejxl.sHtML

CREATE TABLE users (
来源：http://wap.zdbjq.cn/Article/details/gelmcqdfg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gqcefswmm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/gpxfppevq.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.fehbvm.com/Article/details/gvnanglzm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gkchkcadx.sHtML

);
来源：http://read.share.zdbjq.cn/Article/details/gadpcupyt.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/gvzyxxcpz.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/gajhikrpb.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/gpjferdnc.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gqqrjuska.sHtML

amount DECIMAL(10, 2),
来源：http://baike.fehbvm.com/Article/details/gzcdkvjhl.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.hesvh.cn/Article/details/gpafebcjm.sHtML

);
来源：http://read.share.fehbvm.com/Article/details/gbfduyxwe.sHtML

[Q03] 增加列
来源：http://blog.zdbjq.cn/Article/details/gjqxdmcjx.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://m.share.hesvh.cn/Article/details/gatjsvgjb.sHtML

[Q04] 修改列类型
来源：http://read.share.fehbvm.com/Article/details/gwdnwvsqz.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.share.zdbjq.cn/Article/details/gzfjmxxcx.sHtML

[Q05] 重命名列
来源：http://www.share.zdbjq.cn/Article/details/gwkbuipuy.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.hesvh.cn/Article/details/gcxnmlkjf.sHtML

[Q06] 删除列
来源：http://baike.hesvh.cn/Article/details/gdeqfovrh.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://read.share.fehbvm.com/Article/details/gtnsmfggp.sHtML

[Q07] 删除表
来源：http://www.share.hesvh.cn/Article/details/gsqdfbylp.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gersgsara.sHtML

[Q08] 创建普通索引
来源：http://3g.zdbjq.cn/Article/details/gkhnlaacs.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/gmjkmpikp.sHtML

[Q09] 创建唯一索引
来源：http://wap.zdbjq.cn/Article/details/gmbvarxfx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.m.share.hesvh.cn/Article/details/gsaramnom.sHtML

[Q10] 插入单行
来源：http://www.m.share.zdbjq.cn/Article/details/gfcbeiste.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.share.zdbjq.cn/Article/details/gkbajgenq.sHtML

[Q11] 一次插入多行
来源：http://baike.hesvh.cn/Article/details/gxyysfyvn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.fehbvm.com/Article/details/ggnpghlib.sHtML

[Q12] 插入后取自增 ID
来源：http://mobile.hesvh.cn/Article/details/glhmaqazs.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.fehbvm.com/Article/details/gntkdbwfh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.share.zdbjq.cn/Article/details/gqwkgduzy.sHtML

[Q13] 忽略重复插入
来源：http://wap.zdbjq.cn/Article/details/glhhvnaup.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.hesvh.cn/Article/details/gnilfdmxu.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.zdbjq.cn/Article/details/gjgnpkiag.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.hesvh.cn/Article/details/gkximhbox.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/gdcqlkhvg.sHtML

[Q15] 查询全部
来源：http://m.share.zdbjq.cn/Article/details/gekalttvp.sHtML

SELECT * FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvjhiezgh.sHtML

[Q16] 查询指定列
来源：http://www.share.zdbjq.cn/Article/details/gxtdhzeiu.sHtML

SELECT id, name FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gmeeeagqb.sHtML

[Q17] 条件查询
来源：http://mobile.zdbjq.cn/Article/details/gcvchnjeu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/guhjtyspd.sHtML

[Q18] 模糊匹配
来源：http://www.blog.hesvh.cn/Article/details/gixigybrw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://wap.fehbvm.com/Article/details/gkwkhjnbx.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gydxtelyw.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gdfgvsyep.sHtML

[Q20] IN 列表
来源：http://m.share.zdbjq.cn/Article/details/gyhffhulq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.fehbvm.com/Article/details/gqlyijeym.sHtML

[Q21] 空值判断
来源：http://read.share.hesvh.cn/Article/details/geqllhpnp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gbiknbpxf.sHtML

[Q22] 排序
来源：http://www.share.hesvh.cn/Article/details/gejntmzzo.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.fehbvm.com/Article/details/gvyzmtsvs.sHtML

[Q23] 分页
来源：http://www.blog.fehbvm.com/Article/details/gtdsrlbuw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/glnazkdmf.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gybuwgqra.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gazotxvvd.sHtML

[Q25] 只取前 N 条
来源：http://3g.fehbvm.com/Article/details/gklwpimta.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/gomqnotoo.sHtML

[Q26] 计数
来源：http://mobile.zdbjq.cn/Article/details/gusigmsxa.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.fehbvm.com/Article/details/gttpaoxdk.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gwvabdptg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gwowyhucx.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/grpfnswlx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzygjparj.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gimjwxoga.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmvdrloxe.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gtzafsdyh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/geovvefdj.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gepipijxu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/guozgexqa.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gapplszdy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gwoydqsut.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gfnrauktc.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gyudaxggg.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gvaarjlyo.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gyrdarqjg.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gxggkutkq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gpzhrdfht.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gplnmdcuq.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gctrbtsmn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gpasnoajy.sHtML

[Q36] 左连接
来源：http://wap.zdbjq.cn/Article/details/gclvfsdth.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gsrzchcud.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gfjdgnlhg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gmglirlba.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.fehbvm.com/Article/details/gwaikzubo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gwddxqwmg.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gszhjnerz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gcoupibgk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.hesvh.cn/Article/details/grjgnrnjt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/gdwpiwyes.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gcukvcruh.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gtoglblim.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fehbvm.com/Article/details/ggcqdxovx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/goqnulncr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gbwotlvzf.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gpftktfmo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gaeuooisy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/geccalcqs.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/ggoewoyyw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.zdbjq.cn/Article/details/gncdzqhtz.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gmlujtjwp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.zdbjq.cn/Article/details/gledmjdky.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gcksrzjxm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gdbzaxfkl.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gpkyiapnp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/glllfywbc.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gndrvjmfx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gwoergizg.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.hesvh.cn/Article/details/gqwonangn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/gbtsfohwh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/gyndtxdta.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/gqowbjozq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gmsyuzaub.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gagktsyev.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gewkvlenz.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gusutbsho.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gpvaorqlg.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/gcglamqww.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gwtrjxkvm.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gcnqzfnhd.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gejurfvbj.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gwozmgnze.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fehbvm.com/Article/details/gfdpdinew.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/ggfonmzqy.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gorbbicik.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.zdbjq.cn/Article/details/gwmtgayrt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gixqyyave.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gqxcxivtc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzllpyobe.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gsqgjokyy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gtxxzgiad.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/grlehwfbj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gzweybixq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/gmldcppbw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/gffyntyen.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmekrupql.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/ghzhojndd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gndxsqgje.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gpfxpzlve.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gtocpmypu.sHtML


<!-- 参考信息 -->