代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2upbwmfmk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lhadmuqq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2faycavri.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ychkmsgw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ewofzlxw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fqiirqjh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qfbefonu.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2agnlukta.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2llgjsynt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2rewngemn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zevetppf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vtasmfih.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2pdtqsagd.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2irxkgvzs.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2oyodnzej.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ipgdzcff.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2aknuihtg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ttrqqqwv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2haqbwemg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2pibwmxnt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2attaiiuc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ldbtcovb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gcqoxscl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2fyyjnnkb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2thgluqkf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mrdunfgc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2kvnjhtcq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kiohvxjo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hscxsoac.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tukzqbob.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2sgnixphi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qcvjijrh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wdlbdcyz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2otlpkqxf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2xwbutgzt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2geajcxor.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2nnrwszjk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lpegxogb.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dkjthqhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tgfmifol.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hhjneihx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vvnqmkzu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vitenosa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2sntfmdpm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qlcgnyln.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxhiropz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iowqmgvf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ttmoyfgf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vbqwugsm.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jzwxphiq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hdfoilrd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2hcsnpyjo.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jgpdgcvg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kfsuasfc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kcshwokt.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ojxzuxyf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2trexxiex.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zrstvisa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zezoxzfb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nfdfrpxs.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xkkssmrg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2irkjmrpe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mcdrjnnx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zoooeaxw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2dkesokbe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2allhehfd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2gayqaolr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wyazphqr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2iihtjxbh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jrwquaxw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zononkrn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2zhpotzrq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2eaeximjm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wwowixvd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2vzspuabq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2bbmterse.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2hsvxeqig.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gjmmfdvl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ncnlaivi.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2drmoauxb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qevqzthk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2vfuhuukq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tftnsejz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjnbdzy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2lrqhmluj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2bjhmehgt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zkjtrytt.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2exltyagn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2czfnzifu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cradmikh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2hdibnbsp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2bwxwnwce.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qmkunuzi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2stvueuuu.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2lpainrnt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gduakwae.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2lxntkgse.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mjlftpqd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2apbfcyat.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bfxkkann.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2urmpmseg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2apdcuttu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mxqnbasb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2pkrqouhg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2zloewues.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2hpbfsult.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uitslmpr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bcqftjqv.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bwykspxr.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xuvjggwp.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2pwjvkgwu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2njbysvyp.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2owwfwtnh.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2fajzcqrp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vnqraywr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zjryofkl.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dadrynjy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2erinecpl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2cpgdycat.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2luvcywke.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2qgqfwmxr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2njvkoljv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2inejaluk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tzijsjun.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2wfkimenq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zeuesyfg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2zfrnhtjd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mxzrwils.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2mxbcceur.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2wkqeympd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mvekjbgc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ocuadzaq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzvofbwy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qxftvlst.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2kzluwrtp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2amfzyrpk.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2lpubunjk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xkvfjfvi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jicresbq.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2iipxpscc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rescwgei.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2holkgbah.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2kvgaolkh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ywtsmgnh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nsawqxfw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hiuvkxwd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2wkafkwcb.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2myohoxav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ivetqjaa.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2wqutfwlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vlkjgsna.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2zyvfnuih.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2hlzuzqxu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2lyjstize.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2btlmviqu.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yjilsmwv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2nmcqzsyh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dtbgoiyi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ohhruovk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2qkopbiuo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2rznduqwf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkjetuo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rrdfyita.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jjqbsxus.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mxafbmso.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2krmktfkf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2flqddnwt.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xklcnulp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2gzaxgxfk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ghtvhooz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ibsvxlwg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2hkkdshyk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2vrjnfcgf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2twlxqemc.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnorrrjp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2eaauvkgf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2pwswokvy.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pfzupmpp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ninlbjtz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2cfqpylda.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2mgqklmgo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fsskbgiz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zpckivbh.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2njnhxdrp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jvyzrhzz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2gpbepwfv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2anxdzevi.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2epibfdpr.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mcrtyncl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ygdrsnks.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2gvbaozly.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2flbrdadk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2sskmxjxy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2myszpwjz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2yyvwsygx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2lvhvhwqt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2phlsnflx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2buioqfvc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2sqibkebu.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gugauyjs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2iytjmzod.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2dvydjyaz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2qktxwsdj.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2kywwqwnp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2zauiylvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tggsurdp.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2eeqpcndf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2igenazsa.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2iazgevft.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2tfdmshvk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2izfnakio.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2cszldjzt.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2akwxtsap.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ibknoync.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fpwutntv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ovvhfhkq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2vouxcrww.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2mkfvvwxt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2uaiopxrw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wrmupjyj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2bgrmqher.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hqokrtzb.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xndijoca.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2esaafcpd.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kpqbsoih.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2gccrxkei.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tayyqmub.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2zyoktkyx.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2esbgchhd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2chezfwru.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zabrapow.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lgnnffkh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2plswoyqv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cwzwhonk.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2tlyheicw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2mazfkuhv.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cbcacpve.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mhaebvte.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2uqpozvbn.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2cdtfrwrp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ezhdytak.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ouynisar.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2dhtzldjn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ngvwohgv.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rqxntavf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2oprwvqwt.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2tnexmapl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2wdupjqqn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ibxpalyp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2rpnsjjon.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2wtdovqqz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2kcjzdfjq.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2mljdcxlr.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2cahbihxj.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2qcgcdyqe.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmtmhpcp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2oxmegldt.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uswpwlge.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tfztfgva.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2divouiwj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ecttyqvu.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sjjrdsat.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2uaybedhp.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2fnjsakoy.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2fulcfyun.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2nymwujcf.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2wohffuwv.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2gvdfvdwc.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2itoncclq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2xmtcsstn.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2rjfbnsgi.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2lcbumyik.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxnkydk.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zdsxvewl.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2srkyxskq.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2pvuyompf.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2qmcxoooh.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2rbseqtln.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2zvslnsxb.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2loxxjtpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dpdgwhjw.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2iqbdpwlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2twystlms.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2xsmypaks.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2bbeovadr.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2rvzcqfvs.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2vsuidgpk.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2rcuhhyfy.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2sshxevji.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2qflzutwk.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2goftvcbi.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2bgyfugsw.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2hnntmuwj.html

user_id INT NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2pjficezs.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2gkydeqpu.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.52xcode.cn/Article/details/gt2snqbhsdj.html

);
来源：http://www.52xcode.cn/Article/details/gt2vhkfjcef.html

[Q03] 增加列
来源：http://www.ydjk.org.cn/Article/details/gt2zzfxfghj.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kpxdueql.html

[Q04] 修改列类型
来源：http://www.52xcode.cn/Article/details/gt2kiqakars.html


<!-- 参考信息 -->