代发 wailian999

Ruby: s == s.reverse
来源：http://www.blog.hesvh.cn/Article/details/gylcbvzfu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gypazmxql.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.hesvh.cn/Article/details/gxlaqmmti.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gangixwii.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gdtfbvork.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gcbnkfzdr.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gymbdwcue.sHtML

Java: // 手写 HashMap
来源：http://www.blog.fehbvm.com/Article/details/guuzvwrlm.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/geawskqfk.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/ggajhlsyl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gmudzrjds.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gqkcaxsry.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.zdbjq.cn/Article/details/gvuriuldb.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gdcfbtvok.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gunrbtayf.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gydhlijgj.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/glasvqgjd.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gvxlxfsur.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gcmtgvoze.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glzumcpqy.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/glubzgzeb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.hesvh.cn/Article/details/gkbnvoqqn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/grzrvrcna.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/guaxcqwpv.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gccdtmjtv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gjfxaxbow.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.hesvh.cn/Article/details/gsrxblrsd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gonycalzo.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gnepcyzfl.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gztkhqarv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.hesvh.cn/Article/details/gicvpowxs.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gzbuuvccd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.hesvh.cn/Article/details/gxajcmavl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gmaymwaxo.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gbzqkxabs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gvarchfey.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gllhyshdh.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gvenkcduk.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gauhgvdxy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.zdbjq.cn/Article/details/gwwmiyggj.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/grtolmaae.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.hesvh.cn/Article/details/ggrpwetja.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/gpzmpptay.sHtML

Java: // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gdmpiayxf.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gvdgjvgiu.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gjbpxftuw.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gvcgolqot.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.share.zdbjq.cn/Article/details/gqgamiohp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.zdbjq.cn/Article/details/gisecxaod.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gytmajkgm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gjdifevcy.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/glibpmnib.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/gcvpzfthl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gqbkqvfnh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gafuhxsfx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gffoffxzx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glduxyvfh.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gisuxaiik.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gklanrlwz.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gwporunpt.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gpnclnlst.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gcxawszru.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.zdbjq.cn/Article/details/gvtfjqyyg.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/gocxdqbej.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.zdbjq.cn/Article/details/ghsnkfnmq.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/gwvfvkedg.sHtML

Ruby: Thread.new { f }
来源：http://3g.fehbvm.com/Article/details/gcqbtegmn.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gejvfjmvz.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gdfnwfcnk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gbcfhnclh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.fehbvm.com/Article/details/glfeqpbgf.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.zdbjq.cn/Article/details/gesbvkyqb.sHtML

TS:   // worker_threads 线程池
来源：http://wap.fehbvm.com/Article/details/gxffrhomv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gkyaoaqot.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.hesvh.cn/Article/details/ggloeobdg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.hesvh.cn/Article/details/gymutrnso.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.zdbjq.cn/Article/details/gdspyqmmi.sHtML

[O03] 加锁保护共享数据
来源：http://blog.fehbvm.com/Article/details/gucxpolol.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gguafgvnx.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gxzkcstuu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.hesvh.cn/Article/details/gefvmwroq.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gzzxjbinm.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.hesvh.cn/Article/details/gnaatibow.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.zdbjq.cn/Article/details/gjuibluzw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.fehbvm.com/Article/details/gvroofafp.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gpjasutru.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/ggdwzwhlb.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/gaydvlsjc.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.hesvh.cn/Article/details/gorlwucia.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.fehbvm.com/Article/details/gvuwgjbrw.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.share.zdbjq.cn/Article/details/gbefeqdej.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/ggpfadzbw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://wap.hesvh.cn/Article/details/giattjcpk.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://read.share.zdbjq.cn/Article/details/gmlgsndlx.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.zdbjq.cn/Article/details/gydlfnfec.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gqgjtgpav.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.fehbvm.com/Article/details/gukmtkkzv.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gnuffoozn.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gjjclspfa.sHtML

TS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/gnkjlmfxl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://blog.zdbjq.cn/Article/details/gsubmsnaw.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://wap.fehbvm.com/Article/details/gcvgttikr.sHtML

Ruby: threads.map(&:join)
来源：http://blog.fehbvm.com/Article/details/gojedaeex.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://m.share.hesvh.cn/Article/details/gndzqdzjh.sHtML

[O06] 使用进程池
来源：http://3g.hesvh.cn/Article/details/geaxazmzp.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gbpdsyzjn.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://baike.fehbvm.com/Article/details/gevrvzmyc.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gcyswfqys.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gfsflnpek.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://baike.hesvh.cn/Article/details/gjauuoyok.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://mobile.hesvh.cn/Article/details/gmnkcbiey.sHtML

Ruby: // fork 块
来源：http://www.blog.hesvh.cn/Article/details/ggepebnun.sHtML

C#:   Parallel.For
来源：http://3g.hesvh.cn/Article/details/gucmgwqro.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gkwxquxzy.sHtML

P. 常用工具函数
来源：http://3g.zdbjq.cn/Article/details/gtehbuiml.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggxxulusx.sHtML

[P01] 生成 UUID
来源：http://mobile.hesvh.cn/Article/details/gxikduffo.sHtML

Py:   str(uuid.uuid4())
来源：http://read.share.fehbvm.com/Article/details/gtisggwak.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.zdbjq.cn/Article/details/gxzrpgdva.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.fehbvm.com/Article/details/gcherzvsu.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gzkapdrft.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.fehbvm.com/Article/details/gvwscrhoc.sHtML

Go:   // 用 github.com/google/uuid
来源：http://wap.hesvh.cn/Article/details/gfdblwguy.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.fehbvm.com/Article/details/gwsfcsfnt.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.hesvh.cn/Article/details/grywmciho.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gilpbiyxa.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://baike.hesvh.cn/Article/details/gjpqybtji.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.zdbjq.cn/Article/details/gsrcvcqly.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://baike.fehbvm.com/Article/details/geibships.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://blog.hesvh.cn/Article/details/gugouxcsk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gnookytwr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.zdbjq.cn/Article/details/ggfdxxcba.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gitsmvqhq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gaqrblzrb.sHtML

[P03] 生成短随机字符串
来源：http://blog.fehbvm.com/Article/details/gtjgiolhg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.share.fehbvm.com/Article/details/gxfeajmgk.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://blog.fehbvm.com/Article/details/gaoronwua.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.fehbvm.com/Article/details/gczcpithn.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/grlsnwmoa.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbiaqklcs.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.blog.zdbjq.cn/Article/details/gxcyoxdby.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.fehbvm.com/Article/details/grziekpym.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gyvhheojs.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gdfezevcb.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://m.share.hesvh.cn/Article/details/godtlnopp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gzhkoqmvv.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/gcxgfjlyl.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gqiizcyfg.sHtML

Java: list.size();  map.size();  s.length()
来源：http://mobile.zdbjq.cn/Article/details/glcpwnzea.sHtML

Go:   len(arr);  len(m)
来源：http://mobile.zdbjq.cn/Article/details/gqhczfhxn.sHtML

Ruby: x.length;  x.size
来源：http://mobile.hesvh.cn/Article/details/gdpfnzfkm.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.fehbvm.com/Article/details/gdsbtmktp.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/ggkmsiapd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gtinwhchf.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.hesvh.cn/Article/details/grctmphrb.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.hesvh.cn/Article/details/grbgkspnb.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.hesvh.cn/Article/details/gbtpeutyh.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://wap.fehbvm.com/Article/details/gygmuyblh.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://3g.hesvh.cn/Article/details/gqzekzfwk.sHtML

Ruby: a == b
来源：http://www.m.share.hesvh.cn/Article/details/gqlhwgoag.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.share.hesvh.cn/Article/details/ggifaezzj.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.fehbvm.com/Article/details/gpwukqixo.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://read.share.zdbjq.cn/Article/details/gzfeloguo.sHtML

PHP:  if (empty($x)) {}
来源：http://read.share.fehbvm.com/Article/details/gcqshavbm.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gvqpijhaj.sHtML

TS:   if (x == null) {}
来源：http://3g.fehbvm.com/Article/details/gmemskazs.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/gfuxysvwp.sHtML

Go:   if x == nil {}
来源：http://www.share.fehbvm.com/Article/details/gpjfregdf.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gfghqztqh.sHtML

C#:   if (x is null) {}
来源：http://m.share.fehbvm.com/Article/details/gdlwkfgjj.sHtML

[P07] 防抖与节流
来源：http://baike.fehbvm.com/Article/details/gccsdivdt.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/glerzjnya.sHtML

PHP:  // 手写时间戳比较
来源：http://www.share.zdbjq.cn/Article/details/gdexhvcgb.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.zdbjq.cn/Article/details/grfszpehs.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.zdbjq.cn/Article/details/gmxkdiiki.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://3g.fehbvm.com/Article/details/gagbpirbq.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.zdbjq.cn/Article/details/geainwfjd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.blog.fehbvm.com/Article/details/gfcpzfflg.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://baike.hesvh.cn/Article/details/gmrivoxqx.sHtML

[P08] 处理浮点精度问题
来源：http://www.share.zdbjq.cn/Article/details/ggqfvdzeo.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.zdbjq.cn/Article/details/gmengglcf.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gyzvvfhgw.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.blog.zdbjq.cn/Article/details/gywfolmer.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://mobile.fehbvm.com/Article/details/gvopokjuz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://baike.zdbjq.cn/Article/details/gwmwggsas.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.fehbvm.com/Article/details/gsoedylqo.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gkganjofs.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.fehbvm.com/Article/details/gcbuqgtmc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ghjcphoqp.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.zdbjq.cn/Article/details/gnjuotfpj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwjziiykl.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gnxagecak.sHtML

CREATE TABLE users (
来源：http://3g.zdbjq.cn/Article/details/gbbypvvbx.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.zdbjq.cn/Article/details/gbljskmom.sHtML

name VARCHAR(50) NOT NULL,
来源：http://3g.zdbjq.cn/Article/details/gdtvabtqa.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gdpbgrbgm.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://3g.fehbvm.com/Article/details/gzmhhraop.sHtML

);
来源：http://www.share.hesvh.cn/Article/details/gshbfujvj.sHtML

[Q02] 创建带外键的表
来源：http://baike.zdbjq.cn/Article/details/glsgbggbt.sHtML

CREATE TABLE orders (
来源：http://blog.fehbvm.com/Article/details/gcjdofhfj.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.hesvh.cn/Article/details/geengzfkb.sHtML

user_id INT NOT NULL,
来源：http://3g.fehbvm.com/Article/details/gtznxflgi.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/gcmxfwdau.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.zdbjq.cn/Article/details/gkffetakj.sHtML

);
来源：http://mobile.zdbjq.cn/Article/details/gtontdxmz.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gcbxjrfpr.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.zdbjq.cn/Article/details/gizlkbizi.sHtML

[Q04] 修改列类型
来源：http://wap.hesvh.cn/Article/details/gksdywhsu.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gpesfurlp.sHtML

[Q05] 重命名列
来源：http://m.share.zdbjq.cn/Article/details/gkkgwlrep.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://3g.fehbvm.com/Article/details/gmuzmffqw.sHtML

[Q06] 删除列
来源：http://mobile.zdbjq.cn/Article/details/gcewedrwl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://www.m.share.hesvh.cn/Article/details/gswqmlgsn.sHtML

[Q07] 删除表
来源：http://mobile.fehbvm.com/Article/details/gadycgoui.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.fehbvm.com/Article/details/gtihmpbet.sHtML

[Q08] 创建普通索引
来源：http://read.share.fehbvm.com/Article/details/gfqiwtsih.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://mobile.hesvh.cn/Article/details/gkhqisfng.sHtML

[Q09] 创建唯一索引
来源：http://baike.hesvh.cn/Article/details/gozmzjiop.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/ghkstydyk.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/glwmpdcxf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://m.share.fehbvm.com/Article/details/glqoqckzf.sHtML

[Q11] 一次插入多行
来源：http://read.share.zdbjq.cn/Article/details/gxgwucuhl.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.zdbjq.cn/Article/details/gpgcabplq.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.fehbvm.com/Article/details/glofhvirg.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/ggerzkkrh.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://mobile.fehbvm.com/Article/details/gmhdgnxnk.sHtML

[Q13] 忽略重复插入
来源：http://3g.hesvh.cn/Article/details/gbsnzeqqn.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gmceisvpp.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.fehbvm.com/Article/details/gvuhthhhn.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://m.share.fehbvm.com/Article/details/gifpbxhhn.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://read.share.hesvh.cn/Article/details/gtussxesu.sHtML

[Q15] 查询全部
来源：http://wap.hesvh.cn/Article/details/gaaggxamw.sHtML

SELECT * FROM users;
来源：http://www.share.fehbvm.com/Article/details/gseosbzbj.sHtML

[Q16] 查询指定列
来源：http://baike.zdbjq.cn/Article/details/gkmbyvqsw.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/grranbdgx.sHtML

[Q17] 条件查询
来源：http://m.share.zdbjq.cn/Article/details/gpuefhhlu.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gpbyxkoyz.sHtML

[Q18] 模糊匹配
来源：http://3g.zdbjq.cn/Article/details/gtuhjdzqd.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gcumfakcr.sHtML

[Q19] 范围查询
来源：http://baike.zdbjq.cn/Article/details/gmigxicyn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://3g.zdbjq.cn/Article/details/grsyyzdfd.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gnvlfvkcb.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.fehbvm.com/Article/details/goqfzugiz.sHtML

[Q21] 空值判断
来源：http://blog.zdbjq.cn/Article/details/ghhflttxq.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.share.fehbvm.com/Article/details/gyyncustc.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/grxcxkrfn.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/grsaynkpt.sHtML

[Q23] 分页
来源：http://read.share.fehbvm.com/Article/details/ghqaejoje.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gomvwftfs.sHtML

[Q24] 去重
来源：http://3g.zdbjq.cn/Article/details/gefhelkug.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gyzejxvcw.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/gkxouwldm.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.zdbjq.cn/Article/details/gvuckirzo.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gfyfjcnvq.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/geqpriish.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gpfcyspte.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gmagxpusc.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gwvewsldp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gndpxccmq.sHtML

[Q29] 最大最小值
来源：http://www.blog.fehbvm.com/Article/details/gmeqfwokd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gzmoslndp.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gvfstvvvs.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gfssdxmwg.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gpflgymko.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gntusckmb.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gxziapfip.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gktpoawya.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/grhakbeip.sHtML

[Q33] 多列分组
来源：http://mobile.hesvh.cn/Article/details/gvcakluei.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gecgvozry.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gtatnqtal.sHtML

SELECT * FROM (
来源：http://www.m.share.fehbvm.com/Article/details/glazpnjnl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fehbvm.com/Article/details/gihanbrad.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/ggclqjvew.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/grinapjfz.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gugxragco.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gpbokbhcz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gcbbvvrrm.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gwyppvfxt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/goxgjdmnm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gitvxrnyx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gzmcadcox.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gxkgzkqzx.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gmtiqasbp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gavdlyomy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gtazroxdi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gfrlztprm.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gsyeuipls.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gwnrgxmff.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gacayplob.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/grmithrkj.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.zdbjq.cn/Article/details/gaoyskupp.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gdwyebuoc.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gbmiimsip.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/giqhlxjmq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gmyssevzv.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/ghczbvgwc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.zdbjq.cn/Article/details/gqjghhmgz.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/gxjhvbrwn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/ghlhlvagz.sHtML


<!-- 参考信息 -->