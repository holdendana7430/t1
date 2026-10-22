代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ukxguenn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2avbpgesy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2igvsaxba.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2obgfmbxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vxbfbyhf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ewgtproq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2sjcquqja.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wpmzllgo.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2thgfmggl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2eesyvuds.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hqquvqyj.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2vsvlekrh.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2cjrtnrrd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wftbxznx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2nkfvkjdn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aciqkdnq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pyekmvjp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2drtweenc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ksvbabmq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dwwjdnhx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xvufqfvg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2acfkuopy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2grcokvkz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2jllpsiql.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2flrtlyjj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tzszpzai.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ehempken.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yxpfxpii.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zmhnbicu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2cgxgpmgg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2ssnvfocj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xxdlsbbe.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2nydjsjht.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2askuqghr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2eeuoskqf.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rpzvwqlu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hfgmwaro.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ljifobof.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2iucvqnqq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2xxlnnvlg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2uusyjgzt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qcxmexvy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zohfsjup.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2gzjwfmwy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2spxvedbf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zpotimze.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ythlmlrc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vtgulqll.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dyqpdbns.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2telsdegf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2neygxmio.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aafwtukm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2epjutowu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rgroousu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cypvfnxm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2nljrnobg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bkqpznik.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2sonbabti.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mxfdfiob.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2uwcwmvah.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2stuukebm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nwkptkmt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hhxkyiam.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2objmhllt.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qagmrxxv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2dixlyjaf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jtffuagj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dqhlnkvy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2jdocdjos.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rrpxsxrn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ckmcnsjz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2awtquqnz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zacpcxyk.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2enbayawz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2bahenlty.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ncbziwyl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2sejakrli.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kexuhuvx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gnivhdjf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kdkondfv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2odiaured.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2refpsras.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cjjumtah.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sytrrgwo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2alccsylx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2meqmvejr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cwxltuyi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2tsnyfnay.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oiydhbyd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jurxibrb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ubhtscim.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2uxrghoph.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2eggbwnxd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2qmzycrce.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kmslynva.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jmlvzjfq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2qzwzvtvx.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zcqiauex.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2olexsbkp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xbkvjzvm.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vbiesryc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rypjbhaf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vdrgmcpb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2lhvrinaq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nsscctsv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lygkiidj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ggpqlidw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ojzdyyya.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ifdbzbyv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nndcxjaw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gdcqchxo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lymqglap.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ljvimjyb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2nxwpkoxm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fruqkrpj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vajaukas.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zvobojjz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tweatwfz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoignskw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2zkalszje.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikoifnie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2seqexemy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jjoiaaos.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vibsvriw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vnfkdong.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2epxexoud.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2oayburqo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2maeonxrb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yidisqpf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2msemdazn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ybdztbws.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2vcgmdhsn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2imqewrkr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mjancdiz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dmtsxukp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2obmhwyuz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2chyacoht.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2rwugkhhk.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2qapsuxwv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2vepqokcb.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hefbqpkz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ccpyahnu.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2rcknkexx.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2uvqhjbdw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ziduzmaa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kgvaejmg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2sjkhhvpn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rnykvjtk.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jxycolyq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sigtxhji.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2zulosyso.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gmbeyflh.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2roftzjzm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2jnddgqua.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vcshhdkt.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2todgmtsb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sjbffgld.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jbxcnlvv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2cxbnzydf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cdjjvojn.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2laxvomct.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2mjrqpliy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2napdtgcr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbvkadfg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2rvfxeiez.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bziwvdzg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2onvpfkwf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ylfiidow.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2nnlhjljn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hfnyqrgu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xjgyofbg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2sayhxdag.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2roajiknh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uffqkkqs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2sufcgepn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kjsossue.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tjzfnysz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ukoidvbf.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2korhqzof.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2fgadxjvq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nqhvefku.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mjahloig.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2fbqpnrme.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vbxzezdw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2cvdligwt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ycmprkcn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ovhurhew.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ljrskmqf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrsxlrxj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2osuitzqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfmrbuby.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nwkyxtgf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nzwzieqt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbajdwrf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jycbhxww.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rtsgyybn.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2urmzrbgz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2hdvzqqhk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2yydlygtl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2cllzmvfc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xjdusyad.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bnnwvrjq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2eqhkocsn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yfssdqka.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tdgblpmv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ltgmjniu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2bevyirvh.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2rrfdndeg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2qkcuynxy.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2xnckomsj.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2opcuasvt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2foyvnddr.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2pzuzwqcn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2kmzfwwyu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bswfrslp.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2qhwhomro.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2zyaoufwl.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ondudbqh.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2qugytjaw.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2bzcddqgm.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2iqoazfuz.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2eteuzmje.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2dehktwsz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2phuxfotm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zgnbcysq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2glshteoi.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2rthcgkzc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2hnypqaom.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qwejmjgq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2zkbnduxj.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2bnqsdpky.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2jiivlava.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2byxmgcag.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2stxrhmmp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2kihlfppm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2dmzwkxrh.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ycagfkqh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2qaosrwzm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2engvbsbj.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jmhiqrlx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2vnstayai.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2avweptzf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2kxunpfvm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2tyclrvpc.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2fctmxvmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ozzsmmzy.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2yqjscyit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lihxzzsl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2vuwdfghg.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2tpglsayo.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ydrjgvay.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2uipancng.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2akihrbjc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2iqnjxdcx.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rdegwqfx.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2capykzgl.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2avpzdyjo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2ptbbglnt.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2lsjwbvye.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vgifeulh.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2khpwpdsz.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2ujwjdblp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpvdrzf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2sfecczmh.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzgivckv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qzhuemqx.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2opbvornj.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2mkklqtvj.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2eiawomql.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2yxqrailq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zyqrfqgg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sjbnuepi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2yepvfhkh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2klexrxts.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2aicjckgr.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2fcfrbhno.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2njgjwayh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qmtauwkz.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2nnbsyiqj.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2goqrblzk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ykjkkcis.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2ajhwsqgx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2plrwoqii.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2okbbcrgm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2tfntphub.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2nwgbmecr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2qrcwkrpl.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2qmetbhmu.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2gwmrajya.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2ydppaebd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2lonwuazu.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2eoggsoas.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt2lfxnnxpz.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2pjryqbij.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt2tyknehnm.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt2ncacltud.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2zyfvyjju.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kkcanyqr.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mzwdukbw.html

Go:   if x == nil {}
来源：http://www.52xcode.cn/Article/details/gt2pwomglyr.html


<!-- 参考信息 -->