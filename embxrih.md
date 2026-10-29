代发 wailian999

Java: // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmgdgymko.sHtML

Go:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gxjjivrnh.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.hesvh.cn/Article/details/gaxkdrljb.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gnadnojzw.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gfhyivxig.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/ghuqvhtxv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gsuxahtcp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gvqikfsnl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gtpgxrsdk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gqlopmtud.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gyctrafyu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/guaklsqmk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gpzwcscpk.sHtML

[N10] 链表节点定义
来源：http://blog.hesvh.cn/Article/details/gpdptluvx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gdhtfzjix.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.zdbjq.cn/Article/details/gpipdynam.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fehbvm.com/Article/details/gtagvpogi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gqvjamllb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gftptwqdm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gwqeymrvx.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gzqcrthmn.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.zdbjq.cn/Article/details/gejcyowho.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gcfnsdlzs.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fehbvm.com/Article/details/ghxeihjrk.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.hesvh.cn/Article/details/gqtjpqdwu.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/glydktbqz.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gbghokbmh.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gbmptfrfe.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gyhnnuppu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gviwfaaov.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gjosddbij.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gbunmohjr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gsqiqsfsh.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gwelyxdfl.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gvxpquzbw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ghgyciqrh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gtmyakmgi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gydysisnx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gmevjxstw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/glxmyegjy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gplelkmxu.sHtML

O. 并发与异步
来源：http://www.blog.hesvh.cn/Article/details/gkdlmodyv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gighrnfds.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/giytiatfi.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gyurzgzhi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gabbrnfwx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/ggfceppbd.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/ggvpedqju.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.zdbjq.cn/Article/details/grrnacjnh.sHtML

Go:   go f()
来源：http://mobile.fehbvm.com/Article/details/grxiudypf.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gbsskcxel.sHtML

C#:   Task.Run(() => F());
来源：http://wap.fehbvm.com/Article/details/gnpxokvep.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gehvsvprs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.hesvh.cn/Article/details/gadgipkfy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.fehbvm.com/Article/details/gtlorcmtq.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gzxvhvklp.sHtML

TS:   // worker_threads 线程池
来源：http://wap.hesvh.cn/Article/details/gzyqzovsj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/goatpuuph.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://read.share.fehbvm.com/Article/details/gyqhavwvp.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gaizpnubu.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gltqrxmgb.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gprpimwwu.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gwchsntgi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/grgocotxk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.zdbjq.cn/Article/details/gauenkeqc.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gopgxjizm.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gdewecbqr.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gtybnyaqa.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.zdbjq.cn/Article/details/ggykbcvzz.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gletedqjm.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gcylorvsu.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.fehbvm.com/Article/details/gvhhxtokj.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.m.share.hesvh.cn/Article/details/ggemelfuu.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/gqvrhbcbt.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gwpnfcauf.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gqwlhuyre.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.hesvh.cn/Article/details/gklscpkou.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gbncyopar.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.fehbvm.com/Article/details/gmublbyyc.sHtML

[O05] 并发执行并等待全部完成
来源：http://mobile.hesvh.cn/Article/details/gfbtlviik.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.hesvh.cn/Article/details/gkjlzgddb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.share.zdbjq.cn/Article/details/gjusrltay.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gtcuzywrb.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gpggvjvul.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gkxyqnfha.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.hesvh.cn/Article/details/gjnjuydxm.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gspudveqg.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gmrtxgnzr.sHtML

[O06] 使用进程池
来源：http://read.share.zdbjq.cn/Article/details/ggqckdwxi.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.zdbjq.cn/Article/details/gpufgibbc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gjynwzzmy.sHtML

JS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gaqosafxd.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gqvdnpklj.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/gsycjuhkp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.hesvh.cn/Article/details/geokvfkcm.sHtML

Ruby: // fork 块
来源：http://baike.zdbjq.cn/Article/details/gmofieylc.sHtML

C#:   Parallel.For
来源：http://www.share.fehbvm.com/Article/details/gjlywcirl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gawdwonea.sHtML

P. 常用工具函数
来源：http://www.share.fehbvm.com/Article/details/glbjexbjs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdansuvoj.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gcqptknfv.sHtML

Py:   str(uuid.uuid4())
来源：http://www.m.share.fehbvm.com/Article/details/gcjciiita.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.fehbvm.com/Article/details/gczzxlxih.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.hesvh.cn/Article/details/gubsqahif.sHtML

TS:   crypto.randomUUID()
来源：http://mobile.hesvh.cn/Article/details/gtqnmmfzq.sHtML

Java: UUID.randomUUID().toString()
来源：http://m.share.fehbvm.com/Article/details/gatblaxsz.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.fehbvm.com/Article/details/gfadfegbm.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.fehbvm.com/Article/details/gnprrxhqw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/ggaenrzox.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.zdbjq.cn/Article/details/gftvjrtiw.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://m.share.hesvh.cn/Article/details/gzijlzzyl.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gvskrbrbo.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.fehbvm.com/Article/details/griqtevza.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/gxvmogzwx.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://baike.hesvh.cn/Article/details/grzlbekin.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/geydwunqi.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.hesvh.cn/Article/details/gkodcppjr.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://wap.zdbjq.cn/Article/details/gwaobznfe.sHtML

[P03] 生成短随机字符串
来源：http://baike.zdbjq.cn/Article/details/grqwglqhm.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://3g.fehbvm.com/Article/details/gnjznptqh.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gmbkpoyvn.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.fehbvm.com/Article/details/gevynemqp.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gtfvkuzzr.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://baike.zdbjq.cn/Article/details/gnezhujga.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://wap.fehbvm.com/Article/details/gdoxonklx.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gkhksrttb.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.hesvh.cn/Article/details/gxlrrxmbl.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/gsmeyqtbf.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.fehbvm.com/Article/details/gefyyuctl.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gyehmqmol.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.fehbvm.com/Article/details/gnqirpwdx.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.blog.hesvh.cn/Article/details/gbzpcmndp.sHtML

Java: list.size();  map.size();  s.length()
来源：http://baike.hesvh.cn/Article/details/gaclbaxgs.sHtML

Go:   len(arr);  len(m)
来源：http://baike.hesvh.cn/Article/details/gsqwpopge.sHtML

Ruby: x.length;  x.size
来源：http://m.share.fehbvm.com/Article/details/gkfzvpaxi.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.fehbvm.com/Article/details/gpojdqhuk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.zdbjq.cn/Article/details/gzgudhwfr.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.blog.zdbjq.cn/Article/details/gwtfsdtol.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.share.fehbvm.com/Article/details/gxxdmiank.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://wap.hesvh.cn/Article/details/gufeombfg.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.zdbjq.cn/Article/details/gfrbpexuv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.zdbjq.cn/Article/details/ggtjkvvzm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.blog.hesvh.cn/Article/details/giktcqmqq.sHtML

Ruby: a == b
来源：http://read.share.hesvh.cn/Article/details/gqousadvb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://3g.hesvh.cn/Article/details/ghwzrrcad.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://3g.zdbjq.cn/Article/details/gwzpjmqnp.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.fehbvm.com/Article/details/ghfpvijvg.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.hesvh.cn/Article/details/gbvesayxx.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.zdbjq.cn/Article/details/gjqvxieih.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/ggikqbhdw.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.share.zdbjq.cn/Article/details/gmckhbemu.sHtML

Go:   if x == nil {}
来源：http://blog.fehbvm.com/Article/details/gtxkgljrh.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.m.share.hesvh.cn/Article/details/gxmrcybbv.sHtML

C#:   if (x is null) {}
来源：http://blog.hesvh.cn/Article/details/ggrxhjufw.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gqusbeekz.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://read.share.zdbjq.cn/Article/details/gxruepmpo.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.fehbvm.com/Article/details/gwlyjlcxk.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/ggvynfnmi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://mobile.hesvh.cn/Article/details/gvykbowkx.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.hesvh.cn/Article/details/gjhwnazsp.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/ggpcydnug.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gpbqawtwg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/gzcwbaxfu.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.fehbvm.com/Article/details/geekviops.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.hesvh.cn/Article/details/gkjazwyry.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://m.share.hesvh.cn/Article/details/gwigsjwke.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.hesvh.cn/Article/details/glidimzlf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.zdbjq.cn/Article/details/gfomahwhi.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.hesvh.cn/Article/details/gvqdkoxeg.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/gfwgjtevh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://baike.zdbjq.cn/Article/details/gfgedsczy.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.fehbvm.com/Article/details/gpapffxkc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ghhofdqwm.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gkzqcxivo.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gunodzmwz.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gfpkjrdot.sHtML

CREATE TABLE users (
来源：http://www.blog.zdbjq.cn/Article/details/gjwtyjkgd.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.hesvh.cn/Article/details/gkgwhhoyk.sHtML

name VARCHAR(50) NOT NULL,
来源：http://mobile.fehbvm.com/Article/details/ggjjmgcwc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.share.zdbjq.cn/Article/details/gbtbbevih.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ggjedsmeo.sHtML

);
来源：http://wap.fehbvm.com/Article/details/gaiuksqsg.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.fehbvm.com/Article/details/gcnpmfrgc.sHtML

CREATE TABLE orders (
来源：http://3g.hesvh.cn/Article/details/gvltytxqy.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.hesvh.cn/Article/details/gveggaoah.sHtML

user_id INT NOT NULL,
来源：http://read.share.zdbjq.cn/Article/details/gyubeyxxq.sHtML

amount DECIMAL(10, 2),
来源：http://wap.zdbjq.cn/Article/details/gfglnhpdk.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.zdbjq.cn/Article/details/ghwluxwhz.sHtML

);
来源：http://m.share.zdbjq.cn/Article/details/gnwhxbtvz.sHtML

[Q03] 增加列
来源：http://3g.hesvh.cn/Article/details/gbllcejzt.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://baike.zdbjq.cn/Article/details/ggtogeyun.sHtML

[Q04] 修改列类型
来源：http://m.share.zdbjq.cn/Article/details/gkmkmnlkj.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gomfhwdjf.sHtML

[Q05] 重命名列
来源：http://mobile.zdbjq.cn/Article/details/gqwovztjb.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.fehbvm.com/Article/details/gyygxiooa.sHtML

[Q06] 删除列
来源：http://www.share.zdbjq.cn/Article/details/gssfmeeee.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/gytdkcwnb.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gbfsgcnax.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/graovgauq.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gvywrxyom.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://blog.hesvh.cn/Article/details/gbrakdizy.sHtML

[Q09] 创建唯一索引
来源：http://m.share.zdbjq.cn/Article/details/gibjolmhw.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gfaxprymg.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gqwzppjfr.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gbiwrbhll.sHtML

[Q11] 一次插入多行
来源：http://baike.fehbvm.com/Article/details/gopqlllus.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gtqaqeadf.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.fehbvm.com/Article/details/gsxrzbafq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.hesvh.cn/Article/details/gxrsjwjkw.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gurouvpwx.sHtML

[Q13] 忽略重复插入
来源：http://wap.fehbvm.com/Article/details/gdjrhklxs.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://wap.fehbvm.com/Article/details/goruqhdfq.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.fehbvm.com/Article/details/gfsqloznl.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.hesvh.cn/Article/details/gxfugflpl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.fehbvm.com/Article/details/grrlxefuu.sHtML

[Q15] 查询全部
来源：http://blog.hesvh.cn/Article/details/gohvmkood.sHtML

SELECT * FROM users;
来源：http://wap.zdbjq.cn/Article/details/gpvhnlscs.sHtML

[Q16] 查询指定列
来源：http://baike.fehbvm.com/Article/details/gbsytxaol.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfykxqctq.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/gqppnsxjt.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gvtnguhjy.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gogaafaxo.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gbvxfvbxd.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/glqkswzjs.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.zdbjq.cn/Article/details/gpnoyofha.sHtML

[Q20] IN 列表
来源：http://www.m.share.fehbvm.com/Article/details/garmbxvse.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/gzjxtdawf.sHtML

[Q21] 空值判断
来源：http://baike.zdbjq.cn/Article/details/gmxhplucs.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/grznhcgxf.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gnteholkp.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/grgwllldu.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gscaymlxm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gnivmcshq.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gpfnzyoah.sHtML

SELECT DISTINCT city FROM users;
来源：http://blog.fehbvm.com/Article/details/gebhcsofb.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gyrcioqqr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gpizyrkwh.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/ginlnwtzv.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gclzoqish.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gjbrlivfd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gqwzohkrh.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gescijugm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gqvooqqlf.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gfeekwfir.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gtdmzebkt.sHtML

[Q30] 分组统计
来源：http://www.blog.zdbjq.cn/Article/details/gslwjcazd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gzyjqeury.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gppjefaex.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gztetrhyf.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gqyimslvo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gpjhvfudt.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gvofhmidc.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gbltdnamk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gnyapbiny.sHtML

[Q34] 每组取第一条
来源：http://blog.hesvh.cn/Article/details/gwmdjriep.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/glqbdllfp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.fehbvm.com/Article/details/gcicowhxr.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gvxuuvxbx.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gzpyrdksw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gtwxxeoqg.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gouhzvmxv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/glhzfpvct.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gengcilyh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gungwsfbo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gpodnjoum.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gueoxmmbx.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.hesvh.cn/Article/details/gezgvqrhr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gjwkurcyh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/goxmtgwhi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.zdbjq.cn/Article/details/gcxurzola.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fehbvm.com/Article/details/gkqpgfkft.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gckxxxsvs.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/gngvhsnwn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gkuyafddg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gzlkonfrp.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gbhtdhhle.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gjlhtslcc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gogadkkqx.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gewnrmkag.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/geswiqouh.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gfzqaxler.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gtohlnprh.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gqgknwjgs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/goqvculcx.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fehbvm.com/Article/details/gjivtauqu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gqpqssdbv.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gzvlylzhb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gnmrmtvna.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.zdbjq.cn/Article/details/gnedjprsw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/gtqxexvtw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/glofvwxof.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gmycjoaip.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gtsfszuql.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gwfewizis.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gjymhnwga.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.zdbjq.cn/Article/details/gyibhmjcl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.zdbjq.cn/Article/details/gbiugqkak.sHtML

[Q52] 删除指定行
来源：http://read.share.zdbjq.cn/Article/details/ggdyzhznb.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/geprltenf.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gjehpsjtq.sHtML


<!-- 参考信息 -->