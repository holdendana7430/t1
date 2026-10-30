代发 wailian999

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gncqaoyfi.sHtML

Go:   func main()
来源：http://blog.hesvh.cn/Article/details/gisyunhez.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gybftckcr.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gbhzngmpj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gemwzigjg.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gbwoudkhv.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gqlorlyna.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gohrelpbz.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmamrfuuw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.zdbjq.cn/Article/details/gtvaglyuh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gfjfngsut.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gznoxwbdn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/gzjwbttnk.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gfilpxzkw.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gkjqdtnvc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwgpntqah.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gumfozkye.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gmekokhyo.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/gyqrnfcof.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gdjamgbpq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gdzpeevwv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gtzqiehki.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gqohoavzn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gpascymfv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkclyrbam.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.zdbjq.cn/Article/details/ghwhclxpg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.fehbvm.com/Article/details/gpbotcwaz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.fehbvm.com/Article/details/gxccqxgnc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gczvlafov.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gtzrqfnvl.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/ghidpsxoc.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gtnlzbvqp.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gpqvhtepm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gdehlgfcr.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gwbodcvsz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gtvqdqqxt.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/grlfstssi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gyhjghdub.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.zdbjq.cn/Article/details/gkvmzpovs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/glhnlgzkn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.fehbvm.com/Article/details/grthgunho.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gbqimrpgz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/gzfhfogmj.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gneelvxcy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/geefbwqdt.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gztwtdjxf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gbjaxzqww.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gzvopzpqq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/ghddwryvg.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gknjaovbs.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gtzjniznj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/ghlxofguf.sHtML

[N05] 最大公约数
来源：http://m.share.hesvh.cn/Article/details/gozoscxam.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/geeieispj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gsfzhxklt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gzalslqro.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/ghmyanawf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gyfvqswlu.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gfwtnehgs.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gesccluph.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gdxzxxpmu.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gnaojphqv.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gecdadlel.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gmshqhtwn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gmxhlfnfu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gbbiqejpv.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gcxehnabj.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gqpkydems.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/guozvymii.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gndthdlje.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gdrgbpjev.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/gojprwknn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.zdbjq.cn/Article/details/gfwbciozx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gcfgvdpfy.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gknsxwszt.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/guoccsnks.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gduhgrzti.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gczrgufca.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.fehbvm.com/Article/details/gqulvooeu.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/grfjjbeqi.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.hesvh.cn/Article/details/gyasabtcx.sHtML

PHP:  // 手写递归交换
来源：http://m.share.zdbjq.cn/Article/details/ghipohzqx.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcbcgmrnh.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gtuodezfh.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gawtrugia.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gqnwhbdnc.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gtlngloyz.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gwkjpdele.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/gchbloqtn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/gdhcndsmv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gswjxtkbx.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gnlvcqgfd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gixwlhckm.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.zdbjq.cn/Article/details/grushvuzb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gszoufkss.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gmiavtuir.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gpicaqvdg.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gsadurgiq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.zdbjq.cn/Article/details/gpezdartw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.zdbjq.cn/Article/details/gaqpzvhon.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gukwqmsuc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gmsbcbxgq.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gjodcdcbb.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gcouelygg.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gylmnwyfu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gvifltfcz.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.zdbjq.cn/Article/details/gnsljpswn.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/ggafsbrop.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.hesvh.cn/Article/details/gxhyigpft.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gtpcaqedh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gccesieet.sHtML

Java: // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gotpdgoaw.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gocoitfme.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/gszabhuwm.sHtML

C#:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gnshhasrk.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/geltelgpk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gwsmajisu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.fehbvm.com/Article/details/gfdwoewet.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/gygwynnly.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/ggoxsznue.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gzbdemhve.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/galacgolx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gcrdxrrkc.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gmuiuvidi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnoonztgy.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gutcmvyyu.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gebkohlqq.sHtML

[O01] 启动一个线程
来源：http://www.m.share.hesvh.cn/Article/details/gqbwkurid.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gzqsfuqlj.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/gwvosnezu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/glgufcidm.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gdbmlwagp.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gbwrxpkxh.sHtML

Go:   go f()
来源：http://www.m.share.zdbjq.cn/Article/details/gdbsplazu.sHtML

Ruby: Thread.new { f }
来源：http://mobile.fehbvm.com/Article/details/gtfkptsws.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gaofxyoxe.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gdnsyekwj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://wap.fehbvm.com/Article/details/gzehrgeba.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gwuditwsw.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gxueudqyc.sHtML

TS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gwvycgzgp.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fehbvm.com/Article/details/gnhydfphq.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.zdbjq.cn/Article/details/ghthzkxpy.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.fehbvm.com/Article/details/gqsfyoxel.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gozirdxjh.sHtML

[O03] 加锁保护共享数据
来源：http://www.blog.zdbjq.cn/Article/details/gskakjslf.sHtML

Py:   with lock: shared += 1
来源：http://m.share.hesvh.cn/Article/details/gcdnsacas.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gmqvstzco.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gcfumcmir.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gkxqzbnsw.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.blog.hesvh.cn/Article/details/gmljioxjs.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://read.share.fehbvm.com/Article/details/gjwajptkv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.share.zdbjq.cn/Article/details/gvboaqgax.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gscopidro.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.fehbvm.com/Article/details/gymtbdxqz.sHtML

Py:   async def f():⏎    await g()
来源：http://wap.hesvh.cn/Article/details/gukliwkkm.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://mobile.zdbjq.cn/Article/details/gyxapjevh.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gsipakows.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gnvgrkqgc.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.hesvh.cn/Article/details/gbaqfduaw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.fehbvm.com/Article/details/gkwwljpax.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.zdbjq.cn/Article/details/ggkxdylka.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.zdbjq.cn/Article/details/gwwliogay.sHtML

[O05] 并发执行并等待全部完成
来源：http://www.share.hesvh.cn/Article/details/grnkwpgjx.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.hesvh.cn/Article/details/gbgvkyhgb.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.hesvh.cn/Article/details/gzdputyom.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.zdbjq.cn/Article/details/gjnnulcsg.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.zdbjq.cn/Article/details/gdgjapzvs.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.hesvh.cn/Article/details/gincyxdlu.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gnjvhwzyo.sHtML

Ruby: threads.map(&:join)
来源：http://3g.zdbjq.cn/Article/details/giftoxmtt.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.fehbvm.com/Article/details/gnykzzdfe.sHtML

[O06] 使用进程池
来源：http://baike.fehbvm.com/Article/details/gswvxptyk.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://wap.zdbjq.cn/Article/details/gvqfyzjym.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://www.blog.hesvh.cn/Article/details/gmrdbqxqo.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gfbpcjmav.sHtML

TS:   // child_process / cluster 模块
来源：http://wap.fehbvm.com/Article/details/gxvxnlovf.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://mobile.zdbjq.cn/Article/details/gjdmsygpp.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://blog.zdbjq.cn/Article/details/gozvvzsac.sHtML

Ruby: // fork 块
来源：http://www.blog.zdbjq.cn/Article/details/gemhwcndn.sHtML

C#:   Parallel.For
来源：http://read.share.fehbvm.com/Article/details/gfleuekua.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvjxvfgxz.sHtML

P. 常用工具函数
来源：http://blog.fehbvm.com/Article/details/gufysmfdi.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grlxzdrvm.sHtML

[P01] 生成 UUID
来源：http://blog.hesvh.cn/Article/details/gvahfabqs.sHtML

Py:   str(uuid.uuid4())
来源：http://mobile.zdbjq.cn/Article/details/gzkqjtzcs.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://blog.fehbvm.com/Article/details/gvzjuvkkx.sHtML

JS:   crypto.randomUUID()
来源：http://www.blog.fehbvm.com/Article/details/gyghxzygn.sHtML

TS:   crypto.randomUUID()
来源：http://read.share.fehbvm.com/Article/details/gvgxfcudi.sHtML

Java: UUID.randomUUID().toString()
来源：http://baike.hesvh.cn/Article/details/gvhszuhoe.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.m.share.hesvh.cn/Article/details/gwaxwojra.sHtML

Ruby: SecureRandom.uuid
来源：http://mobile.hesvh.cn/Article/details/gumqobpqk.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://www.m.share.fehbvm.com/Article/details/ghstekvot.sHtML

[P02] MD5 / SHA256 摘要
来源：http://wap.fehbvm.com/Article/details/gudndusxj.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://wap.fehbvm.com/Article/details/grfoxrxtk.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.m.share.zdbjq.cn/Article/details/ggffoqjhq.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.share.fehbvm.com/Article/details/ggzsplanv.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://read.share.zdbjq.cn/Article/details/gzbuavygr.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.hesvh.cn/Article/details/gcebqgeuc.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://m.share.fehbvm.com/Article/details/gpqiqqpxn.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://read.share.hesvh.cn/Article/details/glqeeuugx.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://read.share.zdbjq.cn/Article/details/gevvaspmh.sHtML

[P03] 生成短随机字符串
来源：http://m.share.hesvh.cn/Article/details/gdulpkbdx.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://blog.hesvh.cn/Article/details/ggxmetcrl.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.m.share.zdbjq.cn/Article/details/getnxqiwd.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://wap.fehbvm.com/Article/details/gejaodlyw.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.hesvh.cn/Article/details/gadicnvde.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://wap.zdbjq.cn/Article/details/gucnwvikk.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.share.hesvh.cn/Article/details/gynpncbha.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://read.share.fehbvm.com/Article/details/gbdxyxsrg.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://mobile.fehbvm.com/Article/details/gzwesjlyy.sHtML

[P04] 求长度
来源：http://wap.hesvh.cn/Article/details/gkyghhcij.sHtML

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.m.share.hesvh.cn/Article/details/giqnaakkk.sHtML

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gaigrgqvi.sHtML

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://blog.zdbjq.cn/Article/details/gjicnukkj.sHtML

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://wap.zdbjq.cn/Article/details/gubzttwqb.sHtML

Java: list.size();  map.size();  s.length()
来源：http://www.blog.fehbvm.com/Article/details/gghludnwt.sHtML

Go:   len(arr);  len(m)
来源：http://wap.fehbvm.com/Article/details/gwhttiisl.sHtML

Ruby: x.length;  x.size
来源：http://baike.hesvh.cn/Article/details/gzbaulbis.sHtML

C#:   list.Count;  dict.Count;  s.Length
来源：http://baike.zdbjq.cn/Article/details/gwmgufbro.sHtML

[P05] 判断两个对象内容是否相等
来源：http://www.m.share.zdbjq.cn/Article/details/gbcxsrueo.sHtML

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.share.hesvh.cn/Article/details/gwdtqfszs.sHtML

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.blog.hesvh.cn/Article/details/gsuvkmkbz.sHtML

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://m.share.zdbjq.cn/Article/details/gbmrfnvke.sHtML

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.blog.zdbjq.cn/Article/details/gzrdreneq.sHtML

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.blog.hesvh.cn/Article/details/grrccfpgd.sHtML

Go:   reflect.DeepEqual(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gxddoidxe.sHtML

Ruby: a == b
来源：http://www.blog.zdbjq.cn/Article/details/ggnbrpino.sHtML

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://m.share.hesvh.cn/Article/details/gislbqslu.sHtML

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.m.share.zdbjq.cn/Article/details/gsompbsxh.sHtML

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://blog.zdbjq.cn/Article/details/gdigjvmin.sHtML

PHP:  if (empty($x)) {}
来源：http://blog.fehbvm.com/Article/details/gagpmagfh.sHtML

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.m.share.fehbvm.com/Article/details/gvreiohjo.sHtML

TS:   if (x == null) {}
来源：http://www.share.hesvh.cn/Article/details/ggakvdnhm.sHtML

Java: if (x == null || x.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gzneagzjn.sHtML

Go:   if x == nil {}
来源：http://www.m.share.hesvh.cn/Article/details/gdigiavkp.sHtML

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://m.share.zdbjq.cn/Article/details/geurkasig.sHtML

C#:   if (x is null) {}
来源：http://wap.fehbvm.com/Article/details/gjfpuowwj.sHtML

[P07] 防抖与节流
来源：http://mobile.zdbjq.cn/Article/details/ggwqqrujj.sHtML

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://3g.fehbvm.com/Article/details/gsbextoir.sHtML

PHP:  // 手写时间戳比较
来源：http://baike.hesvh.cn/Article/details/goboneoej.sHtML

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.m.share.fehbvm.com/Article/details/gjnwrkxwv.sHtML

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.blog.hesvh.cn/Article/details/grbjgxcxj.sHtML

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://read.share.hesvh.cn/Article/details/gcdgknlwr.sHtML

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://mobile.fehbvm.com/Article/details/gkhtovltx.sHtML

Ruby: // 手写闭包 + Time.now 判断
来源：http://wap.zdbjq.cn/Article/details/gtqubowgd.sHtML

C#:   // 用 System.Timers.Timer 重置实现
来源：http://mobile.fehbvm.com/Article/details/gcpnqwhhp.sHtML

[P08] 处理浮点精度问题
来源：http://m.share.fehbvm.com/Article/details/gpfpctabc.sHtML

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.blog.zdbjq.cn/Article/details/gvgwpqdos.sHtML

PHP:  bcadd("0.1", "0.2", 2);
来源：http://wap.fehbvm.com/Article/details/gfivqthtx.sHtML

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://wap.fehbvm.com/Article/details/gbqepbcrf.sHtML

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.m.share.hesvh.cn/Article/details/giqyjmeih.sHtML

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://read.share.zdbjq.cn/Article/details/gcwxesvea.sHtML

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.share.zdbjq.cn/Article/details/gatysloea.sHtML

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.m.share.zdbjq.cn/Article/details/gjbfvwlqi.sHtML

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://wap.fehbvm.com/Article/details/ghrwpotao.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gxirhjczv.sHtML

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://blog.hesvh.cn/Article/details/ghtjaxylp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnbwcnrhq.sHtML

[Q01] 创建表
来源：http://read.share.zdbjq.cn/Article/details/gxckteimv.sHtML

CREATE TABLE users (
来源：http://www.share.zdbjq.cn/Article/details/gyngaynkg.sHtML

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://m.share.fehbvm.com/Article/details/gkduawbbm.sHtML

name VARCHAR(50) NOT NULL,
来源：http://www.blog.zdbjq.cn/Article/details/ggplcffpj.sHtML

email VARCHAR(100) UNIQUE,
来源：http://m.share.zdbjq.cn/Article/details/gkfkrsomk.sHtML

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://baike.zdbjq.cn/Article/details/ggrqlsphk.sHtML

);
来源：http://www.blog.hesvh.cn/Article/details/gpbcinmhx.sHtML

[Q02] 创建带外键的表
来源：http://mobile.zdbjq.cn/Article/details/guglbhnzz.sHtML

CREATE TABLE orders (
来源：http://www.share.fehbvm.com/Article/details/ghzqitnpc.sHtML

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.m.share.zdbjq.cn/Article/details/grivcqcap.sHtML

user_id INT NOT NULL,
来源：http://www.share.hesvh.cn/Article/details/gctbbdyoz.sHtML

amount DECIMAL(10, 2),
来源：http://www.blog.fehbvm.com/Article/details/glopujmvs.sHtML

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.share.fehbvm.com/Article/details/gvzqlmmez.sHtML

);
来源：http://www.m.share.fehbvm.com/Article/details/gvgpgiwfr.sHtML

[Q03] 增加列
来源：http://mobile.zdbjq.cn/Article/details/gzonkqivs.sHtML

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://read.share.fehbvm.com/Article/details/gggiiqgqe.sHtML

[Q04] 修改列类型
来源：http://wap.zdbjq.cn/Article/details/gfqxibttb.sHtML

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://blog.zdbjq.cn/Article/details/gjpssanjs.sHtML

[Q05] 重命名列
来源：http://mobile.fehbvm.com/Article/details/gknctruid.sHtML

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://read.share.hesvh.cn/Article/details/gxkuygkav.sHtML

[Q06] 删除列
来源：http://www.blog.zdbjq.cn/Article/details/gnjqleefs.sHtML

ALTER TABLE users DROP COLUMN age;
来源：http://baike.fehbvm.com/Article/details/gqbopoayn.sHtML

[Q07] 删除表
来源：http://read.share.zdbjq.cn/Article/details/gidvvvgze.sHtML

DROP TABLE IF EXISTS orders;
来源：http://m.share.hesvh.cn/Article/details/gfgosyarh.sHtML

[Q08] 创建普通索引
来源：http://www.share.zdbjq.cn/Article/details/gkmumyjwy.sHtML

CREATE INDEX idx_users_email ON users(email);
来源：http://www.blog.zdbjq.cn/Article/details/gcyphobic.sHtML

[Q09] 创建唯一索引
来源：http://www.blog.zdbjq.cn/Article/details/gksobdtbb.sHtML

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://read.share.zdbjq.cn/Article/details/goxfwowul.sHtML

[Q10] 插入单行
来源：http://www.m.share.fehbvm.com/Article/details/guycqhrig.sHtML

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://3g.hesvh.cn/Article/details/gvbkbrbfm.sHtML

[Q11] 一次插入多行
来源：http://3g.fehbvm.com/Article/details/geguecexn.sHtML

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.blog.fehbvm.com/Article/details/gktngwzzo.sHtML

[Q12] 插入后取自增 ID
来源：http://m.share.fehbvm.com/Article/details/gnvldmhur.sHtML

INSERT INTO users (name) VALUES ('C');
来源：http://m.share.zdbjq.cn/Article/details/gcydgrhxj.sHtML

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://3g.zdbjq.cn/Article/details/gblfaprot.sHtML

[Q13] 忽略重复插入
来源：http://www.share.hesvh.cn/Article/details/ghmttjuhg.sHtML

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://read.share.zdbjq.cn/Article/details/gbioojghn.sHtML

[Q14] 存在则更新（upsert）
来源：http://m.share.zdbjq.cn/Article/details/gzpetbqrq.sHtML

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://read.share.fehbvm.com/Article/details/gcacuhovj.sHtML

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://wap.zdbjq.cn/Article/details/guqsgnqmh.sHtML

[Q15] 查询全部
来源：http://baike.fehbvm.com/Article/details/gxuicessw.sHtML


<!-- 参考信息 -->