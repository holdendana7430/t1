代发 wailian999

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bnomftmf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2gjudvury.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hdgditsu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2idikjlnp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2esbdqavi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ikbrhgpj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nhdbmyrv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nqdswbfv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2amdumhqd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wynlechz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2axnjbumv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2vafcihky.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2auzmcwip.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2vfuiydfn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2movughbh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2eulxdzqe.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2oiewsckc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2dyickiym.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ggswzcjk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2xmwdhqwp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2pteavjfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wnlpquql.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2naqqkolf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cvxdprco.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nnihwagz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mlkrzfet.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2nrxgwnsh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2asvsxtdo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hsqzqkcm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xcqqvmux.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdmlehz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ywiiudds.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hqesqspz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2eiwgodqy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2azgqebcy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2udjzgitm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lvgrjguj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cgsdykzs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zkftivco.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pwhnfrmo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vwxvbqur.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hpxhgpqs.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wplduksa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2zqggpryo.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ocislcgl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vlpktcwt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ibcjdlet.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ibxrtchu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jvbngwbn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vwwuwnlx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2kfyifcfn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wniiqypu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bfduhhgr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kspqitpg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vodyvstg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lxmijruh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnnfyffm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2whewyitr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rwitgcrg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uazwfsnf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2bilszqfh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xoxwkpeb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ykmeomzp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ofytsviw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrdphzya.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vccuwihq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lulrgwjx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qnlrupim.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2safdjlwk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lutbwzxw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wveiacni.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2iycscrgi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vgbmpgdl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aqxsuuhj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2sgqmgmpk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wkzosuie.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2oeggszlw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2udassbvt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2mcanqjwf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wucvwsck.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2mwhxzgbq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2ieriowgr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ibbxsdiz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ecsifmpt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2bomwrmxt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2juapukjr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2awniuepp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2totgvfdz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2fzmumrof.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zklgtvoh.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2okmgudja.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eiawejpg.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bhhzptgf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2izwjchwp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fezyhtxw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tzgqpaxq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ifhhhdfw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tdqdaqmk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fjhmiwle.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2suqonkgf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2otfhfeep.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hapgxhyq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2bpeptplo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2prwdotzl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pddfidxz.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wuddmlsl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2xatqfqim.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fihmarxh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ajppvaal.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rdipyzjx.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2htbuuotr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2salvwpjj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tcmtvnde.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hbmfcnje.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aooyiunq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ixatldeg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cxvtgueu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wkceuzgf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hnrfveag.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xcbtlxwc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ggqyfkvy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ierlwtoe.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2muvxuvkf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2monnwufc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bsjdstfo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2hkbtnwyz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mgmogdcl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jjbzxjqi.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jxzzcdlz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2sgzbwghu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2gsxwaujs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2albjzvzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mnxupbmi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2hdbllrqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2saebczzk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2yocjfeda.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xmnwelbz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2wpwkcmvf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2gqoupmae.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wfffvxfs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nxiuozwq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2kwdxfzae.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vhjutyul.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2kewcykhw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2aogthaca.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bmfpoatc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2oogjsknh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2eaoolmlr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wscixasm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2cyttdpcq.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xrnvocji.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2nntnuygl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2nzurzotb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2kckciwnc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ekfyfgxn.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2izpgcxiy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2etoupsxf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zsjvfwri.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fordpjlc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hrygbfbu.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vbqeksnz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2mwmzrylt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2vbrwraia.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2dkvkigrc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2btdyepxv.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2usipeksq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gztvryma.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2jyizbrro.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2znxxfhuo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2jumgkndj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2pvdwodop.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2svkklqpj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kfhvgqlc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2oeaejxpe.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2cvuvkwod.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2batzwndz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2xhgbkeja.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tgzfbici.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ddgixiqa.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2vnuoulyf.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dhjlumoh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2lsdxbcae.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fiptsxmk.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2kwmgpzft.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2hmupwhpv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2xpixgcly.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wvcetvnk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qzvklrtp.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ohkldsra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqdxgfvu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2tqnjnupz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqvstiiv.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2awxqywzp.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ujfeafhm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2wscxhdsx.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xhmrlshs.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2syursxdr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wbkretrs.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2lsewvfgv.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ibksxrew.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2rqnijxid.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ddjqpqvm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ecaddxbd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2olosibej.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2naxkidfo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2zwsuyvtw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dkylgqjp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2zbogaabx.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tpagjaul.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2yyyfrmlm.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2mbkpwinl.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2wbynytcc.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2zblxnnfg.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wrvakoty.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2inssyqbd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ralohwhd.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2odoxsdch.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2rikgwjkn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ftvbvqtq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vpqrihzf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ztgdfaml.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xnvpkwsz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2itspbbfr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jneucuhd.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2venksbwu.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2oftkeozx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2uaqicdkh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sohwxpzb.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2zlwicnxc.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2sablvdsa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zvutdyxz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2smuroans.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2okoqcrio.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2koxcdwzu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kdugobgr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2xfqrrmhx.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2qqxkkbhy.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yvvzpdtq.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2umwmtmwq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ovbevszn.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2zrpagxbn.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2biftkcav.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ecdwfwbw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2zxkuxdnc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2qxwtvddw.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2rstwcpnz.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2aldbvqoh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2kpjelmwc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2wgxdcfsj.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bblwpxbk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2bohpnfgr.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2bjdwkmga.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2xzcnmidz.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2mtfoclbs.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2notkdtdk.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2evjvxvsn.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2kmmxzglv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nzryfqnp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2itdfnwtc.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2txghjhdb.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2fcknoyto.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2olznipek.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2dlzmimyo.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2krqugpps.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yejkmxhw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2fjgngnyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aimrsrln.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2rojiivgx.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2wnhisjpy.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2qwmtumbb.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2bcwaegsb.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2zijvypqk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2ddmlykju.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2zlvzlhcs.html

[Q02] 创建带外键的表
来源：http://www.52xcode.cn/Article/details/gt2pteexatd.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2nuuyvaow.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2kybljmqr.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2ahxjsomw.html

amount DECIMAL(10, 2),
来源：http://www.52xcode.cn/Article/details/gt2cgddwsms.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2slzazqrc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2upiqsxvl.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2vefnvxao.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2moddcltt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2fyxlaqkd.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2sheukhjt.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2zzeemfff.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2ywirfpbj.html

[Q06] 删除列
来源：http://www.52xcode.cn/Article/details/gt2sdlszbpr.html

ALTER TABLE users DROP COLUMN age;
来源：http://www.52xcode.cn/Article/details/gt2bbrcepiw.html

[Q07] 删除表
来源：http://www.52xcode.cn/Article/details/gt2mdddnhhd.html

DROP TABLE IF EXISTS orders;
来源：http://www.52xcode.cn/Article/details/gt2qraludbz.html

[Q08] 创建普通索引
来源：http://www.ydjk.org.cn/Article/details/gt2raujpgfp.html

CREATE INDEX idx_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2hmzvbbws.html

[Q09] 创建唯一索引
来源：http://www.52xcode.cn/Article/details/gt2gpnpbdfx.html

CREATE UNIQUE INDEX uq_users_email ON users(email);
来源：http://www.ydjk.org.cn/Article/details/gt2jugbolok.html

[Q10] 插入单行
来源：http://www.ydjk.org.cn/Article/details/gt2moregzfb.html

INSERT INTO users (name, email) VALUES ('Tom', 'tom@a.com');
来源：http://www.52xcode.cn/Article/details/gt2vavjgkym.html

[Q11] 一次插入多行
来源：http://www.ydjk.org.cn/Article/details/gt2gazwyoxj.html

INSERT INTO users (name, email) VALUES ('A', 'a@a.com'), ('B', 'b@a.com');
来源：http://www.52xcode.cn/Article/details/gt2ekuhfsfo.html

[Q12] 插入后取自增 ID
来源：http://www.52xcode.cn/Article/details/gt2eamjdjhb.html


<!-- 参考信息 -->