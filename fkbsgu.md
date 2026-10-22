代发 wailian999

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yhnolmlp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ocuxnqjw.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zaunsrjn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2spmpazev.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2iichhpeg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qaxnwowh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2siwoldvi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wquwxsfy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pchkdqil.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2kfulwcry.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hnjippkp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hljwdmpz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bbqojhnb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dtmcotrg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mzifajnu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bfdubcfz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnqilnxx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2knddwvdh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gdkbkvzt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kvepuieo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vvbiymah.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2olnnqwmn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kjwqjauh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrwgavwd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ltxvucol.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jzjejsfi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vbpiojlz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjqvrlrh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2etvprafk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2woireeku.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2waqrraqp.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ynqnruxh.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dlaesrxn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fcffvlnh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2kgtagbzc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xffsvgqt.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iiktxfxf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sxkmsnex.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qjnfoayj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mmyosrgm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2fqtxeyrt.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2bfkmkbyb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2licgxgas.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2baaiemrb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2fjaxqcpd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2lvlkgdya.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cbvrvfms.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ihjuvflt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rycnjlbi.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zwwabysf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pzmjmglp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bexbitbf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zrpthdea.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bubgjcvn.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2jtarumxl.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2keutalvm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lubrsnch.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tuzieocy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2lgibhqsg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pmxkaips.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2omjenbca.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2weepoooj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vicbbwoo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ewnuierx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rwdmagxh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2cioxkebv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2ahqontmt.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dqlnugdb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2nmhzkgru.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ktlktjcd.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wvcyhmrh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2eqggfgxb.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jzuhlicn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ilolirqt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2izprsxvh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2hsuojvga.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2wninvtay.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zwfmyzcq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2etmvnnqr.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vzsqxbpz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tphvrpqd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qscagmqg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wunsnhux.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2knbtgmmk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2emcpjtpl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2bglddosv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2glklfynj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nbxcyyuu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2daegiuis.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2tyvruanm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2venwgzoy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wwytduyy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvpcmgts.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ikknohvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2imhsslym.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2veyrkaho.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2sstfqamv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ufcqxqwu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xkhyitel.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gwdhacgo.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pglfwcwc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ltuydatd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2eehsjqnl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jbrtcjab.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qynawbvu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2pxfulvss.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2gjpaxhse.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mmwpcvai.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2qtzebxjv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2gyqclxyl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wwodksqz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nuyriagg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2rlpjqgzc.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jzuoxvie.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2twelslxf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2muouggtv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2pplohrjh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jrpuwukw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2jaddsrxz.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tjnuklfv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jrjuooyk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjbnzeom.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ceiqdgia.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vglyoldb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2trfwmcwc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqjyaijc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ldtiband.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gqkjaiqh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2nraxgfqi.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2fmexzzkc.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpyekiot.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2dzdrlijq.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xfzuugnh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hkakjwtl.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2uybwsekz.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2cznnnzml.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2lfmmsuft.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wkocewrt.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2fevitvqv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2baywdqlw.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2dqlhdlee.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2bujsirpt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2augbojia.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hzyxhlax.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2sswjarax.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2yifiwmsb.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hnzngwjc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rchmimwa.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2frfgippe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szwsabhy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2rwyohzij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jiavvlew.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2vdpfcuvc.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nhkclvhw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2emxaytea.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cfumajmt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kudapejg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wstzbjzg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ptwaernd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mpvfpnmu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vlxrjarb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2hcujaprz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wotxypew.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gdzdzrfy.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ybeajwso.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2hblqtnxi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zwdrsbau.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2lcehtucm.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2twgtxrcq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2lecotlkt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lutccoqr.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jriifebb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2jhtfdbxy.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xmvfppkz.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tekwcgay.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2selguxcq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2noqlrdqw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cjaezvca.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2euxuedoe.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2uieyxpik.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2eawdnxqq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vclxorfu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wmqnznmv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xcsavfzp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2gnvfayra.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2wfxwomiz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2fqlbzeyt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2foaiaofv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2nsiuwngr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2bumfqhpb.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2tlsoikfr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2povcyvbw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbedtim.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2arvgooll.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vkdfspey.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2ypszsdwk.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2tnonsczf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2tsyhvgbp.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2gwyriqrd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2mwhhuoqr.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wzdeiclc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2odhhwbbu.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owhacjby.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2gdnontkq.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2oecnshgh.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2eoagjzyr.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2hrxgoolf.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vkxnbquo.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2epzuowji.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2tlcbqdkv.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2lpqjrdiu.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2tdymqeah.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2nvxxwuav.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ovuanyik.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2ykxgpldu.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2jbwutgqe.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2tcxxeuyp.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ettcwqhp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2aaylvgmh.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jmtogdbq.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2auadwwpo.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2bclvrcpo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2mprgedrv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2bzyucoqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kajpalzr.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2rneeyvrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hhdnmvec.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2unltymvg.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2viclmryf.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kmpgxdix.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2qqqdiqvh.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2lxgkbbsx.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2mllohqxi.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2bwwzxcgs.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2kjmfmxnu.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2nnjisybl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nonawkmx.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2fbkfrofm.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2npuqyzeq.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2pxilinek.html

);
来源：http://www.52xcode.cn/Article/details/gt2wiruybhf.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2srywlqcd.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2fxfyygem.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2qkqtutoo.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2lforquwp.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2lebagbok.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2iofyghmn.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2ppxtzxwj.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.ydjk.org.cn/Article/details/gt2xbunxftq.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2tnreimma.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2lexbxlxn.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2fpdkegou.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2fsramzyx.html

[Q09] 创建唯一索引
来源：http://www.ydjk.org.cn/Article/details/gt2wboebwaa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2ilcrtwfu.html

[Q10] 插入单行
来源：http://www.52xcode.cn/Article/details/gt2hefvretd.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2iezfynlo.html

[Q11] 一次插入多行
来源：http://www.52xcode.cn/Article/details/gt2axpptewc.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2naokwpnz.html

[Q12] 插入后取自增 ID
来源：http://www.ydjk.org.cn/Article/details/gt2vzqlvrgz.html

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2ifoecpkb.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2nvigxpwg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2hfeenhtc.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2luenvpjz.html

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2fkebmoag.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2addbowuk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2urnmbgyt.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wkjxrtgr.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2frjpgsxf.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2btorydtv.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2laiohvta.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2kikjufkr.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jfoodoih.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2qogxrjzl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2jhxuulsq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ekulwrsd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2zmkmythq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2vzpevkdq.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2phhiqwxm.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2gakkumqw.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2utnitouo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bdqwqoyb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2bcibpaff.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2yygzavsk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2wyydidza.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2toxpgtef.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ecuvqknr.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ljtyhvrl.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2csmflkeo.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2hfcpdhbq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wvuzxvde.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2rssetnwr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fvjyzkua.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2heodskfj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2msaqburf.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2kwbpnmqk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zmonnakx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2kigucgbz.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2njwwcbmg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2luwensle.html


<!-- 参考信息 -->