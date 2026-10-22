代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hvxmmzhm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jnapiqlz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgrnrjfh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xvmvczba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kdoflqog.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xjsitpya.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tgfbotsd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2umivljia.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nbtampja.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cyflriqd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ffyuhiot.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bhlxpgzu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2uwugukrd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gyazzrmu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nxjrvkqo.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wkvmhtra.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vuocgqsn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ckkgdqzh.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rgbqkcie.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2esnjdusu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jaccxalk.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ecgoxtfb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tlvbksqe.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zdvwzffu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mpyraubf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ynlapqqr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gvkgspwl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rdeofuhx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2citprqol.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vudfhoai.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ypnunuvv.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2rwxhgxfz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2utnlrlmr.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zclkzjai.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xqpgqkys.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dpiecctu.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bnhzadtf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vkxlmvtf.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ocepzong.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mwwoeqhh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2siklbzbo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2nrjigroz.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ootdzujx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2djqzgtmw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehsloyzk.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ockqmksw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vvybzfpm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vdrhafbd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2cpigwqbi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kgbrucgr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2afugmnll.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2llvofdnr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ygukjkwe.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ckrvezgq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xsblvmau.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dznsxzoq.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fshtyjmg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ziygegfd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2imsfseij.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2zuunxvif.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sylrykig.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pzsvbjne.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2encahamv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lnxtlgfa.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eodelfzq.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qshkidhx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xsuthieh.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jupjebom.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ujcfifbw.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2xlxrpsmd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2culyytez.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tniqhsmm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ybgqnrdf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2kmdvssos.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2wpcwfxba.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ifljxdme.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xppxtosv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jfowhctl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2nfhjjbus.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrlwfjhj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ogpvvggq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgkdddde.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pucyuscw.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xgwfkory.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pzshyalr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fumwqzjy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2okhnrtay.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wugvdmrd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2skdhdrsb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2cjzdvrmd.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hvqwvgxz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2itpgmsen.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wrjeugwf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2virockdq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vfoytqxe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mvtkhtbx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wdxjawgl.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2drhzcexy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ractfvgh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ayicatlu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2anyekttb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oqsxlpkp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2adijdjqh.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2wxigqhbe.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2wxhepnwi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2oyeyxxft.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2loeqtzvp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hezvawil.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2boojafyh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xoqzaeav.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dqocqplr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yeegjxyn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tckfdykd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hgvefijh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mtbofhve.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2imlmgppd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2llszvcjd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bhohvsnh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kbtbnhng.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qksonmft.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tumwdmqx.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cukbqljr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2filbyjbi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2mddvjbxc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2smhwlfwc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rrnfygue.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xkjucgyo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2lnotgfes.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lwrdddaa.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cklrpwhu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qrjuxbrh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ectmdvdo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wmmiuiyt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ndplmggb.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wlgcytsr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2mjjpqfab.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2egezcbck.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lmqlfhsb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wlxwyerm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ntasieze.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2flpjvfnn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2pdorcgkj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2zqqryfvc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2vjwtsozw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hojtjrxw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2pimoewdc.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2njkpgyev.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mmamhxqg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eomqmlrx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qypwxrku.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vluimimb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2feejlhvm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2cqblubto.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2azvqwhde.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mybblzon.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jxmtvsjg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ugxnauie.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hglbxkbx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2mtkjkdkv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2devoybou.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2lpeumpqw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rpujpzcl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ntqtzzbv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2nawcbgjz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xlbwjtvo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2svpzmxsk.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mciacmxb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2hmighokx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vcfagpeq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2tstakekv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gibungdy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rwxhohlf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2qdhuamtx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2htjekcgz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2nxelwixq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tznxgtsb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cqptlykk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bjomepva.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zgieylpb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xzqfsruo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2getpgjhg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2tukkssqi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wuqvmzde.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uanhvzbb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2prdbogov.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2xhjkyroa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yywohzxs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xkmnotvu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltzkcaxh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2cdfevmuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbofhxjw.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fuoxztpx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2siqpuymx.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qrhnzwgr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2camwlhgv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2telixhhb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xuoqrfsm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2geqrvvfe.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2djwdghfh.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2bonpcirb.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2efaaqgrm.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2awfdgkdg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2goyqncrk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2caxkrpmr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2gwrkbpqp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vqkwofaz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2xcshovti.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2rydqwkdt.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2hgfooegg.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2jafaemhz.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2pacasmlg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2mopczboe.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2wnetanid.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jmslnoof.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zqeytcef.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2ueiglpjb.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2yelgjczd.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2krrddkhc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wpibrlum.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2tnpcqyce.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2njnbowcz.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jumlouig.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wkzcagxb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2zfcholex.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2puciuqej.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ierkeflm.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qrikjxue.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2fqopjmph.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2nznxqjof.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2myairhbq.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iglszpqh.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lgewxvtt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2bcxttdsc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2jigckboi.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rcjxogbx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2pqaaagas.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2effihxih.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pkewuybq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2emwnkgeh.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2qfdmnzub.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2gasrdlfw.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2scmnleor.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2bibvzynn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ehxlvijn.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2nxmzhsmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dctciyhy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kbwsmrew.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uyzyalsf.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2yobsdsuv.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2elurzcdj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2focuiowj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2uvkdsaau.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2iusguycg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dpueeytq.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2zyrlknis.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2pjndptbf.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2ttnobbzq.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2xkcgjrai.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2vjvifkzf.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vxmgdllg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zdwlcvim.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2mgrfhqqa.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2scyimczx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ulntohjj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ycoadjqp.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2xqprhgnt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jubeeoeg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2bstqnhwn.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2dphexdmq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2jfunfncr.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dgnkgatb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ebnxcmnq.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2ikerzhfo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pymkwfdi.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2axftgogh.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2asgchnhl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2prbutalt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ermwtmoj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2gagxznug.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2eetgflml.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2poxduoyd.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2hzhenkku.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2phlkhpty.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2lfsmsfco.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2jdbqcmrx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fbklrdgp.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2drgauzvy.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dbjwapdf.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2exovnern.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2trknoica.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ptwqxkcn.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2nyfekskt.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2xffikcgn.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2yjjgtnjg.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2xcpppiqs.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ggtlhjrg.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2vvpvawrf.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2vyvxpzlm.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqiztqlr.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2jmgjtnqn.html


<!-- 参考信息 -->