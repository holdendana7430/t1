代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gnxcbyyob.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gphzvcxls.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gkdjyjcgf.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/glnzgeqgj.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/geionlojv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gcsapnwvw.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gfqjuupvu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/ggtipbqfy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/grwtzymlb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gnvzpspte.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gusjsrmiz.sHtML

Java: // 手写 HashMap
来源：http://wap.zdbjq.cn/Article/details/gnxmviipa.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gnlgqmebd.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/gdrveuozs.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.hesvh.cn/Article/details/gnarfifrj.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gfizmgjyq.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gofaxphpa.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/gwapegkoo.sHtML

JS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gsuygznwm.sHtML

TS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gtowwaysh.sHtML

Java: // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gnqnabept.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gpqbwdjtj.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gvuhrphgd.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/garkgkhnc.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gkuguyjzb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/ggrjtcndy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gxyrzkbmd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gncopjvxo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gfvbftzip.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.hesvh.cn/Article/details/gzdnbufbn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.zdbjq.cn/Article/details/glxfdmtnt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gkghnzory.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/ghfocmchd.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gzunaeqor.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/gvfzkrieh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gthrhafdz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/glqpsddzs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.zdbjq.cn/Article/details/gqokybbrn.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gbypnmeqo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gjhbvhekr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.zdbjq.cn/Article/details/gbubrvsfz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gbjimkjxl.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gkfszesfv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gakiixnqz.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fehbvm.com/Article/details/gceyrrhbo.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gfaoixlki.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.hesvh.cn/Article/details/glqnkzneb.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gkgewfrgn.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gpfvljnad.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gnkqjkgfa.sHtML

C#:   // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/glqlkvdxn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.zdbjq.cn/Article/details/gvoilqpwn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/ggepwetuz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.zdbjq.cn/Article/details/gfjpoculf.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gkeismsig.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gruvtyjsc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/glvtutrgz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gbcvouxpg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.hesvh.cn/Article/details/gdzaxraxg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.zdbjq.cn/Article/details/gtdtjntir.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gmxbvnopo.sHtML

O. 并发与异步
来源：http://mobile.hesvh.cn/Article/details/gnzreizkd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gflhklhco.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/grswscdkh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/gzlvxudbs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.fehbvm.com/Article/details/gbzftkvvq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gcmdobtaj.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gfnijgvcc.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.fehbvm.com/Article/details/gtqkebilb.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gwwtobeok.sHtML

Ruby: Thread.new { f }
来源：http://www.share.zdbjq.cn/Article/details/gajytzmjd.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gaaakzlfg.sHtML

[O02] 使用线程池
来源：http://baike.fehbvm.com/Article/details/gcyaujvys.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.zdbjq.cn/Article/details/getqrabre.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.hesvh.cn/Article/details/gouxclquf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gagkxytqw.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gbaraifjk.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.hesvh.cn/Article/details/gibxoxxcc.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gzqblcwqr.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.hesvh.cn/Article/details/ginoohbcp.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://mobile.hesvh.cn/Article/details/gzbgudlgc.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gbvkubuxa.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gmoonfygl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gplwzvpwa.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://read.share.hesvh.cn/Article/details/gzrjzjtqx.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gactzrlre.sHtML

Java: synchronized (this) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gpllkqdob.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gzgobdyya.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.fehbvm.com/Article/details/gghzwnbbd.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/geoxzttop.sHtML

[O04] 定义异步函数并等待
来源：http://3g.zdbjq.cn/Article/details/gursykdpr.sHtML

Py:   async def f():⏎    await g()
来源：http://blog.zdbjq.cn/Article/details/gyxzidhhz.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/guiaqifzg.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/giizhboay.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/giwlbucrs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.fehbvm.com/Article/details/godcvwucy.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gmahopbxc.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.fehbvm.com/Article/details/gmkogavaw.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.fehbvm.com/Article/details/grbdohtfi.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.blog.zdbjq.cn/Article/details/gedulelxy.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gkewdqzok.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.fehbvm.com/Article/details/guqofiapw.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gmynvdmdt.sHtML

TS:   await Promise.all(tasks)
来源：http://baike.zdbjq.cn/Article/details/gknruiaof.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://mobile.fehbvm.com/Article/details/guqqoyess.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.fehbvm.com/Article/details/gtmreesjl.sHtML

Ruby: threads.map(&:join)
来源：http://www.blog.fehbvm.com/Article/details/gsxojsxvu.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.hesvh.cn/Article/details/gfynqrbib.sHtML

[O06] 使用进程池
来源：http://mobile.fehbvm.com/Article/details/gpjjkkfzy.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://mobile.zdbjq.cn/Article/details/gbborjspx.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/gvcjyblri.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.zdbjq.cn/Article/details/gesccokns.sHtML

TS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gvmxmohbs.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://read.share.fehbvm.com/Article/details/giqxpsmrr.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.hesvh.cn/Article/details/gspllnwrf.sHtML

Ruby: // fork 块
来源：http://www.share.fehbvm.com/Article/details/grxoplsip.sHtML

C#:   Parallel.For
来源：http://www.m.share.hesvh.cn/Article/details/gnrtjldqn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gltnhnttx.sHtML

P. 常用工具函数
来源：http://3g.fehbvm.com/Article/details/gmbjkatng.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gyxiutecx.sHtML

[P01] 生成 UUID
来源：http://blog.zdbjq.cn/Article/details/gmzokbgst.sHtML

Py:   str(uuid.uuid4())
来源：http://www.blog.fehbvm.com/Article/details/gxavsqhzz.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://baike.zdbjq.cn/Article/details/gyuvkmdzf.sHtML

JS:   crypto.randomUUID()
来源：http://www.m.share.zdbjq.cn/Article/details/gpqdjstpc.sHtML

TS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/geaddkbvw.sHtML

Java: UUID.randomUUID().toString()
来源：http://blog.fehbvm.com/Article/details/gfieblgsy.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.share.zdbjq.cn/Article/details/gmpenxxnu.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.zdbjq.cn/Article/details/gaaabzxpu.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.share.fehbvm.com/Article/details/gsktdsnrq.sHtML

[P02] MD5 / SHA256 摘要
来源：http://www.blog.hesvh.cn/Article/details/goyeamqtk.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gweyodndv.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/glmqyyddz.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.fehbvm.com/Article/details/gwnzomhtl.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/glfwxhxhk.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.blog.fehbvm.com/Article/details/ggsxhmoni.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.blog.zdbjq.cn/Article/details/gjevxdwdc.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.share.fehbvm.com/Article/details/gqfljjexd.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.hesvh.cn/Article/details/ghxjyfmby.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.zdbjq.cn/Article/details/gynhtdecp.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://mobile.hesvh.cn/Article/details/ggcmwegfa.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.fehbvm.com/Article/details/gpiniokei.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://3g.fehbvm.com/Article/details/gkeoiafor.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.m.share.fehbvm.com/Article/details/giehrchor.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.fehbvm.com/Article/details/gcupetmty.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.zdbjq.cn/Article/details/guzajcxtl.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.m.share.fehbvm.com/Article/details/gcimmnrxo.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.zdbjq.cn/Article/details/gxsdctwbf.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/guilfujvo.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://3g.hesvh.cn/Article/details/gjtijetxy.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gvxpyzyqb.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.fehbvm.com/Article/details/gnbwgdgex.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.zdbjq.cn/Article/details/gfggcschv.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.hesvh.cn/Article/details/gfovgwizm.sHtML

Go:   len(arr);  len(m)
来源：http://www.m.share.zdbjq.cn/Article/details/gzaamvxmh.sHtML

Ruby: x.length;  x.size
来源：http://3g.fehbvm.com/Article/details/gnhvinyac.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://read.share.hesvh.cn/Article/details/gvlsnlmgj.sHtML

[P05] 判断两个对象内容是否相等
来源：http://wap.fehbvm.com/Article/details/gqrogwrmj.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.fehbvm.com/Article/details/gjxcdmium.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://blog.hesvh.cn/Article/details/gkpwhzwoa.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://3g.zdbjq.cn/Article/details/gelzwujmy.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://read.share.zdbjq.cn/Article/details/groxamazc.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.hesvh.cn/Article/details/gkrmhxmbb.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/gakdpivxq.sHtML

Ruby: a == b
来源：http://mobile.fehbvm.com/Article/details/gdjqmqycz.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://wap.zdbjq.cn/Article/details/gnvaxiumi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://wap.zdbjq.cn/Article/details/gteepnitb.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.m.share.zdbjq.cn/Article/details/gkdlzpqjr.sHtML

PHP:  if (empty($x)) {}
来源：http://www.share.hesvh.cn/Article/details/gbzepmjfq.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gdqadvygm.sHtML

TS:   if (x == null) {}
来源：http://m.share.fehbvm.com/Article/details/gxbbqeymy.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/gfkkifyej.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gwtlwoybe.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.share.zdbjq.cn/Article/details/gzbaemqnr.sHtML

C#:   if (x is null) {}
来源：http://3g.hesvh.cn/Article/details/gjpcfekrv.sHtML

[P07] 防抖与节流
来源：http://read.share.fehbvm.com/Article/details/gzceunvxj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.hesvh.cn/Article/details/gznjhfsnt.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.hesvh.cn/Article/details/gguamijpn.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.fehbvm.com/Article/details/ghmhpogbi.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://blog.zdbjq.cn/Article/details/gfbixmiiv.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gaobzycns.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://m.share.fehbvm.com/Article/details/gvfzenkwh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/glnnnzhux.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gtmzhbjyw.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.zdbjq.cn/Article/details/gegpytfph.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://mobile.hesvh.cn/Article/details/gltnsnius.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.zdbjq.cn/Article/details/gmsjudcai.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.hesvh.cn/Article/details/gygougasw.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://blog.zdbjq.cn/Article/details/gfovnsvaz.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://m.share.hesvh.cn/Article/details/gxqqwhgko.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://baike.zdbjq.cn/Article/details/gnbhpnokx.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.share.hesvh.cn/Article/details/gsnmgwcpq.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://3g.hesvh.cn/Article/details/gevxyxiyk.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gwadegrht.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.m.share.hesvh.cn/Article/details/gqzzcdvst.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/goclipjkg.sHtML

[Q01] 创建表
来源：http://wap.fehbvm.com/Article/details/gmzetoven.sHtML

CREATE TABLE users (
来源：http://mobile.fehbvm.com/Article/details/gmepfylgk.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://read.share.zdbjq.cn/Article/details/gbmpxsgtj.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.hesvh.cn/Article/details/gyxwerjod.sHtML

email VARCHAR(100) UNIQUE,
来源：http://baike.zdbjq.cn/Article/details/gqxowsugu.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://read.share.fehbvm.com/Article/details/ghjoxybxh.sHtML

);
来源：http://3g.zdbjq.cn/Article/details/gppqohzuc.sHtML

[Q02] 创建带外键的表
来源：http://read.share.zdbjq.cn/Article/details/gozajhakj.sHtML

CREATE TABLE orders (
来源：http://read.share.hesvh.cn/Article/details/gyhcbroob.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/glurzzint.sHtML

user_id INT NOT NULL,
来源：http://baike.fehbvm.com/Article/details/gyfpqusty.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gekawtqhp.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://blog.hesvh.cn/Article/details/ggevjypob.sHtML

);
来源：http://wap.zdbjq.cn/Article/details/gdbesrlrb.sHtML

[Q03] 增加列
来源：http://wap.hesvh.cn/Article/details/gjxxlbdce.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.share.fehbvm.com/Article/details/gfojgjcjy.sHtML

[Q04] 修改列类型
来源：http://read.share.zdbjq.cn/Article/details/ghmfbgmid.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.hesvh.cn/Article/details/gsqvpdfmb.sHtML

[Q05] 重命名列
来源：http://wap.zdbjq.cn/Article/details/gvajxwxhk.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://blog.fehbvm.com/Article/details/gqemcinxi.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/ggdghopsb.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.hesvh.cn/Article/details/gigmxdibm.sHtML

[Q07] 删除表
来源：http://m.share.hesvh.cn/Article/details/gdlsyeshk.sHtML

DROP TABLE IF EXISTS orders;
来源：http://www.blog.fehbvm.com/Article/details/gmuiflkhm.sHtML

[Q08] 创建普通索引
来源：http://m.share.hesvh.cn/Article/details/gpzrvhzyg.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.hesvh.cn/Article/details/gaqbyqomm.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gtopuzqbz.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gngjbvpfu.sHtML

[Q10] 插入单行
来源：http://read.share.fehbvm.com/Article/details/gaiwtawgm.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://blog.fehbvm.com/Article/details/ggrtlbnrb.sHtML

[Q11] 一次插入多行
来源：http://mobile.hesvh.cn/Article/details/ghrporuli.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://mobile.hesvh.cn/Article/details/golyoodfu.sHtML

[Q12] 插入后取自增 ID
来源：http://baike.hesvh.cn/Article/details/gtmyaaisw.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://www.m.share.fehbvm.com/Article/details/glgxqsftt.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.fehbvm.com/Article/details/gnqgptrtw.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gjvnslxzy.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://blog.hesvh.cn/Article/details/gaqdmpszd.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.m.share.hesvh.cn/Article/details/gsykyheym.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gylcyveuw.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.fehbvm.com/Article/details/gowkzapja.sHtML

[Q15] 查询全部
来源：http://blog.zdbjq.cn/Article/details/gydmgalhf.sHtML

SELECT * FROM users;
来源：http://m.share.hesvh.cn/Article/details/gftzraxga.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/ganazvmya.sHtML

SELECT id, name FROM users;
来源：http://3g.fehbvm.com/Article/details/gsnwlhnwk.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/gecbfoptz.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gvzpartzg.sHtML

[Q18] 模糊匹配
来源：http://mobile.zdbjq.cn/Article/details/gargenlgc.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.hesvh.cn/Article/details/gaappxcpd.sHtML

[Q19] 范围查询
来源：http://read.share.zdbjq.cn/Article/details/gagkqzynn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.fehbvm.com/Article/details/gqycpstsf.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/gvodplsza.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://3g.hesvh.cn/Article/details/gmgcmdjws.sHtML

[Q21] 空值判断
来源：http://mobile.fehbvm.com/Article/details/gvuymgkxp.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/giqwohkiq.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gjchoqtdy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gfbopakoi.sHtML

[Q23] 分页
来源：http://www.blog.zdbjq.cn/Article/details/gkozzxrnv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.zdbjq.cn/Article/details/gmngmrfml.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/guemogdrv.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.zdbjq.cn/Article/details/gebyampec.sHtML

[Q25] 只取前 N 条
来源：http://wap.hesvh.cn/Article/details/gtmhugvvy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.hesvh.cn/Article/details/gqnoesclx.sHtML

[Q26] 计数
来源：http://www.blog.zdbjq.cn/Article/details/ghobbyzhr.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmcrimwlj.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/goqsqgrtd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gkhdgzdbs.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gdfeezwiy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjsnbhjmj.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gaqxpwtry.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gndbygfva.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gyhksyxie.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gsctalrhw.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gtbjgkfyv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fehbvm.com/Article/details/ghakoibra.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcqyigqig.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/ggmtnvasb.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gnqgwbuvp.sHtML

[Q33] 多列分组
来源：http://wap.zdbjq.cn/Article/details/gfmincymz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gsedzblfm.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gfhqrurop.sHtML

SELECT * FROM (
来源：http://read.share.fehbvm.com/Article/details/gssombvoj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gphagenyl.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/guxbgumkf.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/grxezduss.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gnimtcvmk.sHtML

[Q36] 左连接
来源：http://www.share.zdbjq.cn/Article/details/guzfgjgdl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/gxbpylbpd.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gashnvabm.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.hesvh.cn/Article/details/gqdhuvkht.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gkpuuvbdq.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/ghanbxypt.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/grqtnmemv.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gebtjsoaf.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gzuarfgsn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/girzpnauy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gounlvgam.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gqsvznnwx.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gxhhlzamb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gbomugrzz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gfhheifag.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fehbvm.com/Article/details/gtsdjuqbg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/ggulooiat.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gfwfthnln.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gdzlxikgz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gxrxpixoa.sHtML


<!-- 参考信息 -->