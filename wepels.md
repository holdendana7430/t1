代发 wailian999

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3sbxstbsx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3hwrgqrmw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zgbkione.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eyqbpgwy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3vwcfdjgy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3begdhnuz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3aorhiytq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3zgckuzvb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hztobges.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wswtuuvg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3yzlvgrhp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mdatgeoy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gthurufj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3gmioxxqn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pdijanvg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3bsrivskr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3zkkmxmtm.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xvhjtxph.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ldvbdjhi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ilrybhrg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oplevsnd.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywebzpam.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3glgqrvue.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cadmyrdj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3alwmacyy.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vrpubrqq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3edlqsoak.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebmhociy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vkzsvzkm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3aqnpkiwd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3decxblhf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3epdjoheb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3gvvlfjel.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jvgvkvtc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3umsbjsur.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3mairyozb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3vnosavan.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3vawwuxex.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lrvwlwoa.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zrkhxezl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3mcielqwg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rvcdcrjp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3wcjyvlmn.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lacuulvb.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3bjtixkqp.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mpztrvft.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3cwpuzwoi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3siemneys.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3szllwbxv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ehruxaww.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3hqmhzeff.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3pkhupqhj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3pgxrepyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xakjyveh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3klnsbtwu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fhyegbfb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jslklhpd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kidjnskz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nptpaemt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3pociwwvu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3iyxmsgyh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3unmbnzpd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gwzfiwdj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ajnzwaso.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rceomjuw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3dqnkdgas.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3kdnskpge.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qjdqkvos.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3qyfznvtf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3sbdrcwqc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qnogfpjb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tyskvomq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qawtisxi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3diafoyib.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3evnrnvqa.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3wnajkeyi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3iuoamrva.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jiwuwgcl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lbzwkxmd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hccxevjm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ahrxrijq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3taknvuyo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jbwavbvn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nirtrydi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rmxemgnc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3odsafejb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mpxnjvbj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fsjjkbwj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pxxsccmu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3uaxyragt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tnnjfjdz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fmielsod.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fowgqagx.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3dnlgzvrk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rqpnahav.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3otuzrobz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3hiczldsj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gtflqfoa.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zpurbxbf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3youetrmh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3nisuotla.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3aygnehsf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3cuwtohji.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kwbicvoj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qldrmtld.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3niezzvad.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3serxrbbp.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3dufumjfl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mupyiucs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ifcmzmbt.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3tdciggzj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3nedmvxyl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nbvhbbmq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3wgkljsqw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3sxapxjvj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fflvrzqi.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jwzmmepu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ybkkhfsd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3cozvkhcd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3iajzifmp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3tqgpycap.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zguitqwz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3salyzjla.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iowbqsvv.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nuycjvvz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gygxptdm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gedfjvmz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3icmvjlnn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3xpjlhcxn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3wlfysdpr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ccrpwuzv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vbuodayn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jocdcxpj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3huquexee.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ipgtcmtg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gznnkpzf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hlbhwyas.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bzgmijyg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jbenyflf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlnzmwee.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ljekhrot.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rkyrzagj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3piafypsy.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3tqlvkuah.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3yqwqohox.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3kwxgolwd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3owibantm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3iiuqvgdc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3wgmrqwoa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gqandepi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wlcxxtrh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ctosfgfd.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xkcekiaq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uzetsfez.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fjotsaql.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vlthddjz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3dpxttsxu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jqtuuaej.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qzolcvrw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3xdckpldv.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jsvdkfuy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3xmkqrmot.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3klsrcmnh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3hsszbzex.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lhuccnpt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3smzlfcde.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tdlgitkz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3nrqqqnqi.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3dluzcwks.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3cxrpyuwb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3fpvxnbdn.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gqqocesx.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3oyawsmzq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3mqvyzsri.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3biypfkkl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wjdtlxtq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3aekjvidn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3rftpqrdl.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3lcljramt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3refkfgls.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3rfcwhdbo.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3aodufveo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ydiusvho.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3ystftjfv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ouqlhwas.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3mlreidnk.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivzqpaua.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3lixtxftt.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3zmorehku.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3emgxyuir.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3djrocvuo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3neojauvh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3xmvjufpr.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3mckkxlxx.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3erbmkamr.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3udocbjhg.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3lpgdgqld.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgcjfuhj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bfleobir.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3laanjklg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3jpbtliih.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3gabamojd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3zvtwefrf.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3zlqopduf.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3zxyxsrdl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3iiflvxih.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yldiaucy.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3kuykecfn.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kmqcnwny.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3leixybmm.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xjdcuiyu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3vvhzpeug.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3stqppgar.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jwplvzmq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3qbedrncs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3srcatsxq.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uqosijhl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ftrxyhtw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vxtezvgr.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3oaqqjbgk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3zttpsubg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ljubffrk.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3eaohrctw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3awumfqvp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3thrwyuvg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3bippduoc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fqcnixug.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3nvhptmjt.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3pivvapij.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kxilaljc.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3amiubozb.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3uyuwmbqj.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3qwjhoxuv.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3nkfwuhbv.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3qivbiuvf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3nwtglamk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yhyuvycx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3hqjifgbu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gzohrsjv.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3bbabvpix.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3acymvele.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3rcyhuxxj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3iuejwuaf.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3ojtnmjup.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3jlxqiidh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3hgbnqeeq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3xudnmlsl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oqyvrbaf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3jcrslygr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3djvyxhya.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gxsugsvf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3flmxhzmo.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3zksrfkcj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hzgpjjjo.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3gbbjpilv.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ofykcffz.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3juoraklh.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kltqqzcu.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3djygnzid.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3mhohewtn.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3yziidvvv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3exbildik.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3vpcaiwzu.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3gnrljqpr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3puynkcqx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3fzvdikla.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nacwqxxw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3osakshyj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3zrxikoni.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ibfedada.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3gnaqcgcs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3isrkmqah.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3qohjltcg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3qpsxbalq.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nlelpzqa.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3tjbyfhac.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt3zsscqlls.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zcrxjniv.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3kefcyeln.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt3tzflhqla.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3tlywflag.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ckqliknx.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3ckwdpfxa.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt3tlshzlfu.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt3vmvoudiy.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.52xcode.cn/Article/details/gt3sfordxxf.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt3lumziyna.html

[P08] 处理浮点精度问题
来源：http://www.ydjk.org.cn/Article/details/gt3grusmztz.html

Py:   Decimal("0.1") + Decimal("0.2");  round(0.1 + 0.2, 10)
来源：http://www.ydjk.org.cn/Article/details/gt3fvfymdap.html

PHP:  bcadd("0.1", "0.2", 2);
来源：http://www.ydjk.org.cn/Article/details/gt3reyroscg.html

JS:   (0.1 + 0.2).toFixed(2);  Math.round((0.1 + 0.2) * 100) / 100
来源：http://www.ydjk.org.cn/Article/details/gt3znpcwcov.html

TS:   (0.1 + 0.2).toFixed(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fzlmzmpo.html

Java: BigDecimal.valueOf(0.1).add(BigDecimal.valueOf(0.2))
来源：http://www.ydjk.org.cn/Article/details/gt3jllrtwuf.html

Go:   math/big.Float，或全部换算成整数分再算
来源：http://www.52xcode.cn/Article/details/gt3didhbybo.html

Ruby: BigDecimal("0.1") + BigDecimal("0.2")
来源：http://www.ydjk.org.cn/Article/details/gt3whfcengv.html

C#:   decimal d = 0.1m + 0.2m;      // decimal 为精确十进制
来源：http://www.ydjk.org.cn/Article/details/gt3owpciyhb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3msxvwryt.html

Q. SQL 专题（以 MySQL 8 为主，附 PostgreSQL 差异）
来源：http://www.ydjk.org.cn/Article/details/gt3ggmxtoms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtxyvioh.html

[Q01] 创建表
来源：http://www.52xcode.cn/Article/details/gt3xjqdpnij.html


<!-- 参考信息 -->