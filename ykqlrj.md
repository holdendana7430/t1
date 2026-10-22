代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmwksnks.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2qqacqjls.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qqffpfhq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ywjylgch.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2blieurlb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpmbatcf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hsbhdlfm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tzvoejfz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hbotqwje.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kztfwqhs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2dvombptk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kmahvyfl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xymwvizq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lptcdhdl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gvjjrxng.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2apzlpavv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2npcrrlqn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ebkxdfdi.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ufarsosc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2svzglrdp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ddkvefrp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2loqygpin.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vuqxrxsu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lgakkwuf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rbmlxnjd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2tbcgdknf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ptmrrazt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2iyedqtsn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2duxxnmbl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2gsbbdznh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pxrtrmdx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2enohbkid.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2egoooirl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2xpaevmxa.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ozneynjm.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2iuogcpmf.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2inbfjkup.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2aswvrjff.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpyonwyu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ydxublqy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dvqkuonn.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ixsrbfmc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gqlnkodx.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxotzyyi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2irmeooyj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dtlgpcuf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gswofcbi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2njxprieq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ftkpzbzl.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xotthnzb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2izvlqcia.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bccspics.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wvdsvmto.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xhnopxer.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2apzsxybn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2lpxaxjef.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wdgxyfrk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2vagcqmdc.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2xubeemuv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nwgppdix.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ujifzdak.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2wugqkfym.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2efpymgwb.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ntbasflo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nhhpzjqr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xatvvjhm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2bcimlgoc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2mtwmgtxz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2lejqkppm.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ygbgztzi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ulpbolgh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dtwqvgzm.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2yubgowww.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yezvrrnr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2pgjkemqk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ovistmzj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2wpcqkddr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2epwhybou.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2imcpnydj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ghqhroyc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dbpwviis.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2skgrmtuc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mcxtxdfv.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2gtkufxwl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wycyahlw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jwefabnx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2qervsufs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2cndjcvqt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2clhtnotf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2lakvwfaq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wajjtvto.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2spdespks.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wpdldgxy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2qbuuhmwi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2npwpigrp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ddmhrgmt.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2aoyhisrc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ojfjykcy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2echkiveu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jactgobg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hnkjobzq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2evkejzvu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2dmdlbsre.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nqzfdaeb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2srhugdvc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fygaserg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kiqzfnyg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uupyhqsa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2dpemrxsc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2colvmssc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2einkmlar.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yxduldix.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2toyguszd.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yyfjjogb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fixcevrk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hyejaexu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kzfidmib.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2xoefrzfb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qoxpwyfx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2bwkojrfz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2jtvtnbiz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2sccxhifu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2amdzcxns.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sqhsmnkv.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rdbikfcn.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eambqfgk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2btwdptvk.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kxewecoi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2doxhojbz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kdnywwct.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ydawrsvv.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kkqyvshq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2yrxqwklg.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vwvpoasl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2eiguecji.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2sacuyxmk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zpezlayr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2djydyfgk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2paswznus.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2zcpdogww.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ovshlgef.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2uonxhxav.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2scblcqxp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2enrlhdpg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jbeavqya.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2exixuwvs.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ywvsvgbm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rhqdbsma.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2upmjfmjj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sknmbvah.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pcgajmuk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2waqoljpd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gglyppfq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2wadbsvaz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2nquwuwkx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2batfdier.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2jyudblbt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xqfzvvab.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vhosdpyc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ekdexpcu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2orneazjb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vnwzfthr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vqnwdxho.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2qxbuvpig.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2inzmngty.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2laghpazs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yscudphw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2kvlpxytk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2svicvclf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2eukonelk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2belbyjbc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jfbjolyu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ldzhecgp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kdmcuumt.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fqbunjem.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iiczmzqk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2gjmofzxh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2njytwjga.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qwibphzf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vjfrnksm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ptvxjgka.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bhrvnysm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ihyjpmwf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2axaksdad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ajihwwjv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cwwifgfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2enkecscg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vtcbhpvv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2krmxptte.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jsbwuluw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2rfjviiuy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ourjmhko.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yspjollz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2rkrekfjp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2jjcgqois.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2knidlasu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2vcnvotdv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2immgxrvp.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2olqwhczp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ikxhmsqr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2fihlixbx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2tizqwgyj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2bpvcrjin.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ipowtrtq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2jjetghue.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2wszzsuad.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ykaetbfc.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2qjoswklv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2ocluldlc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kitdteoc.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2qvfyyqxo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2caysspbb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2fvcgibxl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zbwojaez.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2plklhugf.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2opeeuuck.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2cdwszkgd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtxopvvt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrqjalvj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kwphuhvu.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2nfxzngas.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2wxuqugcj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugmluqxl.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2hkxczhae.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fhtmcupm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2ivgcelzu.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2pgqwkikb.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2psouxeth.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ukedlmqo.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2efptirim.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bhgublzc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2zmoihlay.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qycuvhpf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2uferyiqw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2knqpndil.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2nqikdwqn.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xfukxciy.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2nhcyvdnc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ivugorol.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2pwfftgne.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2devbsgjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgtpjote.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2nkyjwagv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgmvjqwg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ixactbxn.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2hflcymmr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2apggpxsq.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bbqhpfby.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2lfniwazz.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qbjnqewy.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2golazrpe.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2mtiygyzb.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2eiexgmyk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2kfuzxvmi.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2zvnigpyr.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2wvtnwglu.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2azhjzbnq.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2lukexmya.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jkujmfbt.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2sfsharov.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2vobwonop.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2udckojnn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mgruhfek.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2issluetd.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ogfqxbfh.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2mjihyiep.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xanmpqrm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dadhfxdb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2yblwdahr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2gdkkmyoz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2hvvwrkvc.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2xdxtiksy.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2xtbwymph.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xcwmlcuj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2fxppqtnu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2rltybwjs.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2otcxlwek.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ojpgyjtb.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2lospmvkr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fsdvprvq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2mpzssudo.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wiruaaog.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2txrewfga.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2ayhdydxw.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbiumdvx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wrtpahuf.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2faiwwjjz.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vwqxljbj.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2czxquldh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2mldgsibt.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2ohtcyvlf.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2udkxdmsc.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt2zwikrigg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2wwvubilx.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxamboja.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2iqnvgpto.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbeaptv.html

C#:   if (x is null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2objxvqrl.html

[P07] 防抖与节流
来源：http://www.ydjk.org.cn/Article/details/gt2ezkfofix.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2oomqutrk.html


<!-- 参考信息 -->