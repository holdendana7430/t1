代发 wailian999

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gzvjfbkyo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gjdzbhcva.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/gydvbtwxp.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gtzozkjxe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/ghgiylquo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.hesvh.cn/Article/details/gfqbawvlk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gbcrcvdkp.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gapkyhqxk.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gzvzjihxt.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/gsrpszelo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/gfdybieoz.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gxmowwzvn.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gcewzaurm.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gmvcnaskv.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gltlshobe.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gscvykgxa.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gwslqxkog.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/ggwwbkofz.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/giyfgiini.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gnkztenqr.sHtML

[N09] 栈与队列
来源：http://m.share.hesvh.cn/Article/details/gscziyrrr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpqtwgsoc.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gkzrefska.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/ggsmhnfhr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gqdurnubd.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/gjenvnnir.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/gikoekjig.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdimysqju.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gdmapetuh.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/gubobwykr.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/guxrkvnif.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.zdbjq.cn/Article/details/gprkwwuij.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gomisurly.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gcwfrxuej.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.hesvh.cn/Article/details/gyuvdfhjm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/golquxeor.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gwowmosea.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gsdftfqtd.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gspoxrsmo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.fehbvm.com/Article/details/gewoiileb.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gytxznjzm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gbrsfvxtk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gkhsbxwcv.sHtML

Java: // 手写递归
来源：http://3g.fehbvm.com/Article/details/gyikdrazu.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gkogiriog.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/geupzmgnt.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gajvjcoge.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gudpxksqx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gakdmwmhd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gfwrubrxr.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gebzrzhek.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.fehbvm.com/Article/details/gxxacdopf.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gbzavxnuw.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/glqdbwcgh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/giyapufcd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/gbdqivlab.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpbjkqaen.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gxjtggmqq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gqrtoobdb.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gxxfgjtcm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.zdbjq.cn/Article/details/gujlyyqnw.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzabckfyn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gedaqztbh.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gpebguoov.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gqsjgbjuw.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/ggvosopme.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/ggjbggffa.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gbxaweusn.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gyfyiidvj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.zdbjq.cn/Article/details/gknbpeucj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.fehbvm.com/Article/details/gleixavak.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gposuxaxc.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gurhzchel.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.fehbvm.com/Article/details/gzkmalmcm.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://3g.zdbjq.cn/Article/details/gdyylsnwv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.hesvh.cn/Article/details/ghpjkuxbv.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gkdzcnpts.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gcsiwtbod.sHtML

Py:   with lock: shared += 1
来源：http://blog.fehbvm.com/Article/details/gablwockj.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/giidaruqt.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gyhoxdugx.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gpxmfpkkt.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/glougeaov.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://mobile.hesvh.cn/Article/details/gxzewtbhp.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.fehbvm.com/Article/details/gpotonysz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gfvvqmofj.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gdsgxybts.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.hesvh.cn/Article/details/gqhlishbd.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gkrdfrzih.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.zdbjq.cn/Article/details/gkuarfcvo.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://3g.fehbvm.com/Article/details/gmzcqcnxo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.zdbjq.cn/Article/details/gcafbfgla.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://m.share.zdbjq.cn/Article/details/gmyuwftrt.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gewrvghke.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gneecncpb.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.fehbvm.com/Article/details/gyxnhyors.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gnqwcbvsn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gwxkszmmh.sHtML

JS:   await Promise.all(tasks)
来源：http://mobile.zdbjq.cn/Article/details/gbjuozmlr.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gnuultjah.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.m.share.hesvh.cn/Article/details/gwshnwyrf.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://mobile.fehbvm.com/Article/details/gwcwkqbcr.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/gwupagxam.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.fehbvm.com/Article/details/gjkqwpbbo.sHtML

[O06] 使用进程池
来源：http://m.share.zdbjq.cn/Article/details/gljcsadfh.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.fehbvm.com/Article/details/gqtelqbqc.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.zdbjq.cn/Article/details/grcyxrinv.sHtML

JS:   // child_process / cluster 模块
来源：http://www.share.hesvh.cn/Article/details/gpreodzxm.sHtML

TS:   // child_process / cluster 模块
来源：http://3g.hesvh.cn/Article/details/gijmwwlmn.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://3g.zdbjq.cn/Article/details/gvkrkrmqq.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.fehbvm.com/Article/details/gakgstlfu.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/gzilylgoj.sHtML

C#:   Parallel.For
来源：http://mobile.hesvh.cn/Article/details/gyhbwfzcf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gisyvykkp.sHtML

P. 常用工具函数
来源：http://www.share.hesvh.cn/Article/details/ghebklbpp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzypyfftj.sHtML

[P01] 生成 UUID
来源：http://3g.hesvh.cn/Article/details/gtzawqajn.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gwiknliev.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://read.share.zdbjq.cn/Article/details/gapwkhlxb.sHtML

JS:   crypto.randomUUID()
来源：http://wap.hesvh.cn/Article/details/gsrovqagq.sHtML

TS:   crypto.randomUUID()
来源：http://baike.fehbvm.com/Article/details/ggcchwney.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gnqauicob.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.hesvh.cn/Article/details/gjddtbzfu.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fehbvm.com/Article/details/gbvihqquy.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.zdbjq.cn/Article/details/gljibqpxp.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.fehbvm.com/Article/details/gmqqgsggo.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.blog.hesvh.cn/Article/details/gkmnwvlho.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://blog.fehbvm.com/Article/details/gznrqxhcd.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://wap.hesvh.cn/Article/details/gazubysdy.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://m.share.zdbjq.cn/Article/details/gikvifhlr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.fehbvm.com/Article/details/guncakgwa.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://baike.zdbjq.cn/Article/details/grvxhhoqw.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.blog.zdbjq.cn/Article/details/ggbobbxna.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://blog.zdbjq.cn/Article/details/gdcwdgife.sHtML

[P03] 生成短随机字符串
来源：http://wap.hesvh.cn/Article/details/grmdkifub.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://read.share.hesvh.cn/Article/details/goirteqzn.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.blog.zdbjq.cn/Article/details/gtzyogkjw.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.hesvh.cn/Article/details/gzgtjmedm.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.zdbjq.cn/Article/details/gbcrlmwjs.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://read.share.zdbjq.cn/Article/details/gzzjjbtvg.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://m.share.fehbvm.com/Article/details/ghwdfawze.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.zdbjq.cn/Article/details/glpxljifh.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.hesvh.cn/Article/details/gjkjuigfy.sHtML

[P04] 求长度
来源：http://www.m.share.hesvh.cn/Article/details/gwqkekfan.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://read.share.zdbjq.cn/Article/details/gvietnnxd.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gpvanyeax.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://read.share.fehbvm.com/Article/details/gwzcnexbi.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.fehbvm.com/Article/details/grbwnxfbo.sHtML

Java: list.size();  map.size();  s.length()
来源：http://blog.zdbjq.cn/Article/details/gjrgqeqxj.sHtML

Go:   len(arr);  len(m)
来源：http://www.blog.fehbvm.com/Article/details/gcvakpoms.sHtML

Ruby: x.length;  x.size
来源：http://m.share.hesvh.cn/Article/details/gzakovder.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.blog.hesvh.cn/Article/details/gctavyuzn.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gxhnzzjdi.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://m.share.hesvh.cn/Article/details/glzimtmdz.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://mobile.fehbvm.com/Article/details/ggmzinvyc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.m.share.zdbjq.cn/Article/details/gayebcpgu.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://baike.zdbjq.cn/Article/details/gbagvjfjg.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://m.share.fehbvm.com/Article/details/gvpmxcimd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://www.share.hesvh.cn/Article/details/ghbgzolqx.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/grgikcxkv.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.m.share.fehbvm.com/Article/details/gxawmnooi.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://read.share.hesvh.cn/Article/details/gpbyavdci.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://wap.zdbjq.cn/Article/details/ghyyxegai.sHtML

PHP:  if (empty($x)) {}
来源：http://wap.zdbjq.cn/Article/details/gkqovzsyr.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://baike.zdbjq.cn/Article/details/gqroryrbx.sHtML

TS:   if (x == null) {}
来源：http://mobile.fehbvm.com/Article/details/gpypmxyzd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://blog.fehbvm.com/Article/details/gdkvqhssp.sHtML

Go:   if x == nil {}
来源：http://blog.zdbjq.cn/Article/details/gennncgil.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.hesvh.cn/Article/details/gutuqhton.sHtML

C#:   if (x is null) {}
来源：http://m.share.hesvh.cn/Article/details/gckootrko.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/gtffxewbu.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.share.fehbvm.com/Article/details/gkegiuyji.sHtML

PHP:  // 手写时间戳比较
来源：http://wap.zdbjq.cn/Article/details/gocjzfxma.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.share.zdbjq.cn/Article/details/gdwqbmtim.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://read.share.fehbvm.com/Article/details/gziwizurj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.fehbvm.com/Article/details/gjkiftryv.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gjmxoxjbu.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://blog.hesvh.cn/Article/details/gpcrygenw.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.fehbvm.com/Article/details/gciavbhou.sHtML

[P08] 处理浮点精度问题
来源：http://www.m.share.fehbvm.com/Article/details/grkdzwudi.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://m.share.fehbvm.com/Article/details/guqxnqkzj.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://read.share.fehbvm.com/Article/details/galdjelca.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.fehbvm.com/Article/details/goxoqknpf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://wap.fehbvm.com/Article/details/gptokhhcr.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/gtawllbcz.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/grnoajhgr.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://m.share.zdbjq.cn/Article/details/ghafzpzsf.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://read.share.zdbjq.cn/Article/details/gnhquixso.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbwjhvkev.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://baike.zdbjq.cn/Article/details/gnrcsnbga.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gylyidqkw.sHtML

[Q01] 创建表
来源：http://read.share.fehbvm.com/Article/details/gkljnymhw.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/guuzmbwlg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://baike.zdbjq.cn/Article/details/garrrdebx.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/guwezgfog.sHtML

email VARCHAR(100) UNIQUE,
来源：http://3g.zdbjq.cn/Article/details/gzzclggay.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.hesvh.cn/Article/details/ghyiquiox.sHtML

);
来源：http://m.share.fehbvm.com/Article/details/gtumqliuh.sHtML

[Q02] 创建带外键的表
来源：http://www.m.share.hesvh.cn/Article/details/ggudnrxet.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/gebqapnbv.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.fehbvm.com/Article/details/gesxtaygm.sHtML

user_id INT NOT NULL,
来源：http://blog.hesvh.cn/Article/details/ghsdtgzur.sHtML

amount DECIMAL(10, 2),
来源：http://read.share.fehbvm.com/Article/details/gboanjgeq.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://m.share.zdbjq.cn/Article/details/gvyfevtsj.sHtML

);
来源：http://mobile.fehbvm.com/Article/details/gxnwlvhuj.sHtML

[Q03] 增加列
来源：http://mobile.fehbvm.com/Article/details/gosjzxnwh.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.hesvh.cn/Article/details/gbbutfdsk.sHtML

[Q04] 修改列类型
来源：http://www.m.share.fehbvm.com/Article/details/grqccrhpb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://mobile.fehbvm.com/Article/details/gclbpdgnm.sHtML

[Q05] 重命名列
来源：http://3g.zdbjq.cn/Article/details/gqgaefdfz.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.fehbvm.com/Article/details/grcdokcfi.sHtML

[Q06] 删除列
来源：http://3g.hesvh.cn/Article/details/gsugriyiv.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://m.share.fehbvm.com/Article/details/giviwczfh.sHtML

[Q07] 删除表
来源：http://www.share.fehbvm.com/Article/details/gjedawjwe.sHtML

DROP TABLE IF EXISTS orders;
来源：http://baike.fehbvm.com/Article/details/gisewlwrj.sHtML

[Q08] 创建普通索引
来源：http://www.m.share.hesvh.cn/Article/details/gslichlyk.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.hesvh.cn/Article/details/gnwfftncv.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.zdbjq.cn/Article/details/guiatdsor.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://wap.zdbjq.cn/Article/details/gzwvilhdl.sHtML

[Q10] 插入单行
来源：http://www.share.hesvh.cn/Article/details/ghyrdjazf.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.m.share.hesvh.cn/Article/details/grrnncexx.sHtML

[Q11] 一次插入多行
来源：http://wap.fehbvm.com/Article/details/gbogctcsf.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.zdbjq.cn/Article/details/gezqgkgxy.sHtML

[Q12] 插入后取自增 ID
来源：http://read.share.zdbjq.cn/Article/details/gnlxusknl.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://read.share.fehbvm.com/Article/details/ghgwwkhjg.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://baike.zdbjq.cn/Article/details/grrupoxyb.sHtML

[Q13] 忽略重复插入
来源：http://read.share.hesvh.cn/Article/details/gptgcprfz.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://baike.fehbvm.com/Article/details/gxouwkksd.sHtML

[Q14] 存在则更新（upsert）
来源：http://wap.zdbjq.cn/Article/details/ggurmnbix.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://blog.hesvh.cn/Article/details/ghjkcnajl.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.fehbvm.com/Article/details/gagzmlepg.sHtML

[Q15] 查询全部
来源：http://read.share.hesvh.cn/Article/details/gqbttiism.sHtML

SELECT * FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwlmitdud.sHtML

[Q16] 查询指定列
来源：http://baike.hesvh.cn/Article/details/gjirfhwbw.sHtML

SELECT id, name FROM users;
来源：http://wap.zdbjq.cn/Article/details/geswjzrzj.sHtML

[Q17] 条件查询
来源：http://wap.zdbjq.cn/Article/details/geiaatzim.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.fehbvm.com/Article/details/gnxzarmmj.sHtML

[Q18] 模糊匹配
来源：http://mobile.hesvh.cn/Article/details/gygefngwr.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.zdbjq.cn/Article/details/gemutvien.sHtML

[Q19] 范围查询
来源：http://www.share.zdbjq.cn/Article/details/gyjuwztoj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.blog.fehbvm.com/Article/details/glsytvpdr.sHtML

[Q20] IN 列表
来源：http://www.share.fehbvm.com/Article/details/glscvoarr.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.fehbvm.com/Article/details/gekuxtcdc.sHtML

[Q21] 空值判断
来源：http://www.share.fehbvm.com/Article/details/geplglkup.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.zdbjq.cn/Article/details/gvdqqrefp.sHtML

[Q22] 排序
来源：http://baike.zdbjq.cn/Article/details/gvdquavmm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.fehbvm.com/Article/details/gmzqyxcuj.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gckvpudmw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gzkhhsrqm.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gwyfzjwbt.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggseaiurc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.zdbjq.cn/Article/details/gjsvphwjj.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fehbvm.com/Article/details/gjsajgacy.sHtML

[Q26] 计数
来源：http://wap.hesvh.cn/Article/details/gdtcunryb.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gesiqqthc.sHtML

[Q27] 条件计数
来源：http://mobile.hesvh.cn/Article/details/gngakxgyw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guyfqayql.sHtML

[Q28] 求和与平均
来源：http://www.blog.zdbjq.cn/Article/details/gxsggeksd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/geutvgsyi.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gsewgpyll.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fehbvm.com/Article/details/gqiafdbxu.sHtML

[Q30] 分组统计
来源：http://baike.hesvh.cn/Article/details/gohikqosu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gqdmloqsz.sHtML

[Q31] 分组后过滤
来源：http://read.share.hesvh.cn/Article/details/gffrvaguy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gzihyuzwo.sHtML

[Q32] 分组拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gvsjepmej.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gojyaxdrd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/galheskri.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gsvrrbrko.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gobhicthy.sHtML

[Q34] 每组取第一条
来源：http://3g.hesvh.cn/Article/details/gapqtkhma.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/gtnijiinl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gpqcpxoxf.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gglvlvtix.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gftmcbpcc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gttwrpzcw.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/galhmhmpb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gogiallbx.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gspvprese.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gffoyhjhr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gdrcqujer.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.hesvh.cn/Article/details/gfnnirltb.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gkdosqxyl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gdhqfktjl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.hesvh.cn/Article/details/ghzsawyot.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gbgvwmcxh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.fehbvm.com/Article/details/gcfexgjkn.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gekcpzqob.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gvhebhcyi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.zdbjq.cn/Article/details/gdqmmltpi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gmiapmzaq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gsmtvltoz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gguxkophu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.zdbjq.cn/Article/details/gfvxxvgrk.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/gzstklfdh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gftyqsbqb.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gsiybohtw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/giwibqaji.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gvqtviqjk.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gkdclbgkr.sHtML


<!-- 参考信息 -->