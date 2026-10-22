代发 wailian999

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jnfhhvtw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2qsglunom.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2engbwzvt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lmgimcfn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rncxiwkj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zglboqco.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sfprhftx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2txgjslry.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xsomqpzm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2argdfrpr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2vecfyqgy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cwdblzxi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yiqyskvk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zpuhvdhr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2hmiqykzb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vczyqual.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2icojxczm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ucovivkh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ahipoegi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2junjemkc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uiybcpga.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2xlkqgxtv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lairdtsv.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2evowpwvu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rfunxyuk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2figcqlrn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kghoeynu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmlykxuu.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2iawunwfi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ukjyxymr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lnzucgis.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lhgfftgp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2wvelxfre.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pvsraozi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cxinbhri.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozptfftx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2hsozkrxg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vbbmqbwf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zuwqdsih.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xeezvppp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2rnwivtvp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ftzzvzju.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2iqlvtagx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jvzrgifc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zqkkuxhj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2djzntosy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pwqubnpd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2obwxqhks.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wpdhywfk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2azwtnjtm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rzowxlnf.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vggioqxz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vjjmepft.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vfagwvsk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yatpetob.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nchknqag.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2kiedjuyt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2qlfpvant.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ngdxiofp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2iexlhduk.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2slbqbsbd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nrkqdiem.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gdtmmtky.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gptoocly.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gavqivwx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2vcqtvqww.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wngumxcm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2pptkbyvv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2srkmjyca.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qqmabkdz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mhxlopah.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2xprivtyr.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2iwzvenrr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2admsvbmz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2sgtcktjk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2tjrbcmhm.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sgzjvozo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2homabonf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2oyueqytx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gkbioamo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vvvsnrze.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2kdhfdjqb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xrpvgltc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wwwdxdqw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2tqeceelw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2qymvbfun.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqghkbmz.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2worhndxa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ivwzqqnp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2oilgewgs.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2loxoiajs.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zsjywqmc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2awnundjz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2farxqwzq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2hzczugff.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2wjepzkon.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2dcoxfqmy.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qhhbmgoq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rovtfxze.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2wtmrprsa.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ileobgal.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2sawdinqb.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dfufxewm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2parlxmks.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zrmpfnex.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2txumqzte.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zcsycvll.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gytvghwk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2thpkpilu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wetpzlrs.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2klavbpvt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2ymczhdvc.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2nyegfkxx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2eboyxhch.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jnubdjqo.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2svihqyuu.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2wammdyeh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ydzloqxw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qzoaqvel.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2rpksouyh.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2uqaptlcq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpffnmuo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xqitfckz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bnmjybzn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2qnytmrbl.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dcjkqttr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bihxngpe.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ssobpwuf.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nrlvlnpz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kkrssocd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2eyorjmux.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xlhfwzst.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2miijkeno.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2cuudlpqv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2tydbyylz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2njepgxho.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zrxihowu.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ealsixyw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xmrqeunp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ljogqkiy.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2azjreugp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2vestekos.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xavqjeie.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2fwxiawzr.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rqlpqowi.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2szhtjxof.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yafcjnab.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2zvmvkhxj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2rjsxlywx.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bhhjjiob.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2mgulsiyt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2qpocqezt.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2fnjtuagh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xjfyjoyn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cjkkmdhc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dmpqjvwl.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mmkarmwx.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zktvuthi.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rskukwzu.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hxawjtlk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2icphxnqm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2sajjigqe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2eirwpogf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2nfhxuwbz.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2xyklorcg.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yucsvloy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2qnnuodsc.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2sapzrhnd.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zkbdndtj.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2hxihwafn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2dzxrkicg.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sllmihqp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2svpcvgue.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2bfsujljd.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zagvkqyn.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtddsoiy.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2zaqrqblq.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2ruoutqbp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2vyjalrpf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2xzlnsjqm.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2pbzaesjt.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2msinwkwr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2kolywhzk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2rafbqybj.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2udrwavkh.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2tvabkvon.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2cjxxpmsr.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2wxwmggoo.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2kkywskna.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rblnwomg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2iynwjnae.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2daarkhim.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2gadngnpr.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2yzoznevp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2clfkdxzg.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2rknscuvo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrofdkph.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2uptdffze.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rcxgdmns.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2goeogbyq.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2ahogilpt.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2poqsskpq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2zkiuzxtm.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2yoailklm.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2xnjowdnn.html

);
来源：http://www.52xcode.cn/Article/details/gt2avriiduj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2zavgecta.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2rgjuaegy.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2yynvnpdw.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2udhyojoj.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2acdqrogz.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2ytfgmdul.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mqaslwor.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2winuipjf.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2uvkgxvjm.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2llcehqzt.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2tnykaxva.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2jxpxsaib.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2opmseano.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2aojwtxft.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2qprjvnkb.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2mdqeocqu.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mpdsvjbv.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2lsborxgl.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2lxemgqnl.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2ezlrbcdb.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2dloeycax.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2wtffcdtc.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2kseskfyk.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2kmaqbqjz.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2wpejagie.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2tiamzory.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.ydjk.org.cn/Article/details/gt2womayaxp.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2omguqhfl.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2zoylhpea.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2mjtpwjwg.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2rhvcxwep.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2kdfdmesw.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2hqdrshse.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2yplkifph.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fhoqbknk.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2faexudxo.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvwimmkf.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2seqriohu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2hqbzebvf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tdwctcxd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2rnoudgcf.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2zojrhlzt.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2dbvvxcmk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fzlwhjan.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2wnwrjarc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2pewgljhj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2oyrwnlqc.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2fgpxlttm.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2zendrxkr.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2daeahval.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2rzxfpqdj.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2gkrgckpb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ziwfyrzq.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2gqdcvctv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2pozghenv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2tnebiigi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fwmqinfn.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2pxfehdve.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rucqkxwu.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2oshhiguh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eqvtgnsj.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zegsuyoc.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qqcxrrhp.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2huppncvg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cckbwqwi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zoyxibeo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lemzyaam.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kphrfiqw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2tfyhuzqp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2vymomvlc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2xfmktmpi.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mkjrrigb.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2lddqgims.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ghsnmomi.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jrcrrezq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2zxxngzpx.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qbvxrtnx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2targdwuj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2bvvghknh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ctafnvha.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fmcassav.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tmymqpos.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zktxyqmh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vgxceozx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cbetydar.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tlyevdpt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2gktqlasq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2gdcobadg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gqwdaono.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2fztprsch.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2chfeplak.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2kyxutufr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ezehcilw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2sdphoxtb.html


<!-- 参考信息 -->