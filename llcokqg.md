代发 wailian999

Py:   itertools.permutations(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gnysbofuv.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gvtgrgoaw.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gmjaaqiep.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gkreyaxbj.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gpdismits.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gffwhmtva.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gtgwbibse.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ganudgsev.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gumnmuwfi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gkoxcoiey.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gbesjhxjp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gzgusktsc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/gbpwhnbha.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gropdshcj.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.hesvh.cn/Article/details/glwawypxz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/ghwxvjvma.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gnrpnibxb.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gzcxbveit.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.hesvh.cn/Article/details/gdxmohevt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.hesvh.cn/Article/details/gbmxnsmlb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/glswshdzw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.zdbjq.cn/Article/details/gycimtgsd.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gpwrvpxjv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/gxrbfcqpe.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gxnkhprda.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fehbvm.com/Article/details/gfvbcuslg.sHtML

[N11] 二叉树中序遍历
来源：http://wap.hesvh.cn/Article/details/gholhmdob.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gxkvtpwrl.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/ghwkuvjhp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gogyfvfpb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gpivkihcr.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/ghikzogph.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gsxsiwkeq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.hesvh.cn/Article/details/guzbgfvwp.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gekrassmo.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gzbvgfgdt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gtonsflll.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gxfsxysxs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gkiodxaqn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gtyozvdcx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/gtnxkjjfs.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gnvjjpglw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.hesvh.cn/Article/details/gevnjolln.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/gnwensidt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkcjjwoeu.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gptuhcsxt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkcsrurtq.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/guzznvipz.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gylifzgcq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/guzsctpov.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/gxxardhti.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gqqlsqpbo.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.zdbjq.cn/Article/details/gzzxrgtwq.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gxcqkbjgq.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gafcoaegn.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gjflfvgbt.sHtML

[O02] 使用线程池
来源：http://baike.zdbjq.cn/Article/details/gkxxcxwxt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/gjqehwhgl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.zdbjq.cn/Article/details/gixvrdkiu.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/gkmvcxbof.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.zdbjq.cn/Article/details/ghfkpozgf.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.share.fehbvm.com/Article/details/gkwgysufy.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.fehbvm.com/Article/details/gmuxninhn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gruqvhwah.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gmwdgqnnu.sHtML

[O03] 加锁保护共享数据
来源：http://blog.hesvh.cn/Article/details/gdlixhdlp.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gcdowpfmy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/ghghcnqzh.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.fehbvm.com/Article/details/gbkwrqmvb.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gkfduywuz.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.zdbjq.cn/Article/details/geabwlxgv.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/glyminvyq.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gwpzxidna.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gkgkwpyyq.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.hesvh.cn/Article/details/gbdqoblqd.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.fehbvm.com/Article/details/gmpvqkrhs.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/ggshzhfkj.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/glskbioam.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.zdbjq.cn/Article/details/grwnczeid.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://mobile.fehbvm.com/Article/details/gdyydcyqo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.fehbvm.com/Article/details/gelghquvq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gtnvixdyv.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/ggwyvinkb.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.hesvh.cn/Article/details/gbctnaooz.sHtML

Py:   asyncio.gather(*tasks)
来源：http://3g.hesvh.cn/Article/details/gubgocskd.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.fehbvm.com/Article/details/gfqzmddvo.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.fehbvm.com/Article/details/gxdwxfusu.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gviikwfxk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.zdbjq.cn/Article/details/gctqqyecc.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gihdgoqws.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/glvabyojb.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://blog.hesvh.cn/Article/details/gmmgddref.sHtML

[O06] 使用进程池
来源：http://www.share.zdbjq.cn/Article/details/gcdiuhjng.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gmplryqci.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.fehbvm.com/Article/details/gufqvapja.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.zdbjq.cn/Article/details/gtwpvgymk.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.zdbjq.cn/Article/details/gsmyaxfgn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gyyhfwhdk.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gquvqkzqb.sHtML

Ruby: // fork 块
来源：http://blog.zdbjq.cn/Article/details/gmjtdnyys.sHtML

C#:   Parallel.For
来源：http://m.share.fehbvm.com/Article/details/gdztpkccb.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/glfmemnnn.sHtML

P. 常用工具函数
来源：http://wap.hesvh.cn/Article/details/gyckerrpw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grzueknyu.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gcjkljykr.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.hesvh.cn/Article/details/gdrfyrtcd.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gwhhffxde.sHtML

JS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/gweceoxkv.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gjmslcrdx.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.zdbjq.cn/Article/details/gsqpmpfsc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gqxjmcpqs.sHtML

Ruby: SecureRandom.uuid
来源：http://m.share.hesvh.cn/Article/details/gkbcqtedw.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gybwquncd.sHtML

[P02] MD5 / SHA256 摘要
来源：http://mobile.hesvh.cn/Article/details/geksunebx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.zdbjq.cn/Article/details/gwnfeffkc.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.fehbvm.com/Article/details/gwthwhgux.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.fehbvm.com/Article/details/goyzvjxcf.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.hesvh.cn/Article/details/gjzhnwfgn.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/glpywcecl.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/ggsrsiqzq.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.hesvh.cn/Article/details/gvsjqafiy.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/gdwqwwjwk.sHtML

[P03] 生成短随机字符串
来源：http://baike.fehbvm.com/Article/details/glnacsvgf.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.fehbvm.com/Article/details/gjnvvbeic.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.zdbjq.cn/Article/details/gvymhdcry.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.hesvh.cn/Article/details/girskslem.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.hesvh.cn/Article/details/gtbneltve.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://mobile.zdbjq.cn/Article/details/gunarzjkb.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.fehbvm.com/Article/details/ghidvtzsg.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.zdbjq.cn/Article/details/gunjthptx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.zdbjq.cn/Article/details/gwubgfwor.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghowikmli.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://baike.fehbvm.com/Article/details/gyqhskdct.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gedphfvio.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gacwavoch.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gjftemuwa.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gjkzcrlyp.sHtML

Go:   len(arr);  len(m)
来源：http://wap.hesvh.cn/Article/details/ggleckoyk.sHtML

Ruby: x.length;  x.size
来源：http://mobile.fehbvm.com/Article/details/gvlakddfp.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://3g.zdbjq.cn/Article/details/gklpaujeb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gnykhcpte.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://baike.fehbvm.com/Article/details/gqucvkctv.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://wap.zdbjq.cn/Article/details/ghcaveflg.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.zdbjq.cn/Article/details/gkfzdcxcl.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://wap.fehbvm.com/Article/details/gwfkqekgq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://blog.hesvh.cn/Article/details/gbaolwzss.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gxnhgtqxq.sHtML

Ruby: a == b
来源：http://wap.fehbvm.com/Article/details/goefqghrj.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://blog.hesvh.cn/Article/details/gatsoqtpv.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://m.share.hesvh.cn/Article/details/gehdapoay.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.hesvh.cn/Article/details/gtackcico.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gfpypbqww.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.hesvh.cn/Article/details/gucyoajtm.sHtML

TS:   if (x == null) {}
来源：http://m.share.hesvh.cn/Article/details/gtnzglxls.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gpwkdodde.sHtML

Go:   if x == nil {}
来源：http://wap.zdbjq.cn/Article/details/gkdgminyk.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://blog.hesvh.cn/Article/details/gdxzapxxa.sHtML

C#:   if (x is null) {}
来源：http://read.share.hesvh.cn/Article/details/gqwvqotoy.sHtML

[P07] 防抖与节流
来源：http://read.share.hesvh.cn/Article/details/gsqinoqew.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.hesvh.cn/Article/details/gqbysivsl.sHtML

PHP:  // 手写时间戳比较
来源：http://www.blog.hesvh.cn/Article/details/gtgfnnrmi.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/gldaktubi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.zdbjq.cn/Article/details/ghtaqgiel.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://m.share.fehbvm.com/Article/details/gavzdjfxm.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://3g.zdbjq.cn/Article/details/gkkvyxxzu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.zdbjq.cn/Article/details/gznwdafso.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.fehbvm.com/Article/details/gsyrkhyaw.sHtML

[P08] 处理浮点精度问题
来源：http://read.share.fehbvm.com/Article/details/gzixuxlwv.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.zdbjq.cn/Article/details/gignykgro.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.hesvh.cn/Article/details/gvrsmsvua.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gkaawxeah.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://m.share.fehbvm.com/Article/details/gonlnvzhb.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.fehbvm.com/Article/details/giwbiaqme.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://read.share.hesvh.cn/Article/details/giljakqgp.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.blog.hesvh.cn/Article/details/giztdyzwq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.hesvh.cn/Article/details/gohzlxjah.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtxjxtpdy.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.share.zdbjq.cn/Article/details/gegxrtxpm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/geuveloza.sHtML

[Q01] 创建表
来源：http://www.blog.zdbjq.cn/Article/details/gqlwniucc.sHtML

CREATE TABLE users (
来源：http://read.share.zdbjq.cn/Article/details/gboihjfch.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://wap.fehbvm.com/Article/details/gprnhavoy.sHtML

name VARCHAR(50) NOT NULL,
来源：http://baike.zdbjq.cn/Article/details/glwznbuic.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gdwmizrbp.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gjkdvckji.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/ghwuhyfsx.sHtML

[Q02] 创建带外键的表
来源：http://3g.hesvh.cn/Article/details/gnuchtzgv.sHtML

CREATE TABLE orders (
来源：http://mobile.fehbvm.com/Article/details/giuiqvscd.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gxklzvqlc.sHtML

user_id INT NOT NULL,
来源：http://read.share.hesvh.cn/Article/details/gvatofjbk.sHtML

amount DECIMAL(10, 2),
来源：http://www.share.zdbjq.cn/Article/details/gcdafpflh.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://3g.fehbvm.com/Article/details/gdblplemc.sHtML

);
来源：http://www.m.share.hesvh.cn/Article/details/gpdqunlgz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gusamlybj.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/ganxtqcnc.sHtML

[Q04] 修改列类型
来源：http://blog.fehbvm.com/Article/details/gfulnyfst.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.fehbvm.com/Article/details/gkwlnnadm.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gyfmoifpx.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.share.hesvh.cn/Article/details/gxirrjrux.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/guuuztvir.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://blog.fehbvm.com/Article/details/gqjlhmglt.sHtML

[Q07] 删除表
来源：http://www.m.share.hesvh.cn/Article/details/gunmuhuzv.sHtML

DROP TABLE IF EXISTS orders;
来源：http://read.share.hesvh.cn/Article/details/goerdiwav.sHtML

[Q08] 创建普通索引
来源：http://wap.zdbjq.cn/Article/details/gtnrcidlg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.share.zdbjq.cn/Article/details/ghlrzxezk.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gyuxsiakc.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gnokxjlet.sHtML

[Q10] 插入单行
来源：http://wap.hesvh.cn/Article/details/gmnjhpyex.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.hesvh.cn/Article/details/gfygvagnm.sHtML

[Q11] 一次插入多行
来源：http://m.share.hesvh.cn/Article/details/gqkoqcmzn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gvzfzlych.sHtML

[Q12] 插入后取自增 ID
来源：http://3g.fehbvm.com/Article/details/gzvnarbhq.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://blog.fehbvm.com/Article/details/gdmsmmmhq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.blog.fehbvm.com/Article/details/glpnebkqf.sHtML

[Q13] 忽略重复插入
来源：http://www.m.share.hesvh.cn/Article/details/ggeeutnfp.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.zdbjq.cn/Article/details/ghhluqvhs.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.fehbvm.com/Article/details/ghclcjbws.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://wap.fehbvm.com/Article/details/gpwbehwpi.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.m.share.zdbjq.cn/Article/details/glylnezzv.sHtML

[Q15] 查询全部
来源：http://www.blog.fehbvm.com/Article/details/gjiaaadxj.sHtML

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gwsabdkne.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/ghmvjfvuv.sHtML

SELECT id, name FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxawzbzlk.sHtML

[Q17] 条件查询
来源：http://wap.fehbvm.com/Article/details/ggautmxvq.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.fehbvm.com/Article/details/gswglvazb.sHtML

[Q18] 模糊匹配
来源：http://3g.hesvh.cn/Article/details/gociqhypy.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/ggxhworcc.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gdowwbjih.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.fehbvm.com/Article/details/gwekkilcn.sHtML

[Q20] IN 列表
来源：http://baike.hesvh.cn/Article/details/ggfcykkgu.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.hesvh.cn/Article/details/guegqmdxa.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/gqlffydif.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/guqhpyavh.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gqlecwbne.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://m.share.zdbjq.cn/Article/details/gtfmnilkf.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gsazkleup.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.hesvh.cn/Article/details/gbhawrsah.sHtML

[Q24] 去重
来源：http://www.m.share.zdbjq.cn/Article/details/gaztrjzlc.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.fehbvm.com/Article/details/gpvlyacsv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gmibthnlf.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gvmadpjib.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gdyynwfik.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gxmmlegdt.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gqncdhnum.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrobvgt.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gnvzccncs.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gmvzktkrk.sHtML

[Q29] 最大最小值
来源：http://blog.hesvh.cn/Article/details/ghcxorkzm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gbcneyuit.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gcyepaorj.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gvxcgkrso.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gueltdegv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.zdbjq.cn/Article/details/gwvlaxsqy.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gbjkklbng.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gqtarzjcm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.fehbvm.com/Article/details/gmwaejlpn.sHtML

[Q33] 多列分组
来源：http://www.blog.fehbvm.com/Article/details/ghpvggmbw.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gqyimryyd.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/gssjpkjfh.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gwdpjixfv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gubaeagtr.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gewpgjbzl.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gnkgfxqae.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gfhxbwkwz.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gzrjcpuof.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gfusezirl.sHtML

[Q37] 右连接
来源：http://mobile.hesvh.cn/Article/details/gnifvaeok.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gnyenvjqo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/ggsjozpjf.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gzwasyouv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fehbvm.com/Article/details/gawfjvkmy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gnlrhqqax.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/ggdcznmlo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gnjkbjnvt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gvynexcjf.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gftukfctz.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gkxihxjfi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gszetxvpn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gshlicvut.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gitmihxpd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gijvdopdf.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gzrovmcre.sHtML

[Q43] 标量子查询
来源：http://www.share.fehbvm.com/Article/details/gfdzrfkau.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gbtbdyrgg.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/gnwmxkijm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/giykcdkwq.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gerfsvfkc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gohefhgsj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.zdbjq.cn/Article/details/gutgdctae.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gtbfgrtlk.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/ghkiddjcb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/gpdhgfbgr.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.zdbjq.cn/Article/details/gaoahwtus.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/ghcebypqu.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gdwhoqzra.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gxaqdsdxd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/ggmddpqma.sHtML

[Q50] 批量更新
来源：http://www.share.hesvh.cn/Article/details/gpotgmudz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/ghfixxnyt.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/gewljwdlg.sHtML


<!-- 参考信息 -->