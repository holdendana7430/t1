代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zvcyhknz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lhhvfxhs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kowsewjx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zdkyfjaq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pjdxvwba.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cirdycsj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qwhgqzox.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rxzxzsjg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ycvdckdu.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2avernstx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jwopofgt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zibaxxpu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zdehujkn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uplhplfy.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jjepfpgn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oirlsxov.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2nnnbzjyf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uwhxdwhl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tslhlecx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2emqrnfcd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ygarzvyq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vfagvhjn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2trtydddk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2huvkckrh.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hppzlwiq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qtgnmhjk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xnftupdr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ytzbjzlb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dgylhsxs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2apxosagx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2peblohoy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2qxusteij.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2okikywpr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lfqiqgly.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mvaimozg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2attydcli.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2zaqxtmvz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jwqrqucq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2yakhxyom.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2idysijvm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2mkjanmex.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xdypmrbb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tldnpbbs.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2lelcqbdj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qbyxjsgt.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2upfrryvo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2izoisyhm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mahajfep.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bcnoxnel.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2mpokrvzo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2jsbkavjh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ghyefucu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dxuysrpz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bjpdnzui.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2sqhcnzgk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqykzva.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2zgonwyqk.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xdygiuqk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2xthksoxz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hejuvkld.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2rzxztdcs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fnfrfypt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2amwlnzhb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ytgwshja.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jvswqghr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jjarbqfn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ulnnaqzo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dianwucl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2rtzjrpvc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zwrwkzqn.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2snymfglb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bmvgqirg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zqkmyvpt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ldvsnuef.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwczfmc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2goqfnafg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xapeahur.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2sjafyoni.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ryikvrip.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2kcajgzse.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ozrnywoq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qseciamb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2hqkddirx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qztymgtd.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xhtnnvwv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dszykida.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2xsoerubn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vtopolzl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2qtwsvpqw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ykfezbuj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rfyttckp.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2lavzqllo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2tdgvmbrh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dklculsn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qzqmfwzx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2samwvvdy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fczhpvtc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2okblavcn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yfjnmwlc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2vqxwhkao.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2prsricvb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2svoliwcf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bnxzpgro.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dvomixti.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ctlzwiex.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qjioilnz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2sfbbwskl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pwnenpps.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2oohicpph.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2wcoxhvjr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hkuektcf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2dyeysrru.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2czrzucxj.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jjvxqnvo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2iyjdhqec.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yzvojfwp.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gufmcrnj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2edhfreen.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2alwnaclg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gpolygzt.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lrxzuhkx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ricivgmh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2ussjkgkq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2nwwkyxiw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2eebkpfkk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2tqxzwfxq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gnzzkaje.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2sheittqa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jfgbompf.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2mzigpgnc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vsmxarhs.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2gcecycsx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2pwniufcg.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2urvqfvnp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nyfuqzbg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rlczsgek.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ftgicrsx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wcuvrqwu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sfhrzcox.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hgwdcrxd.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vwezomrg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2vjkumgpy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wimpvwng.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hwebdaux.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rgxjnvez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ugmizvkg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2awdfhxxu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jxdmwcxr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2akwjokqy.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2zeescybd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2cwjsralh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xlpeqksr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2drzhxwpv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2mbanxawq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lsaqzpnf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2phemyqek.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2khqbpfyj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qdmglfqd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mooksiem.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2lnkvbkwq.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dynwrnls.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yebhdica.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bsglbpnr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2gmmzvzlr.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hxtenqio.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jacotxuj.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lafzhagj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2wbhgfzlu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2bowvzkmp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2pgrjwdkm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mhxewojz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dkwvbszp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ttfzrcvu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ostflaox.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2uyryspwh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2kguganvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mftxoogs.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fnajssvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cswiczaw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hkwumvht.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lklrxkwr.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2znkkwqek.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2pgjopjqz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ryvmzoqs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2vxyynesl.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2hwxvgpsf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nkcptxgy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ftwpubhy.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kllllihr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nkmpqioy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2nyzcilbz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2cqptrddf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pvyrscaw.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2siljnmqv.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2lrcgzaus.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2wgmbclbs.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2oacdyzyj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ktjmacng.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2jvegehyj.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lxfhynbh.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2oweffbla.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nnhjxctr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xkxdytro.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2tzensdpg.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2svmlnoob.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qyzemfrb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2znekudnc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2uqqkqlbi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2jeqeiavq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2gfawftbt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtatnpfc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zmuwsbzo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ppwlxsed.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2xonesobf.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xvgdegvm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nuhthell.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kioeqjpk.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2crwyklpi.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jlvlxmum.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pqgcopon.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fedvrdtb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2xkkyyfbn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2vxavmtvx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2gmgfyxax.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qagukeyp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2gkxecmeq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2jrkphhqf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2luufqkwx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fyftidxc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2vnyzhrou.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2rrmfhoky.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2rzsxjynz.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2jlghfmyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqeprqbe.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2uxcyjxnd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfgqhqtn.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2rpisjtpi.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2uqwqftxe.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2bbgdhtph.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2hcihvxzq.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wdwvqlrd.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fhoytmbv.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rsxjwvox.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2givekepf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ahxvbbdh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2dhvzgrqh.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ahbnoqog.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wscrcjoi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2pwhzhxkc.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cmfavaik.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hbdzagja.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2foycgrml.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ogqvzhns.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fqarkpzk.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2xzitykuk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2sppshxqf.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hrfjmnzj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wqdagzdi.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2ziaoimhu.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gvbrflfi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2mudkehzi.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ffrtupxh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2amquglyv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2agtesrut.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2rrpdmkhj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2nlndwolx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2crdgjwbc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2edthzjxn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2knorzirq.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rlptbfel.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gigjjopi.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xlfhddzz.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vmspwjhr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2yexqylup.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2bynldfyb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2ayscdhwc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2gikgwofk.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2tejatten.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cchiwyne.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2dnsprysg.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2aaarxgzl.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2rywwvkfu.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jrrqhifo.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbspytau.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2mkxzvsnp.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kwlzdezr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpfnkouf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2duhdxoiz.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt2virzzeit.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dfkxdseq.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2yrkafogz.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rlmwmmcl.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt2zrztmhme.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt2mmfyrwfc.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.ydjk.org.cn/Article/details/gt2oxrbhnhb.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.52xcode.cn/Article/details/gt2samqixbq.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.ydjk.org.cn/Article/details/gt2qyocqpoq.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt2noujxxpg.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.ydjk.org.cn/Article/details/gt2frngjoaa.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt2trqgfbro.html


<!-- 参考信息 -->