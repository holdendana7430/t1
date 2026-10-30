代发 wailian999

TS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/gwpdaquss.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gztabctrm.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gmxtaggno.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gryslcjal.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gppwujboo.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gmicyevsd.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gwxcfzupu.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/goksalfwn.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gtnlltxsc.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gnrikpxjy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.hesvh.cn/Article/details/ggvsgigly.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gztmipzqk.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gzdcsrzru.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gcyktckdr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gtmrfovlw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gqnueixon.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpwsjorau.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/gfccgsgpd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gvqtktaja.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gpvmebqky.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gzrobbigw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/guwgxxikx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gobgyjzml.sHtML

Go:   slices.Sort(arr)
来源：http://3g.hesvh.cn/Article/details/gcckzmmrl.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gxyulasme.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/glnyahekv.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gchhzehmz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gmarmtkai.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.fehbvm.com/Article/details/gpczompqb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gkmbjzjat.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gsrwwimiw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gnlkeruxq.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gpoceimnp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gqnxxxwiu.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/govbniycb.sHtML

[N04] 斐波那契数列
来源：http://www.blog.zdbjq.cn/Article/details/gckleeeif.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gcgjcimdc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gbmsnfuhp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gyykozxbw.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gzpedkkgr.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/grdcgaiqv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/grdmyggsh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gzbuwckia.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gcckmalie.sHtML

[N05] 最大公约数
来源：http://read.share.fehbvm.com/Article/details/gtavrmkaj.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gkkvghnvj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/gbjkwowpc.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gnygkngsb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gkskbvgtr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gdsafkhfs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gycinvimv.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gsgkepxpr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gylawnfop.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/gdkexbqft.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/glndrtmah.sHtML

PHP:  $s === strrev($s);
来源：http://wap.hesvh.cn/Article/details/gehztrwtk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gsemgwxti.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gyejrisyj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gaghitifp.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/ghyxviyqo.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gzhtscnsy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gsvfidjvb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gzooirwbh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gsknuzdbx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gagadctvi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gmymqzewo.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.fehbvm.com/Article/details/gviofrsbu.sHtML

Java: // 手写 HashMap
来源：http://blog.fehbvm.com/Article/details/gsvthxdcx.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gtzirbdyq.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gefcfuxgp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/ghghourrr.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gskkhfvhb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gtaucopte.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gfkshoyvb.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gydoblgha.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gloigumvb.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gdryxlres.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/geynmqqzz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gqlytwnxe.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/guuqfdgyk.sHtML

[N09] 栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gpfsojhbq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/gjtnjernn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gukjdmxxe.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gybscsjor.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.zdbjq.cn/Article/details/ggoayyham.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gxsxolghb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gfjslltub.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gyansolqt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/ggulyypty.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gvpcfywbg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gwjbcrdzx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gskftzzgz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/gtombuohl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gzmrcacjs.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gekwotorg.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.hesvh.cn/Article/details/gykmzehle.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/ghsolutwi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.zdbjq.cn/Article/details/gazgzxqmx.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.zdbjq.cn/Article/details/gkzevazfy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gpagrswuj.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gggkohdlh.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gqfxekavo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gzogtnszo.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gtqgnutuq.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gtndloviq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gozwjfmho.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gbqvxltyb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.zdbjq.cn/Article/details/gzdxwkoeq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gtzlhselj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/goykhthnj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gsnjslgfq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gmookmchp.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gbbkhpper.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gevfcmwml.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdmynpng.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gbapjdhax.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ggtuaxzse.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gvwzvgufe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwxjkrfmx.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gqsbebumf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/gnvblxwyu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/giytxbgoj.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.hesvh.cn/Article/details/gwownfvty.sHtML

TS:   // 同 JS
来源：http://www.m.share.hesvh.cn/Article/details/gcmtelfob.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gwhvlkinv.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/ggkqwuygp.sHtML

Ruby: Thread.new { f }
来源：http://blog.zdbjq.cn/Article/details/ggelplnbz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gmbkvmyqr.sHtML

[O02] 使用线程池
来源：http://wap.hesvh.cn/Article/details/gybootgsq.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gcufnrveh.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.zdbjq.cn/Article/details/gupzwygxo.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gtqrjclwd.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gmegdztwb.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.hesvh.cn/Article/details/gvgmjousj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.zdbjq.cn/Article/details/gftgozpww.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://baike.zdbjq.cn/Article/details/gsojzgacs.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/grzpradck.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gkbyttrwg.sHtML

Py:   with lock: shared += 1
来源：http://read.share.hesvh.cn/Article/details/gqvzbzujt.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gtobabawu.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.hesvh.cn/Article/details/gbbyyimjw.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gwitrdfsz.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/ggzgsjvws.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.hesvh.cn/Article/details/gzbomfmjr.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.hesvh.cn/Article/details/gkcrjtkra.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gbtduauhh.sHtML

[O04] 定义异步函数并等待
来源：http://read.share.fehbvm.com/Article/details/gjqqehdlq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gqgroxgwk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.fehbvm.com/Article/details/gjdilwgnt.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.hesvh.cn/Article/details/gwmikppis.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gnbkyyynn.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://blog.fehbvm.com/Article/details/gurxzbxjq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gxlugtgof.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/gcfujrywo.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.hesvh.cn/Article/details/gfsefsnkt.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.m.share.zdbjq.cn/Article/details/ghgvsilzn.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/ggickkcwy.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gjbcvlkjw.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.hesvh.cn/Article/details/gantekekk.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gcgzwogeb.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://m.share.zdbjq.cn/Article/details/gumepicsy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.hesvh.cn/Article/details/gfzqckeve.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.hesvh.cn/Article/details/gkelivrjc.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.blog.zdbjq.cn/Article/details/gaejiyhtq.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gmiiqihne.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://baike.hesvh.cn/Article/details/gvthqbfad.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://3g.zdbjq.cn/Article/details/gvghntevw.sHtML

JS:   // child_process / cluster 模块
来源：http://read.share.fehbvm.com/Article/details/gblrmaanq.sHtML

TS:   // child_process / cluster 模块
来源：http://baike.fehbvm.com/Article/details/gjtnxazxy.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.hesvh.cn/Article/details/gtfpseorj.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.share.zdbjq.cn/Article/details/gjfgmohbq.sHtML

Ruby: // fork 块
来源：http://m.share.fehbvm.com/Article/details/gpggdptbl.sHtML

C#:   Parallel.For
来源：http://blog.zdbjq.cn/Article/details/gghntkuvc.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghvralxvv.sHtML

P. 常用工具函数
来源：http://read.share.hesvh.cn/Article/details/gxmpzcrzd.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gizjncvld.sHtML

[P01] 生成 UUID
来源：http://www.share.hesvh.cn/Article/details/gaumpgqmf.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gmadrhxhw.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gwgohtdkg.sHtML

JS:   crypto.randomUUID()
来源：http://www.share.zdbjq.cn/Article/details/gkenphdqo.sHtML

TS:   crypto.randomUUID()
来源：http://3g.fehbvm.com/Article/details/gisfgtieu.sHtML

Java: UUID.randomUUID().toString()
来源：http://3g.hesvh.cn/Article/details/gtuajlake.sHtML

Go:   // 用 github.com/google/uuid
来源：http://m.share.zdbjq.cn/Article/details/gzteiqfys.sHtML

Ruby: SecureRandom.uuid
来源：http://baike.hesvh.cn/Article/details/gscxngkji.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.zdbjq.cn/Article/details/geizkrfcm.sHtML

[P02] MD5 / SHA256 摘要
来源：http://blog.hesvh.cn/Article/details/gspadkugx.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.hesvh.cn/Article/details/gzyktwekp.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgrqxwbh.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gllbcrjuh.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.fehbvm.com/Article/details/gkhoykoic.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gfqjgnjyr.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://mobile.fehbvm.com/Article/details/gwuqmtppj.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/gxgxpxeva.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.hesvh.cn/Article/details/gkufbetho.sHtML

[P03] 生成短随机字符串
来源：http://mobile.fehbvm.com/Article/details/gadedwstn.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.hesvh.cn/Article/details/gtabcvqal.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.fehbvm.com/Article/details/grvgnbcid.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.fehbvm.com/Article/details/grjbukjog.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://mobile.zdbjq.cn/Article/details/gqmtqlqmd.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://blog.fehbvm.com/Article/details/gmvnprcwz.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://baike.fehbvm.com/Article/details/gnxehmljh.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://m.share.hesvh.cn/Article/details/gtlmidqpz.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://m.share.zdbjq.cn/Article/details/gdgsbvgro.sHtML

[P04] 求长度
来源：http://baike.fehbvm.com/Article/details/grftlcvar.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/gjthpetvk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gtfozjvya.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.share.hesvh.cn/Article/details/gikxbzmyg.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.hesvh.cn/Article/details/gmhkzynke.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gntqbyuwy.sHtML

Go:   len(arr);  len(m)
来源：http://read.share.zdbjq.cn/Article/details/gqrjigjbv.sHtML

Ruby: x.length;  x.size
来源：http://www.share.fehbvm.com/Article/details/gqnnamkrv.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gtmttmcmi.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.share.hesvh.cn/Article/details/gvvkerucd.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://mobile.zdbjq.cn/Article/details/gnzxbstot.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.m.share.hesvh.cn/Article/details/gsjkmogbd.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.share.hesvh.cn/Article/details/gwdcexlir.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gijojeygo.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.m.share.zdbjq.cn/Article/details/gmringqcr.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.fehbvm.com/Article/details/gybhxlctn.sHtML

Ruby: a == b
来源：http://m.share.hesvh.cn/Article/details/gahssqzzg.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gegxwoeug.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.hesvh.cn/Article/details/gozmyxhle.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://mobile.fehbvm.com/Article/details/givlddnfb.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gjebepard.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://blog.fehbvm.com/Article/details/gybwggazu.sHtML

TS:   if (x == null) {}
来源：http://www.m.share.fehbvm.com/Article/details/gmmhcvqkc.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gygtxapue.sHtML

Go:   if x == nil {}
来源：http://www.m.share.zdbjq.cn/Article/details/gppoaabpw.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://wap.zdbjq.cn/Article/details/gbzrfinzb.sHtML

C#:   if (x is null) {}
来源：http://blog.zdbjq.cn/Article/details/gumjqbmpt.sHtML

[P07] 防抖与节流
来源：http://www.share.hesvh.cn/Article/details/gfksvynnk.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://m.share.zdbjq.cn/Article/details/gaviktmjp.sHtML

PHP:  // 手写时间戳比较
来源：http://read.share.fehbvm.com/Article/details/gwttebhqu.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/gdwkjeezq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://3g.hesvh.cn/Article/details/goumxbmpz.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.blog.hesvh.cn/Article/details/gudfqcatz.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gtiyzkxkb.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://3g.zdbjq.cn/Article/details/gewwsbnvs.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://blog.hesvh.cn/Article/details/gxtegyqof.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gapsawwga.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://3g.hesvh.cn/Article/details/gmkkzvpxs.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.share.hesvh.cn/Article/details/gohtrcdgs.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.m.share.fehbvm.com/Article/details/grqbsiboc.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://3g.fehbvm.com/Article/details/geawmfhib.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://blog.zdbjq.cn/Article/details/ggfnrkzdj.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.m.share.zdbjq.cn/Article/details/gdrflbbap.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.fehbvm.com/Article/details/gzvoissxu.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.m.share.zdbjq.cn/Article/details/gmshoolig.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzecsurxs.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://wap.hesvh.cn/Article/details/gtmjannmu.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gchzzuoja.sHtML

[Q01] 创建表
来源：http://blog.zdbjq.cn/Article/details/ghoktkuro.sHtML

CREATE TABLE users (
来源：http://blog.zdbjq.cn/Article/details/gqaegxqqo.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gytxiidac.sHtML

name VARCHAR(50) NOT NULL,
来源：http://wap.zdbjq.cn/Article/details/gnvaspyjv.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.hesvh.cn/Article/details/gkwwoquev.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.hesvh.cn/Article/details/gotnxagcc.sHtML

);
来源：http://blog.fehbvm.com/Article/details/gwblfkpjd.sHtML

[Q02] 创建带外键的表
来源：http://wap.zdbjq.cn/Article/details/ghqaiakxo.sHtML

CREATE TABLE orders (
来源：http://wap.zdbjq.cn/Article/details/ghibmlner.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gyabheqts.sHtML

user_id INT NOT NULL,
来源：http://www.blog.fehbvm.com/Article/details/gqqrczlsk.sHtML

amount DECIMAL(10, 2),
来源：http://mobile.fehbvm.com/Article/details/gxffqelvv.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.m.share.hesvh.cn/Article/details/gmfnfxpwo.sHtML

);
来源：http://wap.hesvh.cn/Article/details/gnzpprnia.sHtML

[Q03] 增加列
来源：http://read.share.fehbvm.com/Article/details/gaxbuxzvv.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/grhlgxsuf.sHtML

[Q04] 修改列类型
来源：http://www.share.hesvh.cn/Article/details/gssebgith.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.m.share.hesvh.cn/Article/details/geuwotdgh.sHtML

[Q05] 重命名列
来源：http://read.share.zdbjq.cn/Article/details/gegnphzjc.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://m.share.fehbvm.com/Article/details/grpyozuji.sHtML

[Q06] 删除列
来源：http://baike.zdbjq.cn/Article/details/gmfqzbngr.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://wap.zdbjq.cn/Article/details/ggrjwsayu.sHtML

[Q07] 删除表
来源：http://baike.fehbvm.com/Article/details/gwwmkergi.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.zdbjq.cn/Article/details/gdbofpvva.sHtML

[Q08] 创建普通索引
来源：http://read.share.zdbjq.cn/Article/details/gqtotedse.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://read.share.fehbvm.com/Article/details/gefebvwqn.sHtML

[Q09] 创建唯一索引
来源：http://www.share.hesvh.cn/Article/details/gwxeermni.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://baike.hesvh.cn/Article/details/gwnvkmdgz.sHtML

[Q10] 插入单行
来源：http://read.share.zdbjq.cn/Article/details/gtlpqfhoj.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.blog.hesvh.cn/Article/details/gngnqlshh.sHtML

[Q11] 一次插入多行
来源：http://www.share.fehbvm.com/Article/details/gbvzveksr.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://3g.fehbvm.com/Article/details/gwkpyfwwc.sHtML

[Q12] 插入后取自增 ID
来源：http://www.m.share.zdbjq.cn/Article/details/gdltkofsn.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://baike.hesvh.cn/Article/details/gqomlqvpz.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://wap.hesvh.cn/Article/details/gfkvkzkpn.sHtML

[Q13] 忽略重复插入
来源：http://m.share.fehbvm.com/Article/details/gzfevgswx.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://m.share.hesvh.cn/Article/details/gqawoprys.sHtML

[Q14] 存在则更新（upsert）
来源：http://www.share.zdbjq.cn/Article/details/gdvbfsbol.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.zdbjq.cn/Article/details/gaovjxeft.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://m.share.hesvh.cn/Article/details/gxztulkdh.sHtML

[Q15] 查询全部
来源：http://mobile.fehbvm.com/Article/details/glhrgwtvs.sHtML

SELECT * FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ghhndsjsl.sHtML

[Q16] 查询指定列
来源：http://www.share.hesvh.cn/Article/details/gamvokaji.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gyufdajtc.sHtML

[Q17] 条件查询
来源：http://mobile.fehbvm.com/Article/details/greladdel.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.blog.hesvh.cn/Article/details/gobeeiohl.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gnqbnkvik.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.hesvh.cn/Article/details/gbehdzptj.sHtML

[Q19] 范围查询
来源：http://baike.hesvh.cn/Article/details/gmwtnlnaq.sHtML


<!-- 参考信息 -->