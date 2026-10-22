代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2aaqmjchy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xbdhxwya.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2azhwtpmv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2vuwcjbhc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mfuyueqe.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fjeicqnz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqhpfyej.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zwznjyns.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hbuyybto.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2demoinwh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ciqpzlfj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cfpuirsr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2auiqzfsw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2flghevpn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vstbpgfp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vtkzqlqy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2lstopxhw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2zjfvesjq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lhojjrga.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mdmxbyyx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2hbgzzdbw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2gqqstukg.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aalyjadf.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nqpmlwef.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mhafrqcv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kucqvyma.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2dflljkou.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2buqjzzio.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xhktmpth.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2bkrpxlln.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2eifdhuen.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bwtupkwk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lzctcald.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2vusojpho.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wwgrxfxk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2fexqriai.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2rdddebgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ggasvvcw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ftfsannb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2abfshagw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2wmuikvcl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wpptcswt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gkgzxccr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vpjtmjzo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2gorzwdhp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ecptxkby.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ugpqcrvq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rjxobcgw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nujjnwqh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2cemfxood.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gpbtvkcb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2rkhgfovl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vwbcndss.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rbcdnfyi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhrzbvk.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpfailhg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2aiwjhyai.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iztmssqc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jhlzmbcb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ikttsrfd.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2mfrzscxc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lvfsmbxi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qvuqpejb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2soqxsvpd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2knojbazn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dycpvlqy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2iblvwzsb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cefkzlau.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2aitgazco.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2dohupmgq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pprijzcu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2shboytvz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfaszoqg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2kjzqhuis.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2stysjwsk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kxqujezb.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wztazdef.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2znsdjexx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2etkqwfkp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mcwzvjig.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfcbkwry.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hfhtkcrn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mlianwvg.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hdxdozuh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2xrrvybnp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2rltjifmp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hkcdgyfr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jmbsxeto.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2krfjecdg.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dlcgfrbr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ebtvfdcl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2qxdwvmal.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2acbjueft.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pqulrpkl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yhvoljxe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2eojycutk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mpazzeot.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2qxygskja.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2decnfhal.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ozqkkifj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2bfsspwkk.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2mmoaywzw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vdyodxfq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gihhchig.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ccxviqtx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vdhhxqap.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jtazglpd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vdqqeara.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nqzkiqds.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ialsifyj.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2hluiezyj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hgbjpttx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2snillonw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2gkrhivnf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2aiwspvqv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wbyxzhgy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gxetdlhf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2nrctxwrx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wvyovyee.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2leqdojzj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fxebnckr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2yrjjoyhg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fjacukda.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nmvmtcoc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hflcvetw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2wylotowl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2dbtteuzo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hanysxfu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2fgxgmyub.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbxivhll.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2orumtwsy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2bjcbeypx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2zbomfunk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ayjzopnx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2azzsjoeg.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qffegfwk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fjspgptu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2vigpysae.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lzaaaiwq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2yebyhiys.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vthmbxhq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2osslapvg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tfpyuslj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kcaqpqyp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2eihaamyu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2rqlxtdbp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wlqltrml.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fgybritx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2undioqdh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2eoelxkec.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bipaevnu.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gaxwaobc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2ihdhpltu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2siverlic.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2gpofofzs.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2scdmoswm.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2onqjlfyd.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2bblyrfda.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2idzeucka.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2aqsutkmw.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2utfavtqx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bwwznpxb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2scdwaupr.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2uzptqcjv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2udthxvaj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2zybfmcon.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2wlmpeotf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2tmgakgai.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2kdxxeifa.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2drhzrydj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zresgwbg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2kkrlzkhc.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2cuzxgjmj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fsvtyrbr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2knppcjrj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2zivrdfyx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2vtlrbynm.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qhrehydc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ipwxiidk.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2oenbgmmo.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2zwxeprxo.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2mwtgyyxf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fuedxdvo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2chcufybj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2kxhvlpmx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2kofvlapv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ogmhocfy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2adzufumv.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2odyqljmt.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ibklezqi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jupxriyo.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wdtpicqn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2asbowcgf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wztsmypm.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fprhtmgp.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2sgddlpbj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ptwlwdtb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vhyytvmw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2ecyaeqmj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2dpjwwvxq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2bytydwgv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2xkvxetjg.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2dpzttoxp.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2izxhmrrd.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2yptrzhxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eejohpoq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ysxyqkfb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgzzrqph.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2hyedsjwy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cnirifgf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2kvpjelst.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2pxdvrfii.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ypmssvsn.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wmicdiht.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2dhvgdtkk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2icphsovc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2wwuandcw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2qjkyosuy.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2olgcfthe.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2hwimlffm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2vsatwxmf.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2dapspgyz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tbvjppwg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2xzhloblo.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvfmznm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2jcivcrxe.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lfgnoxbi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xqvuvhmv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2jnpwhcty.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jztkojpg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kcxxysov.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wssglyni.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2xpxcgoqr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gevbgyci.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2abzunqlb.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2omervqep.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2skhzrksq.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pfigklay.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2dwqosrue.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vkujeojt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kgrgxjys.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2gurzggwv.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2hizpjafh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ysltmkdo.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2fdafatad.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2mjalhvek.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2zvxebway.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vrrqwoji.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zsxknqrn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ahdtlyzd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mfncswss.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2gmzhrmrp.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2zeijaizn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2ronqrdxk.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2kaixkoyx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2hevkuqjx.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2ditgcgqd.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ncprhjns.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2dymzpykx.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqfjjwpc.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2wplgslgo.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2eoywnlvk.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2guraeeap.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qargkdsx.html

PHP:  // 手写时间戳比较
来源：http://www.52xcode.cn/Article/details/gt2kkppijre.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2yyzygsbr.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2grikzxya.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2uokqvnbi.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2edxmdaeo.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2ufhjvwpy.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2mljsqjrn.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2peyorjkq.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2ezqsextz.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pgjezymt.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt2zpkctgdb.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt2htunsakw.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2caormpbc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2hpgiuobi.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2bqvmprye.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt2svxzpqon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ohnudcst.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.52xcode.cn/Article/details/gt2wacwkztj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnzggqlg.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2sgflgqxo.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2scgsdsxo.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cqkgvpte.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2htrgypcy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2gzdicjnl.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2qnijazen.html

);
来源：http://www.52xcode.cn/Article/details/gt2yioanhxw.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2hmnrmfyw.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt2xhdlgvdh.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2cshyvjnc.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2rupbxauq.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2gbagtwtd.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2cyvwmxue.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wowupezs.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2yxdgutxo.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2fzakcdev.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2cfcvbslk.html


<!-- 参考信息 -->