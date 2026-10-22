代发 wailian999

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2rmcwxcce.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2eczgmrtb.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2msvoeehk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2tisxcsbr.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2eulemzef.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ihbtqbzd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2jnsqlquu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2dytoqqqw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xqlhzwqy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2mhpveljl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbtebghc.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ptebtmtr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2grpplluc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2znlumogo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qhhlyxcg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2esazudaw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2llrzvxve.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dbqjwydw.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2xmacsowa.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jgwkjwlv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2totifuaa.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wiotteef.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xbfqqreh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ayaiyfco.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2pigvocmt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2jwcjaihc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2iianqawg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2hsgliaif.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2iljakggu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ylqkvwgg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rqhgmeia.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zvdmvzah.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2umdlfazx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kcwguhty.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2gscjigjs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bqxnkatg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2vhtjydwz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ifdbhbcp.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2wrmydmvo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vrgxhicg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2swmisywc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2etedsucy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pjbqenee.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ccpufyoi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2vpumigzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yffvqczq.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2bnjtcsxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qufwhxas.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zhmoteuh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eanblriu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ytuuvaao.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ciuvypob.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mkygezbm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2alydorch.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpwbobvl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rfadtajd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqfznqhv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2befuzlml.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fgerujby.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fkivjmos.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iywlbsvb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2maaybucg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2mzfnpcbc.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2yqvyfuwu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jpumwrmg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2mucqcjch.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2pfnnnqix.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ncxcmblr.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2oldpamlw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qkiiyjyg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ligrqyva.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bbxrfvsi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jeqqjxab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bjwuonyd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2srimyszr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kgqkjttj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xhazbsxh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2gskrwqgq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wywmltju.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2emujuyre.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jhchlrby.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2alicruct.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lwnmdabk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2awkjqojx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vbnooxut.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oovmessu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ohsmwtmb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lwfeycyn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2srvtfmgf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2nduewiaf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ymzactvt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2rtwzqlbb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yrthudqj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2uzyysodo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zbblefvm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2puwlgftr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2oqwymers.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jzojwuhb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2naikrwmb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jmjvaxsu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nzxecrvf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2tzdurytd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2banlpobi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ufmmdqwl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2yakqofcr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rtjzyafs.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2lapyvbwl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2pdebqneg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2oekgxlfg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ovfgoiai.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2blvnmjkd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ywmxixhv.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tzbpiwhb.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gdtnsapp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gobqyidp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2noinbyty.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2imiwnjah.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rhmpurvi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cpumogko.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2epkcrkvn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bcvbtsys.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wujxlrit.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2isodezpz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bozidqsb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ucmdskqy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uvubdraz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2bwkdwcht.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kxnwujge.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2azpjvdgc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rakllrcq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2eksldysr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2migaehps.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2elmtlqen.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2adgcaofi.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xyjnchgx.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2iwtddcjj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wmumkckx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2mjpxgchs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2whfozwth.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ungghfel.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2nykkxjwo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2pckudabm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ygndifov.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ylfrwbso.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nfqefaqo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vkocugur.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hohbhtcf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ovsmuuch.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2clgkfjot.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2dlwnmgxs.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2urwgkfna.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xmkztnde.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rmnfpuyo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bahcnrud.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kjopfvde.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dgbbyenx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fserqhmv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2bcabjifs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftrygcmv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2earyrmxw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jlywzbtb.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yzrksvgw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jnowqiqo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tnnszwhp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2yowyhfvl.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lryktkmz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2rbwlumlf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fmvpuymo.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2dufwhilf.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2lihvijli.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yijmyyqf.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jlsqapfw.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2eyahnnhd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2xqnherml.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2avedujvc.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ugcycvuz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jpnoreye.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2vxihiwyh.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cywmvlsd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ixxnipuy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ynoslayr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gdjpvgfk.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2munmoazl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ggskgjzh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ljnguupn.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ybpmtqpb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2candzfpn.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2kilttete.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2wherscma.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2gpvspuap.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2uiyqhcdc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2cgbmfzri.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2oyfeiqon.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2rufilbnr.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2hwyphffy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2eisvbyrg.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2meeyjcwc.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2czuqoaxp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2xugrvkit.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2femgtngz.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2cvyqrgks.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2iciwujrg.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2lhfabbef.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2sspuwkvo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ppcqrhzq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2fugwqwhc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cxpzemsu.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zlyxxokx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2krwciaqd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kgaonloi.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kpcwdwor.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2cqtablwf.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2avxzschn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kssmmbgr.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xcfdgnut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgliaufr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2pgcghxvr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2cgdwkajk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nljbzvrd.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qyidorjh.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2hlxzkjeq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rvopvvro.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hduopyiw.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2fsdvnpjw.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2hixuicqk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2pmwfsxii.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2swonffzp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yzykmggx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qbcttavr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2hjpwscaj.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ndupmgxt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2rxxfkhfl.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2qsmiiaeu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qewiuxxu.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zouabxhe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2raprykul.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2reqjzbnj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ddslhgvs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vszbvznt.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ddrjwxcl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2hymavrqf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2jwdvsvzy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2gexqznnu.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vkowtjsq.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2vbqwmics.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pzmtcfbi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jqdaxjfo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2amsqncaq.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2dqeejruk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2egupbwiu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2jhfoueol.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2svzpeoaj.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2qiayxqvh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2qyzpchqa.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2kyivuatx.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2vovqxbmf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgxmccly.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2sguilwvh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yscmjkza.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2jknexkzg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2qupuqwtk.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2etbbtpyl.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2yebjkwvx.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2qmdkgcwu.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2wnndoeqp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddoqthxo.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vtgmezuw.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2dxlupuyk.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2fnzewhhj.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2stpcojyw.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ciwzglzb.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2qskrqmdv.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2nvlvzfia.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qidomctx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2qnhetebo.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ttlixrjp.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2onhhhtpd.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2fxhkbgjr.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt2pyxnzvva.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt2khzolxnc.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt2brthpwyt.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.52xcode.cn/Article/details/gt2nfwggovj.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt2akrlgeec.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt2jltqaooj.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.52xcode.cn/Article/details/gt2lfkojwgc.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt2qzipsjiq.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.52xcode.cn/Article/details/gt2nmjcayht.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt2xqstkbne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cedydptn.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt2xsbczjdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubhtrcpb.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt2qbnierdv.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt2nrcmzami.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt2sxontopr.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt2atmibrnt.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt2rtgqwdar.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt2rlfrdlxq.html

);
来源：http://www.ydjk.org.cn/Article/details/gt2imwkvpzj.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt2mmblnbnb.html

CREATE TABLE orders (
来源：http://www.ydjk.org.cn/Article/details/gt2snajlkuc.html


<!-- 参考信息 -->