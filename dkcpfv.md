代发 wailian999

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2jkgoadfp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2uqocxdzm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vxwlzwuy.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wilpcfdk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kzivrcfh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jajpufjw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2volcifqy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2boknsorr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2bmamlevn.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2uduqisjh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2riaizfwy.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jowjxxpp.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2iphapjoy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fzpmdzfr.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zvxgymfr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ehtwckge.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kwfajfvw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2udhzlnol.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2thssofrt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2oipfemkm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nnoesrey.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nycknvbg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2iiiyldon.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ayfazmkb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2flnrzrwk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tnoajhut.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qrnzgqxh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2wkwqdmma.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2wrennhic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sioupure.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2udukygih.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uykqtwbu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hcjxbbnz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2leirfvne.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2luzcnonq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2bfvgoapv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2psndzqwr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lwujfbzv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnmjslac.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2covogjrh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrhudph.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2iffutjat.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ogjpkvel.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2flvwkwlf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yasvylsg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2crtfwspm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yqcaohmb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2hbfgminy.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zzjsbqxf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dosbmvlm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2loeftvlz.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zrdsqdzn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dgahbppg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jslaulzl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2gkmoniuh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2amvfnkqx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jwvmucij.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vhzsvyos.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2rmkaxhim.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2xqzhfhuw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xzirjrxq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2fvuylhnw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sfslovff.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ilulqtzp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2smylgagq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2pkccyjuj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ivlwfkxd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2siqpuqid.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pvknafrk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ajpiinfa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2amvzdlic.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2slhfadxp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtffqeyz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2wrdrzutx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2aaallkuy.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hwlcsqwo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ajaegurm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2krodrpqa.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wehfqrqd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2vxjipcbi.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rxhufusj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pqhrbhfr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2osfonwrv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2kxeppfwv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mrlgkcqc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2eeeheddc.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jagsvyze.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2wgibwfif.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ukvtnkup.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tstybghc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2tomksgjj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ukgdbeus.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tkyfqgws.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2wlqxjxlc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2acdrjrde.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2sungnddh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vlwigzxh.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2joxqphtc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yrbwyjhj.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oovqeiuf.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ewtzmnft.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2epssouvp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2gmxpphax.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xgpeinoa.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozbdqkyv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rygxiwaf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qunftzsc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2whevboqi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2joovlpeo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fjbqzhut.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ezidlhum.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2itoxnhtz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nzdonwzr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zfodukil.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ktstxlgy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2vbgstoyq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2avikcewx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2tlqbphvx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubyblhlb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vbtsfcev.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ptcyonsj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2coyqpqig.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oavtxxgw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ehninupt.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2anuyqjgm.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2okcnfgcs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qakbuzyr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nhrvemyn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2aoshjtph.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pniyjzsc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vvfhhmor.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2aupsnukv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ivysqwkz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fqbjnyoa.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2clkdjfxy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oadrzirv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fodyltyr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ohwdpcaf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xnwsqtgq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mckntmla.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jhsyqsje.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2oaivyzmz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mmmdzceu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2mtmkjapl.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2brybwbuy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yjdlaabo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ijqsmvuo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2crzphqkf.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2faljldzc.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pcfeaakx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2zixnmytz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2syaybija.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iwcqouwz.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2pnfxwacu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hvlslhry.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fmjmfarb.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rgjidxgg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ccqcbdss.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2grpyzgmt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2izobdyin.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2gswpmplw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2gttkomng.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2gotzptao.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2xttdknsa.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2kthzpxvk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2seguzhxh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2ttqunwmq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tpznnnzf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2cwjhwlqv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nbmhwkmp.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2btnljssw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ncsczzjh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2sawivhih.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2sqrbmqod.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ozivytbq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2hazadoyk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2sfsjntdy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2niglfkzk.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2licnvwvc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2aeqckczc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2dvxaktbp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2unzxrnry.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2qjrscusg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2dhpgdrfc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vpybdszz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2awjztyiw.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2upmwcauq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wowkeqdr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tqeqpgzh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2jexwifjs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2zrjbizlw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gffbmhbx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ixmzpkmt.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sepzjvgo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2rrpubyaj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2himdgvxy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2wkixugry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjjmrppf.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2mzxbzfqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cgjlwcmm.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2pbylyvzh.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2nicvujkp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2gqrtnplr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nlalclok.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2scoreiti.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jzgbnbbi.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2jfgtpisq.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2lmctjtav.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2amgrktmq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qbnftnat.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2wvkfytrr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2iaezewhv.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2djuddytk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2kzfkutdt.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nzzqknki.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2tfalktft.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qwwoavwp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2kvcldhua.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nnagxwjd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jkughnwa.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2famjgguh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dxxcufkv.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vzhlqioq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2cyxfulwm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2sytkrioo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2birgvgaw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2aexfxhzl.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2cawvgilo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2lskahwgy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ielsmlal.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2magehsjy.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2dopbmllc.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2oxvyzetc.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2ozevtloe.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2enjyfqnd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ebonryvf.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zrgsvdqg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2nxurnfin.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jeuwpurr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2gasyseit.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2fcarginp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2xxdspkhj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tdezjvms.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2mtlqfirj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2asjgpdse.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2iouajukn.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tgvwkftj.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qvkgyjxn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2fqobzfck.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2oyyrqpks.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2smcyyyyl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2fpcroess.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2jzgrqjjv.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2kgdwtemm.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2bchhnfsz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2irpvjwao.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nwrxvfkb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dbbcreov.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2pvqepmuc.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2czsfufps.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2wypmfmvc.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2ckcnjbph.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2nfbzehxl.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2pichyvsq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2phhbmsmf.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2rklqzsys.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2chdwtkmk.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2axvjffqj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2glqtcnpl.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2xqwpicyg.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2aillfazj.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2wmceeahq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qbacvxmw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2tuskfxkv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ahjedcwp.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2rpbotclt.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2xbptjomb.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ppprgafu.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2gmgfglhg.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2ltbzeyag.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2vlgtpuse.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2mhpfcpex.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2tlndfuce.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2gwiuboqh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2kedcftvf.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ordzyafw.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2pzrnkfvk.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2chcmcndu.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2refhhiur.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2oqubfkaj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2esqffdzt.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2yysdszwd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2ufrzkabp.html

[Q05] 重命名列
来源：http://www.ydjk.org.cn/Article/details/gt2xwqjmrai.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2djlcvggg.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2tuartxha.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2fcbkcdxp.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2dnmuwrbq.html

DROP TABLE IF EXISTS orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ecjgqxnf.html

[Q08] 创建普通索引
来源：http://www.52xcode.cn/Article/details/gt2hwwgrkwt.html


<!-- 参考信息 -->