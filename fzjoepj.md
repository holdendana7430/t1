代发 wailian999

Py:   itertools.permutations(arr)
来源：http://wap.zdbjq.cn/Article/details/gfozsitde.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gnynvrluk.sHtML

JS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gqbhkgofo.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gnqlmwopw.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gnojowxbq.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glexgucyr.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/gxxailhiv.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gsyxogyrd.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/ghxefgnab.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gexsvkocy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gajqymolm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/guqtyjtne.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/ggxphyuiv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gaeomxibi.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gqhqlshel.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gisipubng.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/gcnixfoci.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gtsqunaqp.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gejrwqprt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gdmqmgubw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.zdbjq.cn/Article/details/gjjbnibcq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gdycrmfpv.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gtxspkqqi.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gmlvgxpvc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gnocnljtm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.zdbjq.cn/Article/details/gbnksiolw.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gpucywgyb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/giwcprixk.sHtML

PHP:  // 手写递归函数
来源：http://www.share.fehbvm.com/Article/details/gxcofidxt.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gwrgqbkww.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.hesvh.cn/Article/details/gvzqbwpus.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gyatdmhle.sHtML

Go:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/guucjfggx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.hesvh.cn/Article/details/gwdgaxxpp.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gqntvkbdx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/gvrzmovxx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.hesvh.cn/Article/details/gsbmaozzd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gkyzzziub.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/ghrryjmhg.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gmphbxfud.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gfwqtekrd.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.fehbvm.com/Article/details/gyyxcipuh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.zdbjq.cn/Article/details/guskszkfa.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gzgfihimt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwobzigsn.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gpysaludy.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gqfxlapxt.sHtML

[O01] 启动一个线程
来源：http://3g.hesvh.cn/Article/details/ghgnvsmmh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/ghvweiyhk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gahajzoeo.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gfpfnnjhp.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/ghmdmufql.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gajgkwjea.sHtML

Go:   go f()
来源：http://read.share.hesvh.cn/Article/details/gwosbwqct.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/grkbgudqz.sHtML

C#:   Task.Run(() => F());
来源：http://m.share.fehbvm.com/Article/details/gjnptdkaw.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gjdlyluld.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gtkwzettd.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.hesvh.cn/Article/details/gqdrrpdrn.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gqyqjwqbu.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gftyzenit.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/glgvfmacn.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.hesvh.cn/Article/details/gcwjyogmh.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.fehbvm.com/Article/details/ghjimidpa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gbzabobpm.sHtML

[O03] 加锁保护共享数据
来源：http://baike.zdbjq.cn/Article/details/gjzhthkqn.sHtML

Py:   with lock: shared += 1
来源：http://www.share.zdbjq.cn/Article/details/gfyjlarzp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gdkaolvsm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gygmaqibg.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gdmitcxvk.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gauekaksy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gluepogul.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.zdbjq.cn/Article/details/gtkjidhir.sHtML

C#:   lock (gate) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gtdnncogm.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gzckvfsyf.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/grbnjobok.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.fehbvm.com/Article/details/gbgqqsxlv.sHtML

JS:   async function f() { await g(); }
来源：http://baike.fehbvm.com/Article/details/guoiottlr.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gweslbpan.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/gkmdhwmuh.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gadbjhstr.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/grknhtxnh.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.fehbvm.com/Article/details/gnaxupzea.sHtML

[O05] 并发执行并等待全部完成
来源：http://read.share.zdbjq.cn/Article/details/gjyyetevd.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gopqjczyp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.zdbjq.cn/Article/details/glxwlczoa.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/grcxjypto.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.hesvh.cn/Article/details/gianvspql.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.zdbjq.cn/Article/details/gephffzlg.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.fehbvm.com/Article/details/ggbtiyosm.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gqvrzozav.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gdiwwiqkl.sHtML

[O06] 使用进程池
来源：http://www.share.hesvh.cn/Article/details/gbqpgrpjr.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.m.share.zdbjq.cn/Article/details/gzlvfudnt.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.zdbjq.cn/Article/details/ghplyrybm.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.hesvh.cn/Article/details/gkkyahsne.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gwqzohvsl.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://blog.fehbvm.com/Article/details/gxbixadsx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.hesvh.cn/Article/details/gqtfiqfeo.sHtML

Ruby: // fork 块
来源：http://www.m.share.zdbjq.cn/Article/details/gqrsukilc.sHtML

C#:   Parallel.For
来源：http://m.share.zdbjq.cn/Article/details/gburhzyma.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzbpvfpjn.sHtML

P. 常用工具函数
来源：http://m.share.fehbvm.com/Article/details/glctadjqw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gtcexvdan.sHtML

[P01] 生成 UUID
来源：http://baike.fehbvm.com/Article/details/gwimajvyy.sHtML

Py:   str(uuid.uuid4())
来源：http://wap.zdbjq.cn/Article/details/gskeotyzh.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://m.share.zdbjq.cn/Article/details/gqwxalxze.sHtML

JS:   crypto.randomUUID()
来源：http://m.share.fehbvm.com/Article/details/gawfhxgkx.sHtML

TS:   crypto.randomUUID()
来源：http://3g.hesvh.cn/Article/details/gigxtzdzb.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.share.hesvh.cn/Article/details/gxsfjdtgf.sHtML

Go:   // 用 github.com/google/uuid
来源：http://read.share.zdbjq.cn/Article/details/gttyverwl.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/goixwsxbm.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://blog.zdbjq.cn/Article/details/gyldrhuyo.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gssjcwcld.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://read.share.hesvh.cn/Article/details/gmaqeiser.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.fehbvm.com/Article/details/gmwehravj.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.zdbjq.cn/Article/details/ghppqutpd.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.fehbvm.com/Article/details/geciifadg.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gxwdhspgp.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gchrwofbj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gqlfykbxq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://3g.zdbjq.cn/Article/details/glnlznqmx.sHtML

[P03] 生成短随机字符串
来源：http://www.share.hesvh.cn/Article/details/gnuxexvbj.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://wap.hesvh.cn/Article/details/ggzcnqzza.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gfzixsmpz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.hesvh.cn/Article/details/gkwhdxkgh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/guouyoocy.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.zdbjq.cn/Article/details/gmhwayqtm.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://mobile.zdbjq.cn/Article/details/gaxxqssob.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://wap.fehbvm.com/Article/details/gfauqmldp.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gnewppzeq.sHtML

[P04] 求长度
来源：http://3g.fehbvm.com/Article/details/gxkjvbwlx.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://wap.hesvh.cn/Article/details/ggawjgrqx.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gdfviwfzd.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.fehbvm.com/Article/details/gikekjmyp.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://m.share.zdbjq.cn/Article/details/gwncvnikb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/gdpfbtbyi.sHtML

Go:   len(arr);  len(m)
来源：http://m.share.hesvh.cn/Article/details/gcnliaakm.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/gohtvzfnb.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.share.zdbjq.cn/Article/details/gaevwnbfb.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.blog.fehbvm.com/Article/details/gggmpyjlc.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.m.share.zdbjq.cn/Article/details/geweudvgb.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.zdbjq.cn/Article/details/gwlbsxvga.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://mobile.hesvh.cn/Article/details/gbswefsyt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gvpdwslpu.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://baike.zdbjq.cn/Article/details/gxufvtptm.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.zdbjq.cn/Article/details/ggsqxgjdq.sHtML

Ruby: a == b
来源：http://baike.fehbvm.com/Article/details/gvyzbuvsd.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/ghtcelfpj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gdvvsqkek.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.blog.hesvh.cn/Article/details/gdagbfuai.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/gxrzpihrm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.blog.fehbvm.com/Article/details/gbuyqgljb.sHtML

TS:   if (x == null) {}
来源：http://baike.hesvh.cn/Article/details/gxfiizlzt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gxjpeqnbh.sHtML

Go:   if x == nil {}
来源：http://mobile.hesvh.cn/Article/details/gpemhblid.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://3g.hesvh.cn/Article/details/gakqvstsq.sHtML

C#:   if (x is null) {}
来源：http://www.m.share.hesvh.cn/Article/details/goiuxuwwf.sHtML

[P07] 防抖与节流
来源：http://www.m.share.hesvh.cn/Article/details/gevmmvznt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://blog.zdbjq.cn/Article/details/ghhtwnpxr.sHtML

PHP:  // 手写时间戳比较
来源：http://www.m.share.zdbjq.cn/Article/details/ghdkqiipz.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.fehbvm.com/Article/details/gravkpkgg.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/grqtlpupb.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/goytckuet.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.blog.fehbvm.com/Article/details/gcilypseo.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://mobile.fehbvm.com/Article/details/gsxpmiljo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.share.hesvh.cn/Article/details/ghwjthvia.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.hesvh.cn/Article/details/gmvrwakxl.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.m.share.fehbvm.com/Article/details/guiatggga.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://baike.fehbvm.com/Article/details/gownqnhev.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/ginwkyzlw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/guhqccsuc.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gfmtsowdc.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.hesvh.cn/Article/details/gvqzzwsjv.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gwsofvbhq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://baike.zdbjq.cn/Article/details/gibbibdqn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmztxpcws.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/grbfboupj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfdpabeks.sHtML

[Q01] 创建表
来源：http://wap.hesvh.cn/Article/details/glhqdakii.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gzfryezpq.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.fehbvm.com/Article/details/gegcxknxh.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/ginvhxhhi.sHtML

email VARCHAR(100) UNIQUE,
来源：http://mobile.hesvh.cn/Article/details/gxafoubqo.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://blog.fehbvm.com/Article/details/gforgpcet.sHtML

);
来源：http://m.share.hesvh.cn/Article/details/gpxqprxaq.sHtML

[Q02] 创建带外键的表
来源：http://mobile.fehbvm.com/Article/details/gauxppnrq.sHtML

CREATE TABLE orders (
来源：http://www.share.zdbjq.cn/Article/details/gxtneyrqt.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.zdbjq.cn/Article/details/gpdvigxkg.sHtML

user_id INT NOT NULL,
来源：http://3g.hesvh.cn/Article/details/gyoqnkvhv.sHtML

amount DECIMAL(10, 2),
来源：http://baike.zdbjq.cn/Article/details/gtklstxya.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.hesvh.cn/Article/details/gzzthoasd.sHtML

);
来源：http://read.share.hesvh.cn/Article/details/gyoixvqtu.sHtML

[Q03] 增加列
来源：http://wap.fehbvm.com/Article/details/golpdelrh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://wap.zdbjq.cn/Article/details/gqplhphpf.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gycjhmhid.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.hesvh.cn/Article/details/gnpymdeie.sHtML

[Q05] 重命名列
来源：http://www.m.share.fehbvm.com/Article/details/gzdbpwtdr.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.fehbvm.com/Article/details/gkquslvtt.sHtML

[Q06] 删除列
来源：http://www.m.share.hesvh.cn/Article/details/gnlesndtb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.fehbvm.com/Article/details/gzkvtppxl.sHtML

[Q07] 删除表
来源：http://wap.hesvh.cn/Article/details/goxaxnwdk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gioeknouc.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.fehbvm.com/Article/details/gnwqnnfuj.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gjwruvcwb.sHtML

[Q09] 创建唯一索引
来源：http://mobile.hesvh.cn/Article/details/gfxzrexro.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.fehbvm.com/Article/details/gecfdzjzk.sHtML

[Q10] 插入单行
来源：http://wap.zdbjq.cn/Article/details/giofzjjrv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.fehbvm.com/Article/details/gmmumgylc.sHtML

[Q11] 一次插入多行
来源：http://3g.zdbjq.cn/Article/details/gvncigzhh.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://wap.fehbvm.com/Article/details/gjvwxapjf.sHtML

[Q12] 插入后取自增 ID
来源：http://wap.fehbvm.com/Article/details/gecjqmyoi.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.hesvh.cn/Article/details/gwtsfnxsi.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.zdbjq.cn/Article/details/gmqbzbjvt.sHtML

[Q13] 忽略重复插入
来源：http://www.share.fehbvm.com/Article/details/gxacwzwje.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gfhpnbwoc.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.fehbvm.com/Article/details/grrtgzaya.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gjqymuilq.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gkamgkzfk.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gfowhuxuj.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqkitkjvs.sHtML

[Q16] 查询指定列
来源：http://www.blog.zdbjq.cn/Article/details/gfpzywbzj.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gdwvdaamt.sHtML

[Q17] 条件查询
来源：http://3g.fehbvm.com/Article/details/gcfuoslgk.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.fehbvm.com/Article/details/grnqzfdgx.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/ggjmkegtq.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://3g.fehbvm.com/Article/details/gbjymbsfj.sHtML

[Q19] 范围查询
来源：http://read.share.hesvh.cn/Article/details/gzltyflgd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/gnniqgsmh.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gopsermco.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.hesvh.cn/Article/details/gyceljgmp.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gidkrqnxy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.hesvh.cn/Article/details/gntkxqztr.sHtML

[Q22] 排序
来源：http://blog.hesvh.cn/Article/details/gumrdjxer.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.fehbvm.com/Article/details/gqzbgibtz.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gxioomhpv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gjzsmpzso.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gynwwaley.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gnmyelnno.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gcmsauhbg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gnmzkqyzp.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gfnbonkwi.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gqwnecknh.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gzsvoikvs.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggrlrivls.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gtstpwxdn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gypmharzt.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gdakmxdma.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxcgeqjkl.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gdxwczpha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gzxbwtcea.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gltjnanvj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.hesvh.cn/Article/details/gewbldhqf.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/gxlsyowyj.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gvdlvbrue.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/groknowug.sHtML

[Q33] 多列分组
来源：http://wap.hesvh.cn/Article/details/gvhhffhsa.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fehbvm.com/Article/details/ghscvzcap.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fehbvm.com/Article/details/gaynctuwo.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gtrsjuydt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gwtjcuwdk.sHtML

) t WHERE rn = 1;
来源：http://baike.zdbjq.cn/Article/details/gsxsbdfpw.sHtML

[Q35] 内连接
来源：http://mobile.zdbjq.cn/Article/details/gsafvjmnf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gactvdeee.sHtML

[Q36] 左连接
来源：http://m.share.zdbjq.cn/Article/details/gczveqiyc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gdcalpeod.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/ggztzpkny.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gfzgbnhlr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gjrxevnet.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.zdbjq.cn/Article/details/gglnfbphu.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gswtmskhp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gljsmzitp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gjsynkpeq.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gdaixxsnt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fehbvm.com/Article/details/gsfpiooxf.sHtML

[Q41] 多表连接
来源：http://mobile.hesvh.cn/Article/details/gsegmgwum.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.hesvh.cn/Article/details/gnlavjqgd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gvdztgwyn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gkwejbyvs.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.fehbvm.com/Article/details/gtmgqkhpf.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gcmkbrxap.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gksckbvlp.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/gmfveywem.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gxhyhpzxy.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gkawovelq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gauxzwiyt.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gtxpzugva.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gpocinndr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gqbhqvdup.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gcoltrnmz.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gofkrnfzf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gmdsbvafs.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/geaoiycrq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fehbvm.com/Article/details/gzjsvxkca.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gcpwiohra.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gjzfmveqr.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gyktvwkbr.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gvcmtetch.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.hesvh.cn/Article/details/glprchcki.sHtML

[Q51] 用子查询更新
来源：http://wap.hesvh.cn/Article/details/geelxbjok.sHtML


<!-- 参考信息 -->