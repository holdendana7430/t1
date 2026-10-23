代发 wailian999

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3tbzgsumn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xihlqjcy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3oaatjzog.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qfadbhno.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wjonkjzg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jcugbnfq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jzlnxnic.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hzhxnkbb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3xvqlcxqi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3bgdifyjq.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ntumxumt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3wqmmfzna.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgwkrbwc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wmaxdagp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hwtryatx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bzygxotk.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3hjhjknje.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3foeboloy.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3tdbakauz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3xyrzfezz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ejsfmoww.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mgaadgvy.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kuplwkyt.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qtyaypjh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3dgkrnxqg.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3awzuqgqh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3iszpmmlv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3nmtfcrrb.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wosnieih.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wqtzhslh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3oeozlnat.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3sqjuhlls.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rxobramg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3njdhlgpg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3rswyxbpk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3kebevqye.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cskhqcpz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3yqcsylfq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3pcdggtof.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ypbhzuqp.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3nbnlkndj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lhfxppsp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ttzmbvjo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3zqbmoqhp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3clunxtxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3givwazcn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3lbnuljkw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igcettzy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3yoljodth.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhiantdg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tlvdlgcg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zdqlymtk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hekvhmkv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bfjqitqo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ogrkrnyr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3submsnwn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmshcgn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3odfsyuwl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3gtflxsmr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3ncdtbanw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3mfvrynfy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jqwbkwlx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3wufbpqwv.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ptctuvmg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3rxfqsjon.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3pelzzuhj.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3kyonybfg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3psginuts.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3wkmfivfn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3usxvyxsz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3gdiswrox.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3uypyivun.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ynxruqtk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3twyuuyhx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ihyeyehw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3jkpjyins.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhrpebfs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pusvpopa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lgaiaxte.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3gcieagum.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pucqjydw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kxphfafm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3hhaxzzol.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3imniwslw.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3wihyicqe.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3idpwazqw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipdssgfc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dwzuxuth.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jncymyzz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tocuiuby.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3fdlgdgqo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3unsvqjtj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ivgroiat.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fjmuvgtd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ekosppcf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tgsuvnue.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gkvqalom.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3xblrbxwf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3uiygdqfv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3srojvmkg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3fzxsicnu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uezycmdy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3aogvzlar.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fhdppufj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ujuowdga.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3stghyhod.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ewgflqgo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3fonypxpw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ehvegdfs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3sjdhmdxr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3rbieihgc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zhwzuluu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wzjtrgub.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3wbltxvbl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3oxmgfcqa.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3flzyznon.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zkxkuntu.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lqdqgkyb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lmmwdrfe.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3slgawpuy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3agpilnch.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3tpmfwjda.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3rgrcbgck.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gadgiyfj.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3egyoaghj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nojvzuyk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3oodftipe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ydojyxyj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3vujmwrsf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3fmgpvqpu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fycfrxgj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3kiwspbif.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bqygazri.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3deziogsh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3czxrbpkb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3xjbqecbu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3blvthkkw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3rhtzpetr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eudjgacn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qepnuipz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fdrdtokz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3oltibssz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3duarrmey.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mmqlrkeq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ozlfpccy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3oqewzise.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cmudnsfk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3fvzqagbd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3gepdsuow.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3dumntoft.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zqjctmdt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cejkuost.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3stefyeqc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nlqlwyzn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gwkzopmk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qfhiqbra.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzbehuji.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3kympydne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3txiuulwv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ulmmgrrn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3qtopxaxz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3louqoffz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3maaarlop.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3korxhlck.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3jxwqbiso.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3hnfilbod.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3otnrlnyd.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ejoiajgq.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3oehozntu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kmxzfpff.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3uhkipeog.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3abtslrwv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fmseogfr.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jlfrgtyz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3lgxkrrdk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3momrwvzf.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wzzboqxe.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vivtqdww.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3cnoqlkjj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3dpbtcloh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kkjfcdwm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ikxbbwpp.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3rkmcnkfl.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3ntnysmur.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3tqhxrzwc.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3eoqzoxpd.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dfzrkxkh.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3kzmjgnxz.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3numjacpc.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3hesrpbaw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3uooetwfi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ngnkeqtc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3dpxfzkpl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3pifhofqf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3yeyukjfu.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3bivtiayv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uaoeqmwx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3tkrkjovc.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3fnnkwywc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3baggmnpj.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3gvvvqgrb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3vdcpwnsx.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wmsmbbkt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lavgebrc.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3ysswydrm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3wxulgtud.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ncmueobn.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3hubzfdpv.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3dzizusev.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fyfqddri.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3leztxmwn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3vnyfvjpy.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3cykhzygo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3snlbxjdv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rowysgdx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nsfihfei.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ylsvsucw.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dxvvrysu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3hakxumnn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3naptegpg.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3lrtjrdkf.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kosqgocq.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3xpjxysbu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3rpgevnyj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3sjkaohxb.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3ddsiuvvp.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3ezqlhxsr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3wazmjaix.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vklpxaim.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3mbzqfnim.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kxmdjmit.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3qlxqcljg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kfznyyof.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ztnsuwza.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zuhisenc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3yyjsadzb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3kdsoridc.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3whskolrk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lpzhvixg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bytcuuvs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3xjruozdv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ocvehfin.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3tdbknlxp.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3vikjylua.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3mmvjsqxb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lizifpak.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qgftqdzm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3urqjuecp.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3gvmmzlbd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3mptxhjnn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3xqochthz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vqyfpgig.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3gtmzuzta.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jjqondkp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3fywnhith.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3oashqjqc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3atwmcmfr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3yatxstud.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jreucpqb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3cdxlracs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3llhnrngh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3yqczorkg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3ypvezozm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3egyhoogs.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3atxehbuh.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3smglbouc.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cervoibh.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3sfngxcfw.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3jzvyzcpz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fzizlyxq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3qqhdlrka.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3syqqkyvc.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3ulbpjhxk.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt3jbqkqscp.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3rtdhzdyi.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3lcamlixz.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3qnlncrwp.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3ugwenavz.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3ifbczhob.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3icaqmmrr.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.52xcode.cn/Article/details/gt3orcsxgmv.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jevjkljb.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.52xcode.cn/Article/details/gt3hdbukqcy.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.52xcode.cn/Article/details/gt3marhaqza.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3iaxvqthb.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.ydjk.org.cn/Article/details/gt3nhfiyomp.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3mxdgwmfc.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.52xcode.cn/Article/details/gt3roesrbdv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bypeubpi.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3bdldxurw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvjknpux.html

[Q01] 创建表
来源：http://www.ydjk.org.cn/Article/details/gt3fhllxhwy.html

CREATE TABLE users (
来源：http://www.ydjk.org.cn/Article/details/gt3qwmilnoc.html

id INT PRIMARY KEY AUTO_INCREMENT,
来源：http://www.52xcode.cn/Article/details/gt3tofwinvf.html

name VARCHAR(50) NOT NULL,
来源：http://www.52xcode.cn/Article/details/gt3ergwqtfl.html

email VARCHAR(100) UNIQUE,
来源：http://www.ydjk.org.cn/Article/details/gt3zhmqfitk.html

created_at DATETIME DEFAULT CURRENT_TIMESTAMP
来源：http://www.52xcode.cn/Article/details/gt3nycjlopz.html

);
来源：http://www.52xcode.cn/Article/details/gt3lmdbtush.html

[Q02] 创建带外键的表
来源：http://www.ydjk.org.cn/Article/details/gt3ifxjsyhe.html

CREATE TABLE orders (
来源：http://www.52xcode.cn/Article/details/gt3wfvvroud.html


<!-- 参考信息 -->