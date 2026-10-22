代发 wailian999

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ldmywnth.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2toaxajlp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2kjmykdcx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2sulzdeaz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2nttjkvcq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2smvmbwvk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2emyvwyod.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ezhoxcfx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tgtxfrkt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wurtbwhq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ixmzwlgi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojratglf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hxtpqxes.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vowklfbb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2otrktivo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zzijfflh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ixeziiul.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2muaqshig.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kyxogmmi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2llfbiurh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2novikste.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ksagghbd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yjemrbuv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wvujftym.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mlvwkrjr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wbzljbpu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2cfebaqck.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bawvpfee.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2wyvgagxj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2cthehgcg.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lwhrmryd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2gbpyoreh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2iwswtczb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zhsovwvt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vhomimyd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pimomgks.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ndicoidx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pvvuxnyh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2dnqnccfr.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zlomkaaa.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2iyiwopgb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yixyrxxs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2awjgrrgj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cukxnudj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bnmuqigq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qojqvopk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nfqtliyp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nznpbfak.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2tfaqpjiy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2viyobnsw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2pmfugazf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mwuzysbv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmbvqmie.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2cxcrkrgj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xsbivekw.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2fonswqmc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2pksrnndt.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nvmjsnel.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ztzgtzwg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2obyuicys.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2xyzrvpys.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cijldihq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gfryprpz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qjyywlrp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zsatuicm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rtbyajwn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pyyxsbxq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2aoeybagg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jrpdqzeq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2lovmshvg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fhlisewb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2plvjrhcw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2htilhknt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2idqkeoea.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2pfurckhf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ebhibnsd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efooceud.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2zbwkdwvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifyrmrlq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qqrccxbg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jqdzvnaf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2pybewylf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fodmfxvk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vmykjyki.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xrbagtsn.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bfxrgeiu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vzqitibi.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2balpxzrn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2jaeabegl.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ykucteip.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gzepjomq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2siqidmza.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dugyrduf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2htsqsltt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bbqnnwla.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2uaaooeqb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2hogahjyw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2fbpfnhfm.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2iqiaxjkr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2qbddwaxp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ybcghddn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nzzhvrhv.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ffgluthw.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2yziinepj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2doldgxph.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dchoofjg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2kiiwphyo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2vsjomemv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2uggglsio.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qdfdcvbz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qfptbhpo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2xsbcyfpx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2cnejehmi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2miwfarze.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehkxzohh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fnygsurj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rsrfaogc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2abwztrfj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2zbboxlcj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2htkpjbkn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ytgbnkef.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2laaptbxm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2inhzttgx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2roajrozw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2mtugvipc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2hnugmatp.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rlqrtqbz.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ahrzsgsc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qpmporub.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2anrcamjg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gmedsrnn.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2djwczzsj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2qetzcokf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rccyrobu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2hornjstn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkgqqzrp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2gyfmwluf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2pkpouqdy.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nqgltlbz.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kxkhdecw.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2cmtvvaoo.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2hvjteogr.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2soqkduww.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2luqbwvto.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ptfoubau.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2bqpnxlaf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wqrzkcza.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ituevtxi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2qxxrnsvt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2llzjbheb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mkxhypqr.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2elqkgylu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wwqexdrp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2ngbhqcbf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czihyiqq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2qvgnzwlg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2koujqoqk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rztthohq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vqnyedft.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rjaoarvv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2dnanvivg.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2awpvayci.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2lslzobyy.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2gyjlrmww.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kienillk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qecwyidg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2lwwbgotv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yzhhzlhb.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fftjbmvp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2qkbveipt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2rqqpdwkj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vmkykcrz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2avlnwlhj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zazlrkdw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2csjreobj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2znvpplsu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2chwegrgn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wquhajuf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mzkbyotn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dsonztup.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2gnwywkfm.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2jbjgsgbv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2pvemevzq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uktobfwt.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2dlftwmgv.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zigcyxoe.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jkomzlmb.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2rmfeoflb.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2qxvrhimk.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2djgeqgxa.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2nhqxmszp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2savqcjlw.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2isivmrqn.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2yqxtypyf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2xlwospaz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2avdxnqez.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2pjygxzmc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2egyihrku.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2mieogiza.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2qrgurgkk.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2zdixjvns.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wrwjdcpy.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2dhthfqex.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2oeplafsr.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2djmkpmqy.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2hvuhggrb.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hjbhhmuv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2zeomapzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hdnyhxyy.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2bldstnht.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krhoyzkd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2cqyrfqos.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2pbvmpuui.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kntnvpjn.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2nktzesxl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2bmegvfxf.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fkjcvclp.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vsmmofag.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2elkcrliq.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2cmvzkbbh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2wdnejdct.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2jywllltd.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2zwkyjkxs.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2bjkpbqpg.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2gshgxqmn.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2prxrumgv.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2mdaigawg.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2hwfwpade.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2mekcnkiu.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2cqtqwgzz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2zosqxdyo.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2aejcyvnl.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2kletxdxh.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2iydmetut.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2xhzjtvwv.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2djicxlof.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2yfwftjxo.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2qgdepjfo.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ommdouaj.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2jnpepzro.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2fwkzihgu.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2bgtanypf.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2ixwjhzmu.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2izqcsofi.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ldxwgceo.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.52xcode.cn/Article/details/gt2rsccrnug.html

[Q13] 忽略重复插入
来源：http://www.ydjk.org.cn/Article/details/gt2aymzoxlw.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.52xcode.cn/Article/details/gt2kcfsezry.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2xiedswws.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt2etlxmgil.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2wwsdqhph.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2gvbbfjct.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mobafqly.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2iedeeyvp.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2earlgvco.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2mrocfdtm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2icerjton.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2yqhhupcq.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hctsdqde.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2lwlmhnny.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2emzipzse.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2sfboctks.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ammyawab.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2pwmlfuti.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2dhtijbkz.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2arruyiho.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2emogkzvy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2anwehocx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2dydgxevb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2xscswlnq.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2onmievde.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2fvvlzejq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2dosonycs.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ljzmxxen.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vawexvwy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ccwmiidn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tdgtgcbp.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2gyfmcmfu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xssdykad.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2amojojhf.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wuckggoi.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2gmudtxlj.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ughaztit.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ftapjvaf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dhqvbwrx.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vgafmivy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tnhnhkgy.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2klpdxnfr.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bgiaouls.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ipzishlb.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2iyddouov.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2zenesqzg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2jxaqbuei.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qutioskn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2hnfqhwap.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2zkgvmcqp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dcpjwnog.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ufslmcfz.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2aqsymfvm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2nfeglqhw.html


<!-- 参考信息 -->