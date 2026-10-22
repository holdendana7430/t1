代发 wailian999

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wgtzeqot.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hljadzbg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2gssmlnqd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vszgxvek.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tsaeuute.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iynqfguy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2flpzrran.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2dczfqrer.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2hxpjsizx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2ihwbecni.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ahaopzct.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2osgkwjjq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2govlwjnx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2fvabcpbu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ngtxuspc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2yctqwuot.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kuzolxwy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2yjteullj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ehscegdb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2udxvtsyy.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jzytlgkr.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gjxfudwi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2oqqovdcg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ifpyxuoc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2wnqkbqtq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xqxifsfp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2emtngdeb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ygcdolbq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gdqjaeux.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bogpjfrw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zuthiobu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vnyqfmyn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gzwyoqkq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2kyjdnjzb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2aozoxbub.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xfedyoxa.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2smpfsbxr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ytgqvyok.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mjwvsljj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2wmhixldv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ikyalngv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kbfrverd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2zraecppi.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vriachxz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2chxrwlre.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xhpdsqdk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ffugoxyx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2egsonato.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2glpypulc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2claxhzpu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qfpisgkq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2drefphtn.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2xeivabyz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mxbbwtti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2riudvbfj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mxaowuse.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2dhxmnjzb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bohdkqks.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ahzcxhza.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vrhnmdrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbumtosi.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2murxqkkt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ydqebvvx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zyqkqkrm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2aswthqwy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jpgkojqz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2zuxqvkix.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2xhjytoyi.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tematdgm.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hsmlhiug.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dnwdugwy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lcnxhqjx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rbiyyott.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2cucpjphj.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2zmfioava.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2mgdnfsmp.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dfqzauxx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2datqmkav.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hfikjwni.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2stsybnle.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nkmvaibe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2kqevjzpo.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2gfwmsfeq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2elfxcrzd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2tjelampm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ezoodswg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nbdyxnpa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2nfigihkv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2wmkdvcic.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2womruqeq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2foeniqvr.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2rzwgmjvj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2cjnmszbi.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jfqfqrkd.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2pjuhjadi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2vnzxlhlt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cnnomfwl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2jbyryouy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2pevtwrqx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2eiejqpzz.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2bxaneykj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2xirhvwzv.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2znowbsaf.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vxkchvwk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2wowogbak.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2isjoesbb.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mitkdekd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2rpauvsvm.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2zagpnhjh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2ptwnimqd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2buorxnuo.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ilpbyfzd.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kltklbdr.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2wfllyacy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ersgnzcx.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2nuqslczo.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2pcapbakp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvllxbck.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2pxpvnznc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbybyjcw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2xlzzhndd.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2osohppaq.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2lfqxtjso.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jijlhazo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2rymzqdqc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bewdipyu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bhtsgbvv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rklampns.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2tqlzifhf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2ctknelhx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2gjmjbjey.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2acmjuxvg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2jdacmnqv.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2pmjvaxjt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mffyybhd.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ftnbpsdl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2sraovbij.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ycndvqsj.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xneoevbn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2yayjaczj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2tqzepmrk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oagznwfg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2tizbqljx.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ksiwecxj.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2keefrjud.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hxpfbdce.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2rbhaicyw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2knbfdhzq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2wefhwmlo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2acqiwhdi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pxtnstpl.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2qxydxzjh.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2opwbbhgy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2zhuxewpc.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2uifvobnw.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zsmaazqt.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ewdefnpo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2rryjhknc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2okysnyxr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dunwpurb.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2nywhispp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2glnxzupm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2duuzyudu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2qaelmhrg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2uvrrnaxt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2vhrkecbz.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2yxnupqix.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxghsjpy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2mpbmffrb.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pjztdumm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jsfgqpld.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2bukbzneg.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2hpghsqyu.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2wjfhtilp.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2whwcatqx.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2glmukxzx.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2evfdwnug.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tazahvzz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2gsxwbyji.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2ymkxpoff.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2hfjkpmra.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2wpamsmns.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2kmbwrdei.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2qcrdokqf.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2cwhjvdwi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2uxiqqsmi.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2zyxibhpr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kentrqui.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2uhegoopb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2plkuhfps.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2hdxfffto.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2gqelyhun.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bciislew.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2cdazpokh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2akouaujn.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dbtbrkbk.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2frjrvqsh.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2hmjodvlg.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2hedidddg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2xkfhyyas.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2hnrehvww.html

);
来源：http://www.52xcode.cn/Article/details/gt2pnrvnpps.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2yxsxiwno.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2maeuolkf.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sdybogyr.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2aoahpalf.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2fmtwkbtb.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2fhainuqt.html

);
来源：http://www.52xcode.cn/Article/details/gt2irgvevnh.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2vkysvosn.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2pdvgxvgm.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2uhvsoyhp.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2ynwejbra.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2fknlmlas.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2zgtlzwoy.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2ilhkpmjk.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2smzxtlex.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2plbykcbi.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ridtbfts.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2piswtkke.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2wmryyhmw.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2ufxweypg.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2uqjndbvz.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2ikizyumt.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2tjsmepsg.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2nvnctklf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2zgyfzwkp.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2mfpbikdq.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2wtdbhege.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2mtnthbxa.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2mswzmdkk.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2vdgyaybw.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2jyrdjtla.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2zhlpnmfj.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2flkxbzoj.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2twknhlqy.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wibobwft.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2clrwjglw.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ulbbkzjr.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2ldxrvypu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mjmbuyew.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2klowajnn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fpdlktnn.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2yzvkavoi.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2uepxdwxf.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2ixxjoajx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2yzjohjku.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2upvwfotu.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2qifpnffr.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2yvtvrgkq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2adwbbtsk.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2iiyggxns.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2kgifqdzm.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2gctdhgrv.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qauhhgjf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2lbbkjeaw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wfxywdjv.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2tqcejzeb.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fuqmowaf.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2qdqbuymp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2defjzfhw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rbuclapw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dhuerfzb.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2mjsnvkux.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjbkvdmu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2cnahlhon.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lphgqaey.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2iwqxagus.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2bpxeahhy.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rkszarqp.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gszzxhpa.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2wicdnnjv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2cimuqvnj.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2dxffkajr.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2cbwwrvau.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zzrlxcmc.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2vzpvepah.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yogaoups.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2uoamvvyw.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mgsgcoul.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2oivbfojq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aeyuxkep.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2iicvgvxd.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dqzayrgt.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2kjhfekyc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2btpxiyea.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kneckdrn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hkctgdhx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wuvktgpd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nploveei.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ibwlsojq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bwyaneim.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2xtyzgmvb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gwsujblj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ngnztbzp.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kabhbsaw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2wymtbdxt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bjnlikmi.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jntmvsob.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hbimspfu.html


<!-- 参考信息 -->