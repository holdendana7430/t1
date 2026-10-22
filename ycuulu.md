代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tivuehvk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ojgbqxpz.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2uebjupua.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2xomdahjq.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qvgkkrwa.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qnyikays.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2makzzxsi.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2svausnqm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hnasraid.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qmdptjii.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jaeqwcvm.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bhvwaqke.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jytixlog.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ylrjrzgj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2fdvtvmsk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ngyumshy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ctzuvaco.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2lcnoktks.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2phgdmmwr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mpkpvhpv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2poartciu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rpeauzmv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wijepecd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zcahikyn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2iucyoqgr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ozommake.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2gmcasqyw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rxxlfvde.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tpithmls.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2clprqcbl.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2nqgrfgmr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rkclhsmg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dzexuiet.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2rrjmqbet.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gpwpqnzo.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2otoopgdh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xeeorfuy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fwwunxxz.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcehasq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2lxckcubf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cisvycey.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nopdeimv.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2scduorqa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ictpgptn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2netayfok.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2puimpzzd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bgqedozz.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2atncmoxu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2cwawralh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ctddfggd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gdvelyzs.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tsnhvnnn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kfqbefil.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2qkrxmble.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ggnxqpga.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nirezyob.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xwnqhkso.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vqmftitm.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dmdtjpzv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2waqewytj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uxxlbaeu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rqujmwdw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2wjixphne.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wqebuqtl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fleaxidu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qzqjxykm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lrkqyzxu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2odzrzmzs.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2djouzzca.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wlbczhfa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rzgsodtu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jlxqihcc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bgnustjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rauuwxld.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ahmctkuo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvwffnxd.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2lmdkloww.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jvedlpit.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fysdjshe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qqlfjlsw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qgegehhh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rsvzaroj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lpqdulyg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jiuqorvb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ehhabcmj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qgagbtjc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ravncqgp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sszbefsv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vwlwapse.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dajxpkoc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2lnofyjog.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ogmpggki.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2lrstsvjr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jjwgvpcy.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gsnzbqyh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2mhvjobyh.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2dcqopsjn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2awzmomjp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2klbqdpjg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nuqitjdd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2buaehhpt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2platgbgr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ahkjfzgf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zipxokab.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kbhcjniy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2oavwtnel.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2afxmgmpn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cgatjniy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rxvatkud.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2psijobhr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2haufpllo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uyhrgdrt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ttoywdti.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2iwjmgrun.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlqwwnsk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xgjwlbdc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qnquciso.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cdgbqllr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2zxnoxkvt.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xzpferow.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2oytjrngi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ahlgyvml.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wtdacobk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2exujorlp.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ixlqprol.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qtzegywf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2iicezpkc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xbthxskf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ltshtbcy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nakrmzrf.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cigkpfnf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2sxbyuprs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2agihniue.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wprhbgou.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2zsbkfgfu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2baeeiwgo.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xvndllgx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uozbuzyx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2gepxvaim.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2aygbmcsc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjwsvadj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2anbqlpiu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rmpfdrhu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mciqsghl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dvrmwyqm.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lxkwstok.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qvwronfp.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2drnqvmgk.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eglzctjr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ynzxsutd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ycvpqbrq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kbofewen.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vulkufwh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2naqiqygl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xrlentqq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zdatpyzb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yoszkgis.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rbytltqj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gfrziguf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jameqhsz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2tmypvtuk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pegvnwpd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2spqzknnb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2vzjwcrci.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2utgdahmr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhrckzwe.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fkgdrsjv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2wbdyhzik.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2mcsccmzq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2asverjzs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zzuudhni.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yiftfdzo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tnfkxhdv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2hofeokhk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tvcwuqyl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2zqdoswpu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2hjbqjywt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2knxxbgnh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2epeuxrxy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ozpinaju.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rkqxtzft.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2stehxdzl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2depgojux.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zeygxxrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhuolbly.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lfsjditx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzqnghhe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2kcymmifk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2qqstklil.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2blviraxu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ljslunqi.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ruwdfqfq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hnagalks.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2khqzssld.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2iwpqzhap.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2yzipaxus.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2qqkutysq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2hqylcnno.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2fshdguqy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2jytdjwxl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ppoaiguf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jzzuisvy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2whcrqucp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2epvgdtxg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2joovfytb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2mhiprwzk.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2xhurlajr.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2kniebpun.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2odvcfqwv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2onayikym.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vgmfugmy.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2twhatvdb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2dpxnzdzh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbozboeb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qpgeqzsw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2xpgdqnan.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2fbamgtdf.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xemmalen.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2rzkefkvv.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2xtiikksk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2iqdczzmc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2nmurantt.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2ljrwothi.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hfczqbie.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2kwcrdsfw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2pwgtfksm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zwfqiydu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ldqwoiop.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2gcnemsgk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2bynflvmq.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2kecqgwcw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvpyfjkr.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2filbitrz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2vomktibe.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wdvnxqmw.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qkgdvsts.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2ilwqjmwc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2eyhpjewo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vpfmwtjf.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2rnhgdfad.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kehczdpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2okkjqvpo.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2xneqvexs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pimrkzjw.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2zevbnebr.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2woripsmx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qbluhjnj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qmsseuam.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jrxzqriq.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pxulztpk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2iyupwjlk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2lvtmncfv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ehmsctsr.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2lvyaeptj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2cnjzksev.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2jjilfmpi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2khanlpet.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2slguawmp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uvekjnbz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2znssdueg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qkhjovlt.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2zczevjko.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gykpjyfq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jbrchwof.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2hujgtfnf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2doaqpbzc.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kkilllhc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2hqxzkuil.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fbriswls.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ypunjtzm.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2korfhnnj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2nzynuibe.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2esdfdbnk.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2cluqgiwr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2khsjmkab.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2wjnainao.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qphhzchy.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2sluakjjb.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2syppakfc.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2yznridyp.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2oznpepko.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2ehzznvqw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2yaclunqw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2xgsmpsjc.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2zwzvocef.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ecxlrnxq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kjzdyzdp.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bljgpkgs.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2ahsshhau.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2hcsezkye.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2jvyrknwf.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2iswrsqdh.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2pqkysjek.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqmgeqzm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2aciqqusg.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2uufkipcs.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2aziprkbl.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2msxuntqa.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2tvmgzxoc.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.52xcode.cn/Article/details/gt2ystbecyp.html


<!-- 参考信息 -->