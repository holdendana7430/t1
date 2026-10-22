代发 wailian999

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2emcdeqjx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2gkrjuxna.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kauuwbni.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2opagwmpl.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tbcfjrnq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyyjfkqh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbqehptd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlxdburf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gxvdzqps.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xsplvcsk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2zejiltkp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rvgqawnd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2iwzxvejf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2utsbnhlm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cffvhjkr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2whcccenr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2genlcbul.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2viewfeie.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2uxojscji.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2akoqbhik.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2iedwrnyg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2cbdmmxxq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2bzfbwrhz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xkxzzuim.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kxsmovxl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qdggpwem.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2birqcyal.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2subsmemo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2cddeupga.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2uypiitzh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xiicfmce.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2safiwiyp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ogxvgfan.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2avcwmsfg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rvqrrajk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2sirxmduy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2utjfocvh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbhzwbxg.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jzsyvpfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2efabhhmq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2odzhrlza.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2adyqxfjy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jpdgndbt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zcqnyuyy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dbdmiyvg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2njbrzfqq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxffwqah.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rlxdbhit.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iihioggq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kbuebfuz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lntrqxbo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2uqdxtspj.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rkqgibrn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zqdtkahe.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2rqffctcs.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cjourcvb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ebbdjkjr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rqgeozgm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nobwfdag.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2oenffina.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2yzvcjayb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2swaphlnw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dhtxytmw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iqpieaoi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2cmpdlnqi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2sstpwanj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2acjioccq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2mjzvsjjv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2tufdtled.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2axegoiex.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xwscmxtd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uzxtteqp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yuevrzpc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2gqpzdnyo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2nhgpqbqo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2afjspzba.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jsvrosks.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2jjhjfrvm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2fodxjnhk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2mbuxdctk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ljzyvoal.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wkirhiqu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dwjykzxj.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2zgnmoznu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vkyjiapy.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2hqcdfxyt.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2jqkrghyo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mteobttd.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zxtdmkka.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2otmtzhge.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wzmjzdvv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cmeqxmhy.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wijpxsjw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2mjyyhtcj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2clrrfjvp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2kkfgtmhx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wbgrsqof.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2oromghco.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2oqnnngad.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2oxggdldb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2csmredie.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tbdvqvvt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2vnsvcaut.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tdphzvwy.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbkmnyfu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2ikbunghl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nruysaub.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2txxdbvrt.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ymuocwkn.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2afzhjnli.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cntrcqto.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qacsgpne.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rymipynm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2klvhfobh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xzjrdtto.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nhcqkdve.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2hyocmcgx.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fnoynfju.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2rdppxmne.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jyvxztzm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2whyitjds.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2tkedeqpz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2euefctex.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2dllgrmbz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzqdwxlp.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2peocputu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2kiedbgav.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pedeomiz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2zkpzhiob.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2orxpvgpe.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vqcdoxwm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dfegawux.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2dlanwasy.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mkassute.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hozlvung.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xnuwnfwf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jmfuppmy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2sagsbxur.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2teoofnzm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pebockgd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ghmuygxx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2gciaglko.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mrtcnuor.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yfczckyh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2tezbxvfo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2asrtbdox.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gymzknsk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nxzbvhbz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ifmhwclv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2opstkooh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kgsowuqd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2wwurijhn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2tbrrglck.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kyvwjmpd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nxtnckli.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bdgdxpid.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jijqssjx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2nsjtyxwx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2tytudyrm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2gdvehdvh.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2fixsnnhr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ljbmdkvy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2kcvbbroj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2mfhbgaqr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ftikxfsj.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2bpsylzcj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2madsdlxw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2kjqzssst.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bmxnwtyk.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hdcnfecg.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2orduzcyd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ooovnvrn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2qvttsiqg.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hpgcnufp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xnkprfwj.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qeutixuc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2odmrumef.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxxucohh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2flvedwov.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2zarvvnof.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ichwecky.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gtzcijsz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2dbwyvvuv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zkiawgpy.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2eqnpstpf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2aegqfwfd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2otofamjq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2vowtyrho.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2msbxqasq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2iulnbcpw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zlfmmboh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sttxtcun.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2vkzrfpbe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2hxljpbnp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kwqxxqxv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2lsawnsmu.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2pftytdxi.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vqitpxkj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2mibberlk.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2zwdtcfbb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2khmmhghn.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2trukbqfc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2hejgmtrc.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2pcdxpckf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2vlxcmsta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zoatllqy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ctzazdqp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tfhhcsia.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ntcjjyss.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ahuutany.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rzvdzbqs.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ofzxekck.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2umdyxkgu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2kguyxksh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yrilsmvs.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2peuxvsbq.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2udmuneqw.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2wyrpmwrm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2amwrrzol.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2voyxbllw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zoetcwwy.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nisvraey.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dawcboeu.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2whkszmmn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gmiurtif.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2rqacwuvw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qasmrmut.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2iszraizd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2vhileong.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2zmkmrvki.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ekaghksu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2lggckwng.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2crdrqmqy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2hsbfbafr.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rjsuacvf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2sroisfai.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rsmhfmjn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mwweopvs.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2stxbtled.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2kbporefk.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jilncqyk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2oafycgfu.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2aaddxgsy.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lwojsqjk.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2wwgujndg.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2qodvfgsw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bvvrsbsi.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ofeojmif.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2sbrzutpk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2mapcudgo.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2pakllcem.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2syxkcynn.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2vqlutyiw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2ngcjynls.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2buwbjojy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2yhhhooru.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2bwxyxcci.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mlkgpnnz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2itcaynnc.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2cjnqlnzm.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2ufuexxmt.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2bnnmcrnj.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2hfxjexor.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2nlsgigoz.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2qeemeahz.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2sezfjaqk.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2obirrnps.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejtylxpy.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt2uyamqjcr.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt2kbrakake.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2tbhcabpv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2biajvsnh.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt2alwlgljr.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cztrwewp.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2efziedkt.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2bbnaexac.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt2czdnwaqi.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt2kszbgdyk.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2hqivwyyi.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2mdsacagm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nekjfppm.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2wwpjdqru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwzndnno.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2dgzxxxty.html

CREATE TABLE users (
来源：http://www.52xcode.cn/Article/details/gt2aqnalqwp.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.ydjk.org.cn/Article/details/gt2nvhuujdt.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2dodscosy.html

email VARCHAR(100) UNIQUE,
来源：http://www.52xcode.cn/Article/details/gt2zniffmwh.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.ydjk.org.cn/Article/details/gt2ytgaydrc.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2wgvlrlsj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2eqpkuwhe.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2qsqqloza.html

id BIGINT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2cxmfyqjv.html

user_id INT NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt2sqhhiwza.html

amount DECIMAL(10, 2),
来源：http://www.ydjk.org.cn/Article/details/gt2nfmibymf.html

FOREIGN KEY (user_id) REFERENCES users(id)
来源：http://www.ydjk.org.cn/Article/details/gt2zvughkoq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2vncnbewy.html

[Q03] 增加列
来源：http://www.52xcode.cn/Article/details/gt2qmykcbvk.html

ALTER TABLE users ADD COLUMN age INT DEFAULT 0;
来源：http://www.52xcode.cn/Article/details/gt2njvsasun.html

[Q04] 修改列类型
来源：http://www.ydjk.org.cn/Article/details/gt2lpxvnham.html


<!-- 参考信息 -->