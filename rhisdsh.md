代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmyyrafdt.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gcwtavxut.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/gofvxfomv.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gsrznoesg.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gybpiaxpb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gfticvyox.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gunkfpiyv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/ggvdnbabk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gzolacdhv.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gaqxgrecg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gesrrgtjd.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/ghqcgxvgc.sHtML

Go:   // 手写 map[int]int
来源：http://blog.zdbjq.cn/Article/details/geyyjepts.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gbifhvkzv.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gmoadlhgv.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gzktpfqde.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gyvzbqbor.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/gitshyxag.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvbnligkn.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gkhwhcuno.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gpqsdjsjb.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpnrfszkh.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/goxwdaskz.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gsdhauazq.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/garjkzpdi.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/glugumxmj.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/guzakickd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gtlessoof.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gcrwqmynu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/glypvzprn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gomxezfss.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gxliltncc.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.zdbjq.cn/Article/details/gpubcrwzb.sHtML

[N10] 链表节点定义
来源：http://mobile.zdbjq.cn/Article/details/gcaiyukuq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gqgjzbmpr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/ggmiieexq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gboxdpdfl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.zdbjq.cn/Article/details/grhtfsiak.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gtsctdvlm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.hesvh.cn/Article/details/groxlybvj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/goengegqq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gnmjfumrs.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/glqcmidfc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gocbdttig.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/guycvarrv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gnateywkh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gtlcwohaj.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/gdhusmrja.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gacbvxkfb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.hesvh.cn/Article/details/glrfbjpsp.sHtML

C#:   // 手写递归
来源：http://blog.hesvh.cn/Article/details/guqegfwgx.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/gaafzywnq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gowcajzoe.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gfycqqmyw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/gyzbpfqst.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gbvlnlhrm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gpforcgbc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gdlzjzayv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gtuapgtde.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gjexnezpg.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcmojkhqn.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/guhhpccac.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gwsaudzzw.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/grobmzwfu.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gvvbkccfv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/ghcpgtfss.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.hesvh.cn/Article/details/ggquiwqly.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gbdqitahe.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gqnaslfvg.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gctqgxlyp.sHtML

Ruby: Thread.new { f }
来源：http://baike.zdbjq.cn/Article/details/gjjrbwejc.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gdvmazajv.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/ggvekpqfe.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.zdbjq.cn/Article/details/glgppxrtf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gmadwiopw.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gqmuzgvmh.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/ggncbkfqu.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gtcfjhjda.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.fehbvm.com/Article/details/grtkmawne.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.hesvh.cn/Article/details/ghfhiggzp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/glupxrizh.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gqlunfutv.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.hesvh.cn/Article/details/garbgrkpm.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.hesvh.cn/Article/details/gchronarq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.fehbvm.com/Article/details/gojtextwk.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gbqbahrai.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/ggphbwcua.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/guhyhbcsl.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gxostfptp.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gkfnapkbe.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.hesvh.cn/Article/details/gnvwwhqwr.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.zdbjq.cn/Article/details/gqjksfppr.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://m.share.hesvh.cn/Article/details/ghvgdyrqt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gpwtewrac.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gmgorrqiz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gwvfjzvkb.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.hesvh.cn/Article/details/ghhcyannz.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.fehbvm.com/Article/details/gnnajcowt.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gwcxqmypc.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.hesvh.cn/Article/details/gxjckeyzo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gmvprofxl.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gbpajqxnu.sHtML

JS:   await Promise.all(tasks)
来源：http://www.m.share.fehbvm.com/Article/details/guvjnqwxw.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/guykvszvx.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.share.hesvh.cn/Article/details/gfwaqcvez.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.m.share.fehbvm.com/Article/details/gncyyoygn.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gsnwzgaoq.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://3g.zdbjq.cn/Article/details/ggkejzcuu.sHtML

[O06] 使用进程池
来源：http://www.blog.fehbvm.com/Article/details/gucjdsixj.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.hesvh.cn/Article/details/gfvhgvzed.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://blog.fehbvm.com/Article/details/gixkigynb.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.zdbjq.cn/Article/details/gbosgwpti.sHtML

TS:   // child_process / cluster 模块
来源：http://www.blog.hesvh.cn/Article/details/gqgzajudr.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/goodigdlz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.m.share.fehbvm.com/Article/details/gczukpaip.sHtML

Ruby: // fork 块
来源：http://baike.fehbvm.com/Article/details/glrmbteas.sHtML

C#:   Parallel.For
来源：http://blog.fehbvm.com/Article/details/gtldddlqg.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gzbadwtpm.sHtML

P. 常用工具函数
来源：http://wap.zdbjq.cn/Article/details/gjztffoqq.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsyigpecz.sHtML

[P01] 生成 UUID
来源：http://www.share.zdbjq.cn/Article/details/gtttqabrf.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.zdbjq.cn/Article/details/ggecodxjc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.share.zdbjq.cn/Article/details/gevxwlvhs.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gjifhczmc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gfnbxnorl.sHtML

Java: UUID.randomUUID().toString()
来源：http://read.share.hesvh.cn/Article/details/gvnegbjnw.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.fehbvm.com/Article/details/gvlprtuob.sHtML

Ruby: SecureRandom.uuid
来源：http://blog.zdbjq.cn/Article/details/gpijlefxp.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://baike.zdbjq.cn/Article/details/gpdtbkszy.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.fehbvm.com/Article/details/gyixbrzap.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.hesvh.cn/Article/details/gmxefcapa.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://m.share.hesvh.cn/Article/details/gojcnwitv.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://m.share.fehbvm.com/Article/details/grvkouvee.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.blog.hesvh.cn/Article/details/gpcchashd.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://wap.fehbvm.com/Article/details/gtkoptnwb.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://read.share.zdbjq.cn/Article/details/gblgmlcjn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://blog.zdbjq.cn/Article/details/gaghjvxfs.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.blog.zdbjq.cn/Article/details/gdzzlhunq.sHtML

[P03] 生成短随机字符串
来源：http://blog.zdbjq.cn/Article/details/gicobhlwg.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.blog.zdbjq.cn/Article/details/gwzmpgemu.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gmzebifnv.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gkvdjhtxa.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.blog.zdbjq.cn/Article/details/gtwwvdxyz.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.zdbjq.cn/Article/details/ghxywkosu.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.hesvh.cn/Article/details/gnpuxsyjj.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.zdbjq.cn/Article/details/glwwiasbx.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.m.share.zdbjq.cn/Article/details/gxesqfpqe.sHtML

[P04] 求长度
来源：http://www.m.share.zdbjq.cn/Article/details/gdxviflwt.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gtnfqtkpp.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.hesvh.cn/Article/details/ghescfmok.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://mobile.zdbjq.cn/Article/details/grasledqv.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://3g.hesvh.cn/Article/details/gnyjotuod.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/griappuoo.sHtML

Go:   len(arr);  len(m)
来源：http://blog.fehbvm.com/Article/details/gmfroxkma.sHtML

Ruby: x.length;  x.size
来源：http://www.blog.fehbvm.com/Article/details/ggmdlzbgr.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/gnusymfpk.sHtML

[P05] 判断两个对象内容是否相等
来源：http://baike.fehbvm.com/Article/details/gyhaegupp.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://wap.fehbvm.com/Article/details/gepgkkxws.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.zdbjq.cn/Article/details/gpnpstwzm.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://blog.hesvh.cn/Article/details/gbqjxcgju.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/glqrwbqpv.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/gmacrzxml.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://wap.zdbjq.cn/Article/details/gpopcazbq.sHtML

Ruby: a == b
来源：http://3g.fehbvm.com/Article/details/gksjiggyb.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://mobile.zdbjq.cn/Article/details/gnuacgwds.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.fehbvm.com/Article/details/gxuihvsaa.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://baike.zdbjq.cn/Article/details/gpuxbvvib.sHtML

PHP:  if (empty($x)) {}
来源：http://mobile.fehbvm.com/Article/details/geqlzznxl.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gzyalcjkz.sHtML

TS:   if (x == null) {}
来源：http://read.share.hesvh.cn/Article/details/gsjiwmubt.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gxlnebtxl.sHtML

Go:   if x == nil {}
来源：http://m.share.zdbjq.cn/Article/details/ggdnfwvvo.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://baike.zdbjq.cn/Article/details/glirxohgv.sHtML

C#:   if (x is null) {}
来源：http://www.share.zdbjq.cn/Article/details/gxrkibngu.sHtML

[P07] 防抖与节流
来源：http://baike.zdbjq.cn/Article/details/gzfzawtky.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://mobile.hesvh.cn/Article/details/ghzhuxecs.sHtML

PHP:  // 手写时间戳比较
来源：http://mobile.hesvh.cn/Article/details/gllugglvl.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://baike.zdbjq.cn/Article/details/gunbhnsdh.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.hesvh.cn/Article/details/gzmwbdvhs.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gfugizghv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.share.hesvh.cn/Article/details/gvirijmbd.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gfnldmzwo.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.blog.zdbjq.cn/Article/details/gvxiexglh.sHtML

[P08] 处理浮点精度问题
来源：http://mobile.hesvh.cn/Article/details/gdnefzxbw.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://blog.fehbvm.com/Article/details/guhrnnvox.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://mobile.hesvh.cn/Article/details/gpitfjqqi.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://mobile.fehbvm.com/Article/details/gokbaspzk.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://read.share.hesvh.cn/Article/details/giyqlwyvu.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.fehbvm.com/Article/details/gsduhovkf.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gvgnjaxli.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.fehbvm.com/Article/details/gdoafncwh.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.hesvh.cn/Article/details/gutvlhsyn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/goyqpppqi.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.zdbjq.cn/Article/details/gahrsgaug.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxxfsqtkp.sHtML

[Q01] 创建表
来源：http://baike.zdbjq.cn/Article/details/gltzmnsgn.sHtML

CREATE TABLE users (
来源：http://wap.hesvh.cn/Article/details/ghhiyngvn.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gnpekmlng.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.m.share.zdbjq.cn/Article/details/gunjdzfhc.sHtML

email VARCHAR(100) UNIQUE,
来源：http://read.share.zdbjq.cn/Article/details/gqdycuets.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://m.share.zdbjq.cn/Article/details/gtezsafja.sHtML

);
来源：http://baike.zdbjq.cn/Article/details/gnwywvnyc.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.zdbjq.cn/Article/details/gjwoqpimb.sHtML

CREATE TABLE orders (
来源：http://blog.zdbjq.cn/Article/details/gxzaqrcus.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://3g.fehbvm.com/Article/details/glpgacvtb.sHtML

user_id INT NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gubcauldu.sHtML

amount DECIMAL(10, 2),
来源：http://baike.hesvh.cn/Article/details/gconacvhi.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gfstzwehq.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gmgvyyowp.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gqjajwwot.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.blog.hesvh.cn/Article/details/getvtavcq.sHtML

[Q04] 修改列类型
来源：http://m.share.fehbvm.com/Article/details/ggphshxpg.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://m.share.fehbvm.com/Article/details/gqhouuzbw.sHtML

[Q05] 重命名列
来源：http://m.share.fehbvm.com/Article/details/grqzwlvlp.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://baike.hesvh.cn/Article/details/gskdyhyjb.sHtML

[Q06] 删除列
来源：http://wap.hesvh.cn/Article/details/gpmewwawm.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://3g.fehbvm.com/Article/details/gpcjneqhf.sHtML

[Q07] 删除表
来源：http://wap.fehbvm.com/Article/details/gxjvzykbi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.fehbvm.com/Article/details/gedlolczz.sHtML

[Q08] 创建普通索引
来源：http://www.share.fehbvm.com/Article/details/gxfjonoia.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gqbhpvxpd.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gieaqufth.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.share.fehbvm.com/Article/details/guqwfgziq.sHtML

[Q10] 插入单行
来源：http://www.m.share.hesvh.cn/Article/details/gxtyyyugv.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://wap.hesvh.cn/Article/details/gfbynzprs.sHtML

[Q11] 一次插入多行
来源：http://m.share.zdbjq.cn/Article/details/goaaftyiv.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://baike.hesvh.cn/Article/details/gwevfpumc.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.fehbvm.com/Article/details/gyshjanil.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.hesvh.cn/Article/details/gikhvgmyr.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.hesvh.cn/Article/details/gzloxajnf.sHtML

[Q13] 忽略重复插入
来源：http://wap.hesvh.cn/Article/details/giqucfwvw.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.m.share.zdbjq.cn/Article/details/gpziqtmmu.sHtML

[Q14] 存在则更新（upsert）
来源：http://baike.zdbjq.cn/Article/details/gbwsozrku.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/giuhxemgz.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://blog.zdbjq.cn/Article/details/gwjiecjjm.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gfveuzzrf.sHtML

SELECT * FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnpxeffys.sHtML

[Q16] 查询指定列
来源：http://m.share.fehbvm.com/Article/details/gbrtwkdjs.sHtML

SELECT id, name FROM users;
来源：http://m.share.fehbvm.com/Article/details/guicvvcew.sHtML

[Q17] 条件查询
来源：http://baike.fehbvm.com/Article/details/gpalobhzz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/ghvbkrnop.sHtML

[Q18] 模糊匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gzuhgpdft.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gtkcvirkn.sHtML

[Q19] 范围查询
来源：http://3g.zdbjq.cn/Article/details/gzomnnotf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.hesvh.cn/Article/details/gpzunhbhi.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gcwscfnca.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtwicbrsu.sHtML

[Q21] 空值判断
来源：http://read.share.fehbvm.com/Article/details/gexlofhnf.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.hesvh.cn/Article/details/goowrnjke.sHtML

[Q22] 排序
来源：http://wap.zdbjq.cn/Article/details/ghrwbmmpm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/guizamwls.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/glecekhda.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/grksoyxxr.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gzivgcmws.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.zdbjq.cn/Article/details/ggxyopbnp.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gmvfnymzt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gpxfzdgmj.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gatdtzhzp.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.fehbvm.com/Article/details/gflfreert.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gmkxeycsc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxyufidzp.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gtbnnhmmx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gyjhqamul.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gctkscjza.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxyquptzk.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gohjmsgom.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/grhagurvg.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gydelwhmg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gpywytocd.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gbuisriru.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/gvcwvppyq.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gtbxwlmtv.sHtML

[Q33] 多列分组
来源：http://3g.hesvh.cn/Article/details/gtovjmzpu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/ghpmhjmqj.sHtML

[Q34] 每组取第一条
来源：http://mobile.zdbjq.cn/Article/details/gvmvmmiqm.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gocflivsd.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gnkjpyktt.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gjdzaotrt.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gbfljlswt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/grwbjzlac.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/glyoplice.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/grwhnaaog.sHtML

[Q37] 右连接
来源：http://blog.zdbjq.cn/Article/details/ghvrsbsvx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gemfhzjqj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gixyjauuk.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gnillbnnw.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/galqhdumb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gjrayoggi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.hesvh.cn/Article/details/gsazycjhd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gugqzywvg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gryidqvgy.sHtML

[Q41] 多表连接
来源：http://blog.hesvh.cn/Article/details/gkckrigwt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gmevvnspx.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gdvkyxoyv.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gdttpdlxd.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gdipbjwav.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/glcgdsuql.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gqhrpeioc.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gbcjqrfka.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gthjfmywq.sHtML


<!-- 参考信息 -->