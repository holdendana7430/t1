代发 wailian999

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyvpfokc.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vfvrdtdp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nxtaxntm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2teavmjbv.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pifbtuqx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wvtruuvk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wnpfmala.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bywtnmlz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gckkfwww.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2faubpbpd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sfdzegdn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xozamtck.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2xxhntfeh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jgvwwtih.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2wggndbsz.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2azncvjuc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kvfyzkjq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2mciixokm.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tzkentth.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2apibydzd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yajitrul.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uzqhihcr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2axdntaex.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2fnjitlxa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ulhyfhut.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2idzgdynx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2qzjnbrse.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xcxaxpkd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2jrrgcyfb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2guiacykq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qgaijakv.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wjahfjjl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uwtveqxh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nhjtsycc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pywmjjbv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mlvjlxbj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2eosucjdi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wbpjfvhx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2flutikcj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ccczgomq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2myvhucyh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2opzgjldj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fyfqasej.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hurqxlee.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pwfpgvnp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2qtabxsri.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2idvagsnb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2qwpvjzcu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2saaippcy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bkhgeriv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bvkflmth.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fdyjccpo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2vbalwsqs.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2aofrmouk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rucdscby.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kqlijfff.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fipuftnh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jsrwmziu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rvlkvsry.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nyzvidro.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2tpjbkapv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nmosohtz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2fckzrzox.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2eeadpdps.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2nvljspqm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2siaxlggy.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2qctujvei.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ytxvcqfr.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gpflcbzf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2agtkbznl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vvhnmcar.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2aqchnnoa.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tcddvazc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rsntujjz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cpuywzdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbnncoiq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fnmlteci.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ekwoytyp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ltzgaguz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zrsopkgh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vgecxmqb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2vblyvadt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2llafufva.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2jwdffkyl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ldofvnqv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2lbdooflp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xburcjiy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jlefnxgx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2estkkpsr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bbjyjjik.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2qcfzhvkt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wpjfcorv.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ofiidzyq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2cwzkjesx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ikcfdvbt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tzzzqjpl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tqyojxoi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sgfaugnr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jezqfcdi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2sffpiwph.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2pxgzwpfr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2aggrqvso.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kerqmpry.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kiiotbjp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2syieucoj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bymdygea.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wtxdpwzk.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gswlhqoi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqduvoaq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2wdigtrih.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ypsuacut.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2dfiuetqi.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ttaqreke.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rwwiarqc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyazlrsg.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2evfdqzhc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qovqodmv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2canqaxqd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2klrtqemp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2uekdbybz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2vklzeynz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2wpfzcizi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cqwdnyxu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2adyxfbpo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fjqqfjsy.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2geudhcuk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oshiyqyk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2yfqifpis.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ygxgokmv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2vthloauj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fuokxzvz.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rglqsgxs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mdxtnzlh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2fueqvmon.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pxprwcsu.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lvkjidgx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2qgcogjls.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hszfiaho.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2epnbbnlx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ldvelhnv.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2oifhkjgc.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lwqkrnqx.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2levlswqf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2awxecfeo.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bgafxjfn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iuwuuezy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2voonafdu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sbwvfeic.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2kebcnhrn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rzuyjarc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pcxvnoai.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zwwtjuxa.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2zvkznsiy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rvabwwzm.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2thfsqxjj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tqqlvypl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2yhjvkpox.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nsmnnabg.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2mrorilsz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2cpisqeqx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qnahvxim.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ntmdarnw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2slwptjut.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vycmfxhn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2thckwccn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xbuuptsh.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2naebelec.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2hknjevig.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2pupwajrk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ngecemcr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2mgzgmmkb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqyouewx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xbbellhn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2rlutoaeo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ovyhbkje.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2xbfavwta.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dnbxdrat.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ymqwjvdd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zvruyavf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gxudfyll.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wvttioes.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2arslffpl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2iuuinbna.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nxqwhxvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rikngvqd.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2hxsqttkq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arrjwcaj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2sjthxgvq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2eshjbepf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrjaizag.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2bjqoxztx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eqjdzsty.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hyfmwvcc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2mizoolmh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2ppkjzrwl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2nkgfbaia.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2haiytadm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bjzfyhac.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2walptgbq.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hvsjcthq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hrkobutl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qfgkxcij.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2ekfrcjvy.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xeewfqkl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qblwosqs.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2cmqcehgl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2qisklzao.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2wrvfxtri.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pkjubfjo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yfqntlew.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2uqvjmjwu.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ogzbgpdq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2jpnjlnrv.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2iyyueffk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2meaosmri.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tgkxxflb.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2aopylwxq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2bvmdewfw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dlbzetwi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2njvgwugb.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qpcxepqo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2krnuehsd.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2geyjihii.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2nzoazebn.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2mjroxgvz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2cvurigco.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jhpvddwq.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zwiicqhl.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2whhcusua.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2wlagfyul.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2cjoffcvk.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2qdxohtzb.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2dqghvzik.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2yavwaipj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2rivldjhj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2youhxgtn.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2skwuects.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2cjggqdej.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wtrpxtkl.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yankqtfe.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qlkjiyhl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofzkgtbm.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kjwlkonn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqgqevsb.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2azrmwziv.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2csagkmkl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2euyfauab.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2mlvrkqkz.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2guzbmysn.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ljfwfwou.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2tuxxpwms.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2hnhteyjr.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2caccjphc.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gtmsxaru.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2fmevyeui.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jvlzxhvj.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2cgfyyvrb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2xisgjlat.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uybebmos.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2mytiujcf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2rwgkysup.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mgcrjkth.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2exchilnb.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2dwwmtdgp.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2udbrmkic.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2srmmxsgm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vtrdekct.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ukvykcvl.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2vsknjikj.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2ovrnojus.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2dmdzqgdm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2skkbjbkd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ehdbcvsj.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mzazpmrw.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2xoarapkt.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2haxphirp.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2rsqmwhtb.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2aznvalwp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2mquhojtn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vsxemniw.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2gxndlcde.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2zaeqbuxe.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2gznoireb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lnasrtcr.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2wlzkitsp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xzzhgsjl.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ewugtfsx.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2hliixpzi.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2uorsnxda.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt2nwebsxmv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2blnqmxmy.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2uigtfrxe.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2wmtlimoo.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2uplwiskm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vzntgexf.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2sebmyytu.html

Ruby: if x.nil? || (x.respond_to?(:empty?) && x.empty?)
来源：http://www.ydjk.org.cn/Article/details/gt2lnjzoawa.html

C#:   if (x is null) {}
来源：http://www.52xcode.cn/Article/details/gt2fdilysej.html

[P07] 防抖与节流
来源：http://www.52xcode.cn/Article/details/gt2htvdyxsh.html

Py:   # 用装饰器 + threading.Timer 实现；或 functools.lru_cache 做缓存
来源：http://www.ydjk.org.cn/Article/details/gt2rkxobann.html


<!-- 参考信息 -->