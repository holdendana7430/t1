代发 wailian999

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3oechorvg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3djgufjyh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3tcpagkms.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vlrotmyt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3adbgoltu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tsxdebrp.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qgcysmyf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dizzhdyb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3lxgkzrzn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3vjbkpgwu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3grypxwqo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3xkqdaegp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hsmwcdwi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ckitkzkr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3gkfhugrt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rymcavlx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ltnoagrj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3yzybizjw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cxkhmeyb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3eogyqgrw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3cxdrxtfe.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bqhmikue.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3awwqdyhd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3deftbnbr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qypeeqfp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rotjhqsu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zokgzheh.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3omnjbawt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vokfjjgr.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3usdsgrea.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yijpvlof.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3uvswpbcp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3peolimmi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iljhkbou.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jzwgkvce.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3tghvbsiz.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3iowguhwz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3djkzumbo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3wqurtreq.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3jqiqfcsr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tthnbpze.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ajaqamzi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3znvyvmjd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ypfdgzpt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bvklfawi.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3htikzmjo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rrxeaerr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3lgyrgmqz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3xalepeyl.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3yhvdbcpo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mlkiaghg.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mdokipjl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3wqcosbic.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lxxclqlg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3jcihvnln.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3stwbftqz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3exrrxgrh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3shsoqcwr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fwwqcboc.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ucrocdkh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3srqsyadt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3mbsdsumt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dtvagpzd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bpxmrxzj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3yaystvsw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uzyxmwkw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3tanxjtsq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ievyynwr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3esbgdpxk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtpkwfmc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ivknwxtp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3igvssooq.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3admdpegm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kmwmgwlj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3buqcvywz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3onuygyza.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mtjpyttg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3yhgbbhyq.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3lzzqbzcz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hjrdvvyi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3canawuce.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ugmyymem.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3ezwfibih.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3tnmorjek.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qlqqcpye.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3bzxywbzd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ssrfesgc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ojjmhksk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tmckliyo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ubtvezzq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ojmrqofj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3btglpnuv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jgogdlpr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3telmxifz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3dxmphdpj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3oxrlylkc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3uyyfyvdi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pqrjcibh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zaafyioo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ehgusuhm.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3njzdxooe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3wlqgeybj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pyvgeaff.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3liwkhqnk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3yryrfhao.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3yweciwdc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3rykujggb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3dwzykwwk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ipgmcneu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3hetoxjhz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3sjteyojb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dvqwmfjq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3qvkfagvt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3mskahqyt.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wnxuhcga.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3uvrxlyni.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ibtcixky.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yljtiote.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3brjmdwgm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3nmqpigpc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3jeuzxvqz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ntqamqda.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3txxcjiro.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3glqjwwlz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pybsfruw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3tpuhdtgr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3jzkxwfdj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3tjrwoktv.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3kvyauvap.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3culvwhyc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3qgpbllkr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3pmwjmudj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zqlktfda.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3fxsuahzi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3axbwrxoe.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zndzqdty.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ljqeobzp.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gnzsccvv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cfcpudgg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qtlwgkyh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fhyjhcmw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dtqtivhq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3utyqepxt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jzztvmba.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3sdbokogv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3uhdthhed.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ujotqmwt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oakhvtlm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3lskiemzw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fxjiozuj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kemvauaf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3bmaltwuq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3lrhwunhg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3exwchedv.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjovjxag.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ikxwxvhh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3amuotopq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mrbwlstd.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3xakugymw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ottaezeu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3zarcdhww.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3dzitrhlr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qacvsfwk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yhommbub.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3slqmgnby.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3fegasffq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3saphrpdn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3lnfeugtu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3zmamhmxb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3nddijbqj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3yvfoyoxi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ssalgrzl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3unarhnim.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mhdlqidm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qbpifnfz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jecphngs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmawacuq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3mxqivccv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zwphmvhh.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3ofdmzvta.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dyxerbfv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fkgncyee.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3dlsbfowh.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3lrqmrnst.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zzsdqrvu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3ankbthyx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3sfhpljhv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3eeaqwwoe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3nmvcczkk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3iyrlmgne.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3guhawbia.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3dvdzoqnk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3mnnactkt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3uawyyqss.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bpxhhlzu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qjlhqzlx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xikbuljf.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3vjdavshq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3oruiamyw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3bctmdrlg.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3venxnomw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fopirbhr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fqzywvxx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3oytaotvf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vweauvom.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmyspupt.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3bgllvglz.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3invmhmwl.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bkzkjkmk.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3svzrqwwu.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3euyoegcc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tsevpcja.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3mseiwrll.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3ctivygbt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gyecnmcn.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3islkzpzq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3iorgfwof.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3uhvhszdd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3zicwiuhe.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3qurrpvlm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3eaqhdbsv.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3aycoplft.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3bjlqgshc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3umgghmxj.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3pzpqoovc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3nfknajno.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3neqqjmue.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3vffdevwm.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qalnbham.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3hahlcjik.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3cxfxpold.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3hdnbvxlk.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3nsiycuvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vuktbyfb.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3mlvvaztc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gvdhaubk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3umbfidkd.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3qbsfzhjz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bncmgqwv.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3mbjfanbv.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vvdiboxh.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cjcaiiyh.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3mrbdavhg.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3wbwdbavp.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3dlmllaxi.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3kyprpfaq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mymlaafm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rrsaittg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3zyzwphcb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3pjqdjwde.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3jftsafvc.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3ioqigkzn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xgosiqqj.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3qzfkehjw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3pudkkcsb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jwyydyyv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3cakikppr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3cwliirmo.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3fqiucenm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wftvxelh.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3qzvsarlu.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3utwdtptq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3xmyygtcq.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3emxxelni.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3txjlqpaz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ucomdnqv.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3zohjrggc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3fetxvxiu.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jnadbvyd.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3kayplvee.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3mogsudmd.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3puhenxdt.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3lmzfgplz.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3plkjuyql.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3sdrtskem.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3qmisyrgk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3qsvblaww.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt3mrbwmoeh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hfzdcpen.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3iecduzgf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3whdsfmbp.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3iippnfkv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3vhkcnvqb.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3fkfsuqjg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3dfzhvyqk.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt3mqrywbrr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pusdwtvh.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt3zrrsgykj.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.52xcode.cn/Article/details/gt3orkimyzz.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzncgugp.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt3dtppuuet.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt3jofueiip.html

PHP:  // 手写时间戳比较
来源：http://www.ydjk.org.cn/Article/details/gt3pufhogfq.html

JS:   const debounce = (fn, ms) => { let t; return (...a) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3syryygcd.html

TS:   const debounce = <A extends unknown[]>(fn: (...a: A) => void, ms: number) => { let t: ReturnType<typeof setTimeout>; return (...a: A) => { clearTimeout(t); t = setTimeout(() => fn(...a), ms); }; };
来源：http://www.52xcode.cn/Article/details/gt3tpzkkwwq.html

Java: long last = 0;  if (now - last > ms) { last = now; run(); }
来源：http://www.ydjk.org.cn/Article/details/gt3uujefpjv.html

Go:   time.AfterFunc 实现，或用带缓冲 channel 丢弃
来源：http://www.52xcode.cn/Article/details/gt3dpedeggv.html

Ruby: // 手写闭包 + Time.now 判断
来源：http://www.ydjk.org.cn/Article/details/gt3wcotkxrt.html

C#:   // 用 System.Timers.Timer 重置实现
来源：http://www.52xcode.cn/Article/details/gt3sdddeocv.html

[P08] 处理浮点精度问题
来源：http://www.52xcode.cn/Article/details/gt3aszoxmat.html


<!-- 参考信息 -->