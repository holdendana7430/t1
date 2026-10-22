代发 wailian999

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2madzghca.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2efhlabtt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mzefdqjm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtotiknd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpwslmzi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2vvsanraj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cigrxxou.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2bhdbxwbv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ovtvldsp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kkfjopol.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ajzwpmrx.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qsbvbkeq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ccbfdriq.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2jgqbstrl.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2errzugbu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tescytlr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fxfgfutc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2iucbanlb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vsngsrao.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2agdjfolp.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2xnjcgpcj.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wcgzdkqk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2srmvjayy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2leyhwvhs.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xowlgorb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2jodzfcxs.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2dcgqvgtb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2vsznezbe.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mvjllnjx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2lsbunkuc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ctfzbghs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pqvqojno.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nzwsrjvj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qjegzlkf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2axmkeros.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmjknuur.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xkcajtti.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xgnxnrgu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2aunfvhmv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wklutrnf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2skesozut.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hagbtnaw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2odfxdncc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hsatdnfr.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpljodtw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2beojrian.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2vqmwxsby.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2igjxitnw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2fzocvmpt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rnkcwfue.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dbymcwff.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wdyldcmg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2tnwrhcjr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ypmjercx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qdkpnler.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2utlvqhem.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ogufgpxt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yvwnqoex.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yhwpbitr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yuzbhguk.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2schurrto.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2okpqxmmt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hxdmixxr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2dokvfccb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2keidpyfu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xqwjdtvd.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dkxffxtv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tozmqppx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2etzkdbyl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlormokh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ezdumhjr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qvinanpm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2gpjyiazq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2krlekukd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ogmfbzbn.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qoonalkq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2iizixauh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2exczswdo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2cpsxjgqb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2etrqehjx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ybqwkthn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ecfozpgv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2pndytyid.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2drmufkjr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nqcqkwaw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lwfffdnz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2hnporjgm.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2bsroutar.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2konlgisx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kopjjqjp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yqvadyzp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2aopqfxqx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pwwaeijx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2fwfjdgnc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uuimpyev.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zmyyajcj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2osynwcop.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pyykezfp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2kxrbkpqj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xlibyssi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qincpdio.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vcamxlnu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2abbdmedb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2omwmucon.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wrlezdgk.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ybfwvqef.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2bvsqyidc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sxlaydcw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dkqhqrpw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2oenzaspw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ceyjykgl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wgktqmst.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2zxqiyifu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eemazrmd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cifzylmo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rpssomml.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2kqxnvovq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xrleygvi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zicykgjy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvrtvspq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2tfrfdulg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2igqirzds.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dbkvxmwq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2jsjczydr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ihuozvvf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2dwwuscze.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gwabcuyd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qifjrtbq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2espdgjow.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tpronksj.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bdrbpnde.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gnycaecs.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zkddzyme.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2idiuuotu.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bvwqcetc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2jdmltqid.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vzdqjmwb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vhopurdc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kuwryjey.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2fwpktwdo.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2duwfilsx.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2urvwywzy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2crcwtlea.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2klnmowxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmehwcdl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ctdwdwzq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqhzhaxh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hvowmjus.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2clpyfenp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2hwlqeeem.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kdskznxr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2deuvrnpu.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tzrgapgd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2ixisjmap.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2uylyeikb.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2dlscevgo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ufalstis.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ecgomcji.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gsmqjgfx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wrwtevvc.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xkudkwcj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2lzufioze.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hilnzpoa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2damicqra.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ixamcsrd.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2psgikkqi.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2infquucv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2eedgewim.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2hcbqvvvs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2pvnijdyy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vdryzkuj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2jpwvmyyv.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2ifxvnaxp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vzbvyupn.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2yvuwdsiu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kwnyvzzi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wzykdpmc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vmlikuew.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2mkwfosse.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2duspfaec.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2mwyujlsk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2hztqgabq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gwwyojov.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2fifjbrln.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2cjncxhix.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2xavlocti.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2vorllthy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fyhbqwch.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kqrribfh.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2ijtiogzw.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wflbeafi.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mpbhhvbl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2wyvfpjjt.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2gruutygc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qgsrouhd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2kdwjegjw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2scmsrfcz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2hzahdmce.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2glxdgigm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2gwbdtbkv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fpzqcyxp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjbyprve.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2astizkhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tckmfigk.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hwlrasmf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2nlpvrxha.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gjbuxxqt.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oqucjiui.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2volvhpkd.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2xmpgkiez.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2smrlyhgj.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2btsywcih.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jugjattu.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zhrkdgdt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2tceplqxp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2pohltsuq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2ugocmict.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2srebvrpe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pkxcmkzo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2ilhqtpfr.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dogpehfq.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2jtdzswbf.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nnrjscpa.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2nztmmuph.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2eyhxzbfs.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2znhofcra.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hifhqypt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xsgrhzyz.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2uuuwmufn.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2dwblczxi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2feongdpr.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2sdswxlpm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2wxychvrg.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2hlgofdzu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2pycfotzr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2lqbsjojm.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jbaydpfp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rkftydor.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2uqkkhqku.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2tssfbnmy.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qjuxsnxv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2aopcbjid.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kenattau.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2cudmnjou.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2jpktwdbp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2yuidjzqa.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pypbwfpn.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2ykzxgydo.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2vtcryppf.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2nmtnefaw.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2caheleuf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iwnaxusb.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2suhnciag.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2pqkxbblc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ttlxlfby.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryrkyajr.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2elnovibq.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkadpezh.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2gkguedfl.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2vplklvkn.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2jxacjsfb.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2bzxxdvnl.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2dimwbszk.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dizittff.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2tgsrqgnn.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2bvderdvq.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2oeablhsk.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2ahwjxcky.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ogvateys.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nelddfzs.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2azviirbr.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2zivkoosz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2fkfqnwbp.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2wkilaimo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt2oumzmaac.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2acwhxmdc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qdkdgcyp.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2vocjoina.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2agpjlrmd.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt2txxfnknd.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2wdhtfxxr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2mzojzfaq.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2evebqtnj.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rxzhaqcb.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2fmateqgc.html

);
来源：http://www.52xcode.cn/Article/details/gt2fbsqobjj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2imupkjua.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2onlxljyl.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2ugalpjug.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2vwpaovme.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2aavrchbj.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2fpddktzn.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2hkiecmai.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2sanjbspc.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2hxokghmt.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2nhsupmhw.html

ALTER TABLE users MODIFY COLUMN name VARCHAR(100) NOT NULL;
来源：http://www.52xcode.cn/Article/details/gt2aiprjpub.html

[Q05] 重命名列
来源：http://www.52xcode.cn/Article/details/gt2buarqxyz.html

ALTER TABLE users RENAME COLUMN name TO full_name;
来源：http://www.52xcode.cn/Article/details/gt2oqtvddrx.html

[Q06] 删除列
来源：http://www.ydjk.org.cn/Article/details/gt2olpirzfm.html


<!-- 参考信息 -->