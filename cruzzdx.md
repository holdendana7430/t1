代发 wailian999

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gtnwgqtax.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gfqhcaiaj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.hesvh.cn/Article/details/gqmarrrcz.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gvbfmstwo.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ghdhtyoud.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/gxtxkzseu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gwkjitach.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gagbbzuob.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/giaarcfve.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gebsjalsv.sHtML

N. 数据结构与算法
来源：http://www.share.fehbvm.com/Article/details/gsadtedpw.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gixgxraem.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gqiiggblb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gaypxobbv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxgrqdzfs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gkukuytjx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gkaedfrqd.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/grkhhukme.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gklegnkmt.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.zdbjq.cn/Article/details/ghoyfvrtv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gfzdnwcay.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gfoqakolp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/goapmntsh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/gegliktwg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gdmldatsa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/ggvemtaqv.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gohizbwmr.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/ghwtzhxzc.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gjasietlu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/guhlbyoju.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/ghbnunqkp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gawacgdby.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gzipskheu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gtzujgarb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/glgzmltcs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/glhqcgnkr.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.fehbvm.com/Article/details/gujbucaxb.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gchazgair.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/giwfatwae.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/grvqjjgxk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gttjkinfc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.fehbvm.com/Article/details/giozlpvuo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gubovgdlv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gbffrktku.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/grpynxyet.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gcrojomar.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gtjykybqg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gregjkxyh.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gqmplokob.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/ghezwwhxt.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gwrujcucj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/glrfzatck.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gszglbozc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/guduhsxwf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gewnqbuuv.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gngxlhjdj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gqeefinvb.sHtML

[N06] 判断回文字符串
来源：http://wap.hesvh.cn/Article/details/gzrjldbjj.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gkesbaiol.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gwqlbffhb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdvwupwvf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gpqnijwbi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gxkxalcdh.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gejmoavaa.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gcpfhbpbk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gnnfqmjbr.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gobfgyltk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gbvvjidax.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gwiiszkmt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.zdbjq.cn/Article/details/gtdbbszjl.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gvdpkddwu.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gyotbraze.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/gtqdsphkz.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gyydmrlib.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.hesvh.cn/Article/details/ghgzdnqyl.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gbsudsmdm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.hesvh.cn/Article/details/gdblavyek.sHtML

PHP:  // 手写递归交换
来源：http://read.share.hesvh.cn/Article/details/gfagtvbvy.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gqqrdgbdu.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gobcvhcho.sHtML

Java: // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gngitlphi.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/ghwmxilnj.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/garmoielp.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gkdxevgya.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gabiyrgow.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gzvvfmpts.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gfqqmgruk.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gmxipuuvs.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/guntafati.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gagvkvblw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gnwwggdwx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/guaszymzp.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fehbvm.com/Article/details/glxlgcntm.sHtML

[N10] 链表节点定义
来源：http://read.share.hesvh.cn/Article/details/gkykpltec.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gfpoayzfj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gmycdlaob.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.fehbvm.com/Article/details/gpqrstxqs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.zdbjq.cn/Article/details/gdvaobifu.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gtbxouhsd.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gczwvpisf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gfzqfxddr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkcfyygjd.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gzzktdyuk.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/gfmimgzjz.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gpapvwfej.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqmcmoztm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gbwumavdf.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gxpavtbnj.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/grpnjtwhw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gnborjual.sHtML

C#:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gasjktmjh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.hesvh.cn/Article/details/ghopyxmoh.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/glxfabotm.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/ggptdmgvw.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gjexlzajb.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/ghzfjnwlh.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gkryxgrhf.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/grzpwjbui.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gtqeuubum.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gfxlbtlxr.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ghgvliahe.sHtML

O. 并发与异步
来源：http://wap.zdbjq.cn/Article/details/gvbuishjf.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjetoliez.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gznawhfdx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gleipumxx.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/gnhnksomc.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gtqiwiwtx.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gmlfeupme.sHtML

Java: new Thread(() -> f()).start()
来源：http://blog.zdbjq.cn/Article/details/gweeidiiw.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gsgpfihsb.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gachlefxj.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gqqptpeim.sHtML

[O02] 使用线程池
来源：http://m.share.hesvh.cn/Article/details/ghemxhslb.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gxyagnzsv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/guqqsyauy.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gajsmtcec.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gjxbtwwzy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://baike.zdbjq.cn/Article/details/gghvfaskw.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://wap.hesvh.cn/Article/details/griqaetsc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/glldpxrqx.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://blog.hesvh.cn/Article/details/gnljpdiuw.sHtML

[O03] 加锁保护共享数据
来源：http://3g.zdbjq.cn/Article/details/gvszubsru.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gulzqhepv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.hesvh.cn/Article/details/gqaooulrz.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.hesvh.cn/Article/details/guygvxuml.sHtML

TS:   // 同 JS
来源：http://3g.zdbjq.cn/Article/details/grxlttyhj.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.hesvh.cn/Article/details/gtohoyboy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gryxoctmk.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gukjqwgzj.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.hesvh.cn/Article/details/gsakrshfe.sHtML

[O04] 定义异步函数并等待
来源：http://blog.hesvh.cn/Article/details/gtiqkjtvy.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.zdbjq.cn/Article/details/gpjqpwgog.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fehbvm.com/Article/details/gzcuatmar.sHtML

JS:   async function f() { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gcqwnuvug.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gviumbqhg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gotxbxjfz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.fehbvm.com/Article/details/grvklhymv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://mobile.hesvh.cn/Article/details/gjsxqhmvd.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gkzuyhbjo.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.hesvh.cn/Article/details/ghtxejmjo.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.zdbjq.cn/Article/details/gificqdex.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.fehbvm.com/Article/details/gfqzeygpg.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/glislluqv.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/grslvkeyl.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gwldiatwy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/ghlveaadk.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.zdbjq.cn/Article/details/goanvaoss.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.fehbvm.com/Article/details/gmoyggqhq.sHtML

[O06] 使用进程池
来源：http://mobile.hesvh.cn/Article/details/gxoknwjwu.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://m.share.hesvh.cn/Article/details/gzexxfqrl.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://wap.fehbvm.com/Article/details/gudskqkwg.sHtML

JS:   // child_process / cluster 模块
来源：http://m.share.fehbvm.com/Article/details/gogvaalgm.sHtML

TS:   // child_process / cluster 模块
来源：http://read.share.hesvh.cn/Article/details/guyrftoqx.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.fehbvm.com/Article/details/gjsajswwx.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://wap.zdbjq.cn/Article/details/gyrtgfdjl.sHtML

Ruby: // fork 块
来源：http://read.share.zdbjq.cn/Article/details/grbqbynca.sHtML

C#:   Parallel.For
来源：http://read.share.hesvh.cn/Article/details/gmytuxuhl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gcptbknfo.sHtML

P. 常用工具函数
来源：http://blog.zdbjq.cn/Article/details/gipvlvqji.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggzyofndz.sHtML

[P01] 生成 UUID
来源：http://wap.hesvh.cn/Article/details/gdtixtojy.sHtML

Py:   str(uuid.uuid4())
来源：http://www.share.fehbvm.com/Article/details/gbxstijra.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://mobile.fehbvm.com/Article/details/gpzhczgdo.sHtML

JS:   crypto.randomUUID()
来源：http://baike.hesvh.cn/Article/details/glwenhfve.sHtML

TS:   crypto.randomUUID()
来源：http://baike.zdbjq.cn/Article/details/ggdcwiyai.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gatqwqqts.sHtML

Go:   // 用 github.com/google/uuid
来源：http://blog.zdbjq.cn/Article/details/gurjasuxv.sHtML

Ruby: SecureRandom.uuid
来源：http://wap.fehbvm.com/Article/details/gsseihfro.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://wap.fehbvm.com/Article/details/gymqxpndt.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.zdbjq.cn/Article/details/gqwfdhnzj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://mobile.fehbvm.com/Article/details/gttywsfns.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.blog.hesvh.cn/Article/details/ggmgxptak.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.blog.zdbjq.cn/Article/details/gjfxbbezt.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://mobile.fehbvm.com/Article/details/gjrbtseje.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gughnhupx.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.m.share.hesvh.cn/Article/details/goazebugp.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fehbvm.com/Article/details/gljagcawq.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.zdbjq.cn/Article/details/gtbjnxxrn.sHtML

[P03] 生成短随机字符串
来源：http://www.share.fehbvm.com/Article/details/gdziytcgz.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://baike.zdbjq.cn/Article/details/guvsojacl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://m.share.hesvh.cn/Article/details/gehsjowcz.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://read.share.zdbjq.cn/Article/details/gbtmjmtgs.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://m.share.zdbjq.cn/Article/details/gkkdlhlyc.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://m.share.hesvh.cn/Article/details/gsxleqgzr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.m.share.hesvh.cn/Article/details/geoubqczy.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://3g.fehbvm.com/Article/details/gelxqabnw.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.blog.hesvh.cn/Article/details/gbvcackcw.sHtML

[P04] 求长度
来源：http://www.share.hesvh.cn/Article/details/gcbhcpxme.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://blog.zdbjq.cn/Article/details/giglkmrzb.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gylmsgsgl.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.m.share.zdbjq.cn/Article/details/gcvykjwnh.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gofhetsds.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.share.fehbvm.com/Article/details/goloiunyi.sHtML

Go:   len(arr);  len(m)
来源：http://3g.fehbvm.com/Article/details/gzzdggefw.sHtML

Ruby: x.length;  x.size
来源：http://3g.zdbjq.cn/Article/details/geicltlub.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://mobile.hesvh.cn/Article/details/gdqdizqif.sHtML

[P05] 判断两个对象内容是否相等
来源：http://read.share.hesvh.cn/Article/details/gidvdqvlz.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.zdbjq.cn/Article/details/gntfyguwh.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://baike.hesvh.cn/Article/details/gorzkplpc.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.blog.fehbvm.com/Article/details/ggbmwcflt.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://blog.fehbvm.com/Article/details/gcssljkvi.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://3g.fehbvm.com/Article/details/gilzlyzvu.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://baike.hesvh.cn/Article/details/givrgqpdm.sHtML

Ruby: a == b
来源：http://mobile.hesvh.cn/Article/details/gcnktecjs.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.blog.zdbjq.cn/Article/details/gpnplxmwu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://mobile.hesvh.cn/Article/details/gbxzcmqor.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.hesvh.cn/Article/details/guuembwom.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.zdbjq.cn/Article/details/gnxmuwjxf.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.share.hesvh.cn/Article/details/gnllvefaa.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/gvonmvddd.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gdfllidip.sHtML

Go:   if x == nil {}
来源：http://3g.hesvh.cn/Article/details/gkedogqze.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.blog.fehbvm.com/Article/details/gkhaooltg.sHtML

C#:   if (x is null) {}
来源：http://www.share.fehbvm.com/Article/details/gihhorjao.sHtML

[P07] 防抖与节流
来源：http://m.share.zdbjq.cn/Article/details/gwjbewwve.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://wap.fehbvm.com/Article/details/gfsrgvuhp.sHtML

PHP:  // 手写时间戳比较
来源：http://m.share.fehbvm.com/Article/details/gbgjeadve.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://m.share.hesvh.cn/Article/details/gbbpnozjq.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://wap.fehbvm.com/Article/details/ggcgcriba.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.m.share.fehbvm.com/Article/details/gbyrxhpby.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://wap.hesvh.cn/Article/details/gzrzwfedh.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.m.share.zdbjq.cn/Article/details/gydmqvzrc.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://read.share.hesvh.cn/Article/details/giftqwnww.sHtML

[P08] 处理浮点精度问题
来源：http://3g.hesvh.cn/Article/details/glvicwwmd.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.hesvh.cn/Article/details/getfjznpa.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.blog.zdbjq.cn/Article/details/gepaxwpxb.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.share.zdbjq.cn/Article/details/gargyyqiy.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.blog.fehbvm.com/Article/details/gwxtkgjps.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.share.fehbvm.com/Article/details/gmigmylqb.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://blog.zdbjq.cn/Article/details/gegmjghvh.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://mobile.zdbjq.cn/Article/details/gcjifbvis.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://m.share.zdbjq.cn/Article/details/gpofqiift.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gkzxstovt.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://read.share.hesvh.cn/Article/details/gbpzdlxcd.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gykivszoc.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gfshyebsw.sHtML

CREATE TABLE users (
来源：http://www.share.fehbvm.com/Article/details/gyymshvwl.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.blog.zdbjq.cn/Article/details/gioqrrncz.sHtML

name VARCHAR(50) NOT NULL,
来源：http://m.share.zdbjq.cn/Article/details/gnjxgjtmp.sHtML

email VARCHAR(100) UNIQUE,
来源：http://www.m.share.fehbvm.com/Article/details/gynyyvqmb.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.m.share.zdbjq.cn/Article/details/gcfrtqlal.sHtML

);
来源：http://3g.hesvh.cn/Article/details/gvrlkxftj.sHtML

[Q02] 创建带外键的表
来源：http://blog.hesvh.cn/Article/details/gkeqxeftn.sHtML

CREATE TABLE orders (
来源：http://3g.fehbvm.com/Article/details/gyhfjcrrh.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.fehbvm.com/Article/details/gpkotjwbi.sHtML

user_id INT NOT NULL,
来源：http://blog.fehbvm.com/Article/details/gorgccvfy.sHtML

amount DECIMAL(10, 2),
来源：http://m.share.fehbvm.com/Article/details/girlmbryj.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://mobile.fehbvm.com/Article/details/gblimmapl.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gwdozvllb.sHtML

[Q03] 增加列
来源：http://www.m.share.fehbvm.com/Article/details/gmgeyzoqm.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.m.share.fehbvm.com/Article/details/gqmlhiaua.sHtML

[Q04] 修改列类型
来源：http://mobile.zdbjq.cn/Article/details/ghkhqokpd.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.blog.fehbvm.com/Article/details/gerdgibni.sHtML

[Q05] 重命名列
来源：http://baike.hesvh.cn/Article/details/gmkklhifo.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.blog.zdbjq.cn/Article/details/gcbfcmwwt.sHtML

[Q06] 删除列
来源：http://www.m.share.zdbjq.cn/Article/details/gexfjguzl.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.zdbjq.cn/Article/details/gykbxpkyy.sHtML

[Q07] 删除表
来源：http://www.m.share.fehbvm.com/Article/details/gwjvunqsu.sHtML

DROP TABLE IF EXISTS orders;
来源：http://3g.zdbjq.cn/Article/details/gqllrtppc.sHtML

[Q08] 创建普通索引
来源：http://www.blog.hesvh.cn/Article/details/gbzgowskh.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://3g.zdbjq.cn/Article/details/gysvftzzz.sHtML

[Q09] 创建唯一索引
来源：http://www.m.share.fehbvm.com/Article/details/gchnkmoyx.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://3g.fehbvm.com/Article/details/ghvssonfb.sHtML

[Q10] 插入单行
来源：http://mobile.hesvh.cn/Article/details/gqhqnmxgh.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://baike.hesvh.cn/Article/details/gglgxusnp.sHtML

[Q11] 一次插入多行
来源：http://www.share.hesvh.cn/Article/details/gtctqfxhg.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gesfxohxb.sHtML

[Q12] 插入后取自增 ID
来源：http://www.share.hesvh.cn/Article/details/gpehshwsd.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://mobile.fehbvm.com/Article/details/grxnfhanq.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://blog.fehbvm.com/Article/details/gdrbugkgz.sHtML

[Q13] 忽略重复插入
来源：http://blog.fehbvm.com/Article/details/gudpfllpt.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://3g.fehbvm.com/Article/details/gvkmenljm.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.hesvh.cn/Article/details/gkbnivjdh.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://baike.zdbjq.cn/Article/details/gfotkjwso.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.blog.hesvh.cn/Article/details/gqlwmsubo.sHtML

[Q15] 查询全部
来源：http://www.share.hesvh.cn/Article/details/givvgprzq.sHtML

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxbfvxcum.sHtML

[Q16] 查询指定列
来源：http://www.blog.hesvh.cn/Article/details/gquvmxueu.sHtML

SELECT id, name FROM users;
来源：http://www.share.hesvh.cn/Article/details/gwqvcuboi.sHtML

[Q17] 条件查询
来源：http://m.share.fehbvm.com/Article/details/gwwkeeqsv.sHtML


<!-- 参考信息 -->