代发 wailian999

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fyvdulem.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3exlblflj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3kegbvquc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xidekagu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cyhjryuo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bycejmfj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bujzwjdj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hxgixsch.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ijxhvtjs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3nwnaqdwh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sjtltcpa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3mqhzjrgj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3txmgcwwv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3uqxwdzic.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jiaivbew.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3otblhano.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lpgrftmq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pflpmblv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3apzkuapj.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fxixksua.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3apshgwpt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3wntlqwri.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ryyqufzt.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3eildlwkc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sicdqekb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bkfaaede.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rorxjjtt.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pnymvlmy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wljkhwmv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gxbsxfqy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3nmlndvqp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ciwlnqtl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3bacejayf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3hfebvskl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xjyvkfme.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dlaxioca.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3swnkennz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3razpntlu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3kdwglsne.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rqpfgjpk.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3cmlvmsvb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3oymisgez.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3yxouyymf.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pfklnudv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3okbbabcp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3joezqdqj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3vuryyukz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3aktziedj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3vdihyrjp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlfjdvrt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rgmrzcfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jzssonmr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3igegdvol.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gqzoyrue.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uauevtrn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xszrkrsq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qwkfrxxb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lepocujs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rhvgkrxb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3njuvijqa.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rwrnhkhu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3xjwerhfg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vewqztlc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ummqiked.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3fmdsdsoy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3utkukjie.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3uxvhbftm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3goyqsnbw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3idizulrs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bidkmdiv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3sryghexd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3vgrxbdpk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3vvxthswr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3kedpdfvq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3xsvtrjje.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qunvvotp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jnnuwzah.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3kqbyabkn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3ltxsinww.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ywnresta.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uqntgvnq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aabypbmk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zbijtouy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xetnfzuv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ohnjcuyp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3qvlkxeln.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3myqnsbop.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3egdoitus.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lgnnoeuq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dmbyotrf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uuclpthz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgnvyhsd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dhvwxiuo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kiywmcrb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3otekapfi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zwsuwavo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3qtbujtis.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3knskunzk.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3beqxkzhq.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zkbulygu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ulhgvxzr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3urcmxzpo.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3mhozqhry.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lrmiavcs.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3frmamlgy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3beiwxlhr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ebhvaciw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3ovgaudtq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nhofopxk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wonoltga.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3tcywxxld.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3byzemmcg.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3uaqlcvlo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3yspmyntb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hvmrkpzi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3txtzrgsz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sqjrgsgw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3kjzzkmzb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3clyeqoml.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3awrddygb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iczltfdx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xvxlekuk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xgslcwkk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fzunoekf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3sapjeldc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ryxenlbm.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ipknvzqj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zrvuqrqy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3vhuwhokd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hnassvbt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3dpkiikrb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ufdzftbw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dpekexzv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3oubigvtu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3tkrywxcy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3pdaxwvdi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3wmhtscnb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cczglulo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3cubfmjyl.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3vgidobge.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3uavitkbc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3jtjoueyf.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ezmsfdjv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3iaisrcvz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3kbcxwbqf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3scaywure.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jwcutvxo.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xzpzhryb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nlxkeyjg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xcnzlnkd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3dekinmar.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fevclorm.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3dfbsuuzw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3bopjvewu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cwpbecfe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3mzduvapm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3vjmgymrg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3claeweep.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vawgbamu.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3obdrfmjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3viiqtnyo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3wautpkrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qmpfulzu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3rsuplcgm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3vbliyqhh.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3oqbwvffk.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3pgdcksej.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lbgybmix.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3icumgcqd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ctvijudo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ruuebywc.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3azgnmcgc.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3tetnwegk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ralnuwbu.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3fmkjgzkj.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xsheqbql.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tyfmvyha.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3kfqfpdcv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3vvxtbjdj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3qxkocort.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3lgmsuidb.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wukktvsp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3sdqtwmup.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3zclztbsn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3ppomrgdk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zgauczgl.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3amgucnos.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3yvfwomjk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3ntfqtfsf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ogldfabd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hlicazfp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3wszswdly.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zhsbnwgc.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybgnyluo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffiobrbn.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3xiowuxnf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3wimndqli.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3vvcwhzqn.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3civbkkoa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yngedyjc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3kjtkdmtj.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3lfmidkbp.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qgunkmxi.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfqwcsc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kggjiffg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3uixycfor.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hliilutd.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xjoemjqe.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vtvbqowy.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3tlqngpjk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ykadudzh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rpbpwvdp.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rswrpecy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tuapmove.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3fwntruxi.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3zgerfrin.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3wacuxhgi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnjpsbqq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghiqlddm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wexquhtp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3favbwieh.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3folhubju.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3jslgokml.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3sldbtxvb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3xhstbjez.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pklnrnwg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3rxluxjrr.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3nvoyrgjt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3mswavlso.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ojknbznt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ajxsvbpz.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pxgbombf.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3lapiquzp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3iwxfphxz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3cmdtdsyg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3crivlupn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xnuevurp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cywnwmdc.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xnmnmkjz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ikhguoax.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3zguvmczx.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mcbgglje.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3imajlbxb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3kpiylpim.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3timficoy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3yshbwgzh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3twaqwnxk.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3fvvagyfx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3updyaoae.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3zgfnijde.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nxfuvugd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3dupjfont.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ujvytylp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3gtxgwaqf.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3vrktwljt.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3rdiiwlii.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3rlsqtkqm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3qhbpxdsv.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hmfkncww.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3zziduerf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3jcghvsre.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3nalrlodm.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3qmurnbds.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3xufuhhan.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3kumkwyhw.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3pzkehjrv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3xcffuyfk.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzkduxoc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3cloyeefc.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mknymono.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gwylpuqt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3dovqlnin.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3lousdgdb.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3osdibqrd.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3nulvohcn.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3zsolbiec.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3bcqnwsrs.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3adyegroz.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3mjtwlucz.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3rkhzmhjo.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3snooonnb.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ibbhpaak.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3zfaaguxz.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3eqdyqbur.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3hvksgtxm.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jdckficd.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3vjofhvin.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3hcdsxrtz.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3bieietkw.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3rnrvjugd.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3qsdvfyug.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3mxytymbs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3obythmqv.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3jrzdsrey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jozwjzqy.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3usawvgrc.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3ynuouccl.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3nslnnzwd.html

name VARCHAR(50) NOT NULL,
来源：http://www.ydjk.org.cn/Article/details/gt3mqygjjlr.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3codkeyww.html


<!-- 参考信息 -->