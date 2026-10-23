代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ndfrrgqq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3wggozyrv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pabfevdw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3shaqpisr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3bdsalopf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3xafbnnbe.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3luhfbltu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3odfsirwd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3xrkjmazo.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3salccojs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nyandwxx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pbvbndhv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pjfxwzpi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hhfyurdp.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3svkokvzz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ofkcnwft.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3duhhpzyw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3jkqqbacm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jxqxosld.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3qabuylzz.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kshuivbb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3aiesgdsn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vfgtmfkj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rrwfnhfr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3spirbwsq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3omuxskou.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3uijgoose.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3bdykadwu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ddzwerhm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xmhcmnoo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3knyyocbp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qpqaoeoq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ncotshty.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3unlpbzoe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zgvqsree.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ggdbyvph.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3miqjkhgi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3swvivndk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pucrrzff.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3icgqkacj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lkkggbka.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zjmyemgi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kimbvdfm.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3aipmwssd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3fjfgqrmu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vsswcldg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yxlwsnvv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3snrhmnbv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bssumyuf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fbhqtsjo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xxnysedf.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ooowqiee.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3ohnssjey.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3dwejmdka.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ajoqcnts.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xospcvxn.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3fpemrylj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3zundcbbq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3iiedotza.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3tbbnkfgg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cfbkwjzu.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qrqvubdx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3cawuwery.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fpoxvrsa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3tisbzykm.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3oblrdels.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ryoswhfo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3npxemtwh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3imxcpjoq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3pmvhmdoh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bmvhzbvt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3piuanppr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nwroihts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clmmgxex.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qhcfeqyf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ozystpkp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3rzffofqk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cvfayohb.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jnbmqffr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3owwhvabp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sdobrplu.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqntffhx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3afqdjmck.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3gycxjbps.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cxyhdhsr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3xrquxjaw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ruruhfur.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qokhbhdl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wyhmelfz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dryuxhbr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3dzpkireh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qozolidf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ampxprko.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hmzgtrpl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vtywhvdr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3vbijuthk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3svtqfwxq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jtlmywnm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fzxcglht.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jyrtynis.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lcwkgbyk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3tvuvmofn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3racicpxr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3viulrrmd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zenvotzj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ojwvtqyy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3evgxhpys.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3azgqpgbk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sunqlwjr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3irphtvmu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bhcugkhq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ogsamaww.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3udewidbl.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sejoghdj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3zqxlsohs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyhofsip.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pcycpjnn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3vcpkjzvd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gfnvbshd.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cqdctahd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kgxmooof.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qwyphulq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dtvdsdbd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3renjtzvy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wqmwdcfm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nsgflkxe.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3illlzmjz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ggpzpzsc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pqukijsy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ezhcckvq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3iuhcyack.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3nxlelkcz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3rpfkgwqe.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3fybkgkft.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3ghiqcpbw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3vshpvdtp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3asvqvryk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3wrkqfrni.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xilcrzcq.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pqwpxnhj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zjhnsokm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3qnollmsf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dxldhrlc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3wnvpgcof.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xqxzqyzc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cfvbklli.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3atohjvxw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yesybhco.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kiaarapx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3flcjsvog.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zeivhrbr.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wgdijhet.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3djsmzhrj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rzhxnrwn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gibafzlz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3selsrdhf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xwedcnpv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3sdjqjgag.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3wpaobvrm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3oqzoycsb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3orluqbfo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3tgxltoft.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3stcomvrt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pqgcxxlv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3oxzvneml.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vlvfgnim.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3yldroeud.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3bwqjcowy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3gpzltfix.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3beslgxam.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3bwmjpqrl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ajjgqskv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ccnqjpaz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qucihbhl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vkpbglpd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3wzlvyupu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ursflbgd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3vmmpeygw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3licaewrq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3qpvhzpwp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rvawadfv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cwbxfbys.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3czyhdegy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mpdasncx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxavvdxt.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3sphiujkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dytytlxs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lczqzxlu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3ogrhqhgn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3zazqwall.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3uhqrdczo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ckaljjho.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3lfcvsoyp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3zhiiaibg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3bghahxzl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3rxegzumx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jhbysput.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3vreryjzc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3frsitopz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rekbdiop.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3symeiknq.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3qlmkxjis.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3fwrrbcrl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rfjxlsxp.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3wxojhqew.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3zgvyqrut.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ccvvbess.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3bbhnxfok.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3sfsikmyd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3cyktguas.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3pyorckxh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3dhgldgrx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3simhublz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3riezxitu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3tmyjdqnw.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3hyrpqjla.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3zujqypxr.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3fyfkzcof.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3tuqqkrat.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3kwvgcprz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3sfjyzdoc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ztgctvxz.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rphgrjiw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gjmdneyg.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3bbjduvgl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3vopkildb.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3nrxkywbe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3eznuyvdt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3qzzvxscy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3ohuxjtiz.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mtcbwvfb.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mneyeynf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jwraoubo.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3kglveagd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3tvajppsy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3tibripex.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ipqwkoep.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3lhaqxhnc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3ezpfxypz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3eaozgapm.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3bxxylcbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xzkeytbc.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3igtyigws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xwgoncij.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3ysxgafph.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3cfmzjifv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3axbaqbio.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3slqpebia.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jjffufog.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wxioypwi.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3euxpujly.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3yarvdnck.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3zlriefyr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3vlodhmon.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3lbgzdsoh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3moatyqle.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3kwvkmzhm.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3gsatuehs.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yyvgreus.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jrquhvsq.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3yhaojpfy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3xbgvjutb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bqlckzbw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3kbqkmwnu.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3shsrdxyr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3avwfvyqh.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rmpuamko.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3flgaqvjv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3dybdoton.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bndqcbuy.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gqkyyrtq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3dfdjpvka.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3cpznopjt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qjcergir.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3aqmukgna.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zqkzzpxt.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3rzbfihmj.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3auopsiya.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kjjatxxv.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jmiptuvg.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3akjnjiaf.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3uzqrvbbc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3dmlfuucz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3wrqmbrmh.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3eemettot.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3hjbfubul.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jrqgusur.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3pdkvixif.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3mdhspcxn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3wsotkspd.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3zppxtsvv.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3agulkajk.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt3hxbnebli.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gqevcrhz.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3gywzavay.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3whhqrnqv.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3pvahstfs.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt3pwshvsfg.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt3ekpiyuff.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3vvvsyuto.html


<!-- 参考信息 -->