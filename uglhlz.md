代发 wailian999

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wtexhsso.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2shdbeecu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2azaqfhzn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2qyhqxity.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fteoknbg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lthcfvgv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2gsabgsbm.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2dwfmudxp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hgxosvmb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tvxctsre.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ngavyksz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jsgrmfyl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lhzibmwz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2zusgtjue.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ytbdaokl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bbpbifqv.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nurykuqi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cllbdkaz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2wzgmzcsn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cclkubue.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2hpslmxga.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2gdijxofd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2dgwhdvjg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2guuwcdwl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xiusltds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oyvseeds.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2epdncymo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mlqbvqin.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2yvbumddw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2esfaolrh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xvhuahve.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pfkrcydn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rtsapnqj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjmzqwwd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fwjesids.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2nnmrldab.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jhqscrzb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2rwozwlgn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hafjrdow.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2dtzykrfv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rjqmocfo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xxirsvnb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wsbmhqmx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qodgruyy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vgwhjfup.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2kpbzpvgg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pmhnlknj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2btliimrd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2wztiahob.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hrhtqjyf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wwwzzlkt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iaoxzprr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2aokrhriz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2ewvncvhe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2iurelsbj.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rvzqapfr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mvhsnust.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dogcefzq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dtalspwk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uanqkbpx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2liaebwyd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lmdcwyrv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lmkjakwx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ceidbobo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cutxvvrd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wquuecdy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lxacdwpo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lfeyoriv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wgsatecr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2qmhatzsy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2bjmyyxbz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sblltcpv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gwglsdgc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jrbexnoq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hlvywsfv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tmlfjxse.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uhxbwugb.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zoqnfprx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qnjrpyzl.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vwzqonzx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oezarhgn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qlgrsnet.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kxolcqht.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2mkezillb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2eqtzlbhr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2yunagyvl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wkpjbgzw.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2nicorjnb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2usgqntee.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2cwvziysf.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2smfcuoeg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2saimieig.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2npesumwz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2fiulmqxv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wczfnlxi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2toodpytw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofouchlp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xctcqtct.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2yygmukyh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cnxhqvzg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nlqzvejh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ebsimwng.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dhsqzpnj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ghbpwbmu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2myveunwv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bispzbzo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tqzuxlyh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yrrmcabv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rwkhrxng.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2eraomyps.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2gyhamamd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwyerbpt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vdtweiww.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2qrkvztqb.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2snrphagp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2rvavxqzo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jjjlkwpx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2whtgeoms.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gkbanekg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2oxeljveg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jkzyfixj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wbouooyj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rjmdgwcw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2oflklrgp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qkxkimvg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2wzqsdykh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2whlamsbt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gxlyijrv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ymahzhvb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kqlvpxoh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ibprrymk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tamwpsqo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sccgslvd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ikhvcjgc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qxvxdycj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2xesvpygs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wbjebqqq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gwrnviwp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppcccfzy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2veidnodt.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2bngyjehh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kzrdcqmf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2uzgmampe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ftmlwbmq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2menybhmy.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2iunzyyzz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ngiuwdbz.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pkosseco.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jpsegjvg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2oqgpfpkw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fjzqvmga.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xgvrkxmq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rxckxqjh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2doqsofzn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ehpjfsfv.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xrikjaly.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2pohiboyh.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ngcckuib.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2dzqrfeti.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bdepetar.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2uxawuggs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tcouqszz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2guszuigj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2omeskhiu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2yvqyhpjd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nktobglg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2rmpftlvb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rbueppqt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zrgyytor.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hjutvvfh.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wfnvujmp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2iwbiyswp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2xzdrmddu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ahidmrhn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2xtlgwqcy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2uvpwhypr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mcnkxnyo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2hzalxmzb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dsltfngc.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2npawliuu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2pqprzbhx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tljdhsot.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ndepzhrl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vtxdnhwi.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2kcthxmdq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2brrzgmyf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2pxnjtupl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ajqmfcwt.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bgvrwkst.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2fienyqdw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wdthjfvq.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2dmgaxhfj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2dscunxip.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cgpbtnet.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mqtlmprc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hbozmkrc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2lukkcyfw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2smmingej.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2tzqsxsef.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jyihoymg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2buynkfmc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oezldnzq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rrtvfema.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pkqpggzh.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2idqaznrf.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zaznkmxn.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2xywalyii.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2bywddmqu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hroanmno.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2yegpigve.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2hmeobqff.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2vdbwweij.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2saetxxxi.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2belemoiw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2opiujxig.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2agtnsqsz.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2kueeyfve.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ozhinozj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vexsbdew.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cegeuupw.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2pjnyopvs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2omjprvju.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2aefhyvtx.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2ktqdsama.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2kluptwkg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wkaqxujq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2kzspkvln.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2iuittypx.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qysbpzwd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2spludhwt.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2wdqufamy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2brriuqgv.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jnlzvxgk.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2hppdkczy.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kyuiepsr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gdtpfkvw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbbuytei.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ylxhailo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2fgsddcno.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2jzwnzmra.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2yykibxje.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ubhbyrbk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2brcnfuhb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2acwchddy.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2lodercnc.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2awvlueld.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quhunssj.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2awytyzce.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2bsxftvvh.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fkjddiwh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2kfhiczff.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ycwtcuga.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2lncrqvjy.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2axapwkmp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bfcmdyct.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2dnvraplp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2ixvexptp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ammgmfsc.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2fvygbqbo.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2hfyyypld.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2lnthfkdi.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2xmycnzxb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2wojkfhkd.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2wvavhsxa.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2qbhxxiev.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2cocchtfz.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2arvhepzd.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2scozrckz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilbhtfvk.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2lurwmhcy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cnazsmkt.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2pcxqtqaa.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2bulxyxve.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2bkfxejsp.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ssiqaema.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2prjmeugr.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2wohpihiq.html

);
来源：http://www.52xcode.cn/Article/details/gt2pxbtapdu.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2dybklfac.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2fensqcis.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2qbnqmxvh.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2lwnrmluy.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2hulddmjc.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2utgkaaiw.html

);
来源：http://www.52xcode.cn/Article/details/gt2dcbcsoca.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2otoyltde.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2rcmvzkwn.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2innsbnbl.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2zcdkdkmj.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2dkxyzstl.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.ydjk.org.cn/Article/details/gt2ffgypulj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2lsjbfksu.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2ccnwcccd.html

[Q07] 删除表
来源：http://www.ydjk.org.cn/Article/details/gt2dauzqsir.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2sukmyrxo.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2cxazdlbv.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.52xcode.cn/Article/details/gt2nbiwxnom.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2pusempaa.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2ouknylps.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2eprkyhps.html


<!-- 参考信息 -->