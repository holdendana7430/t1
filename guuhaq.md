代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kdgorxqm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iyzfzgvb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2efwnxrdz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2wshidaby.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pcxxgebb.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mgyoryut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kzxytuia.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2tbaiitki.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkvmkyrk.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2mzzyatop.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ssyudilr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qfdrgmig.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2demjxwcq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hamodcml.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2baujeiep.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2qagvajcg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tcejlhrm.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nagbqnsj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2wuydlxiu.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yiwyutev.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2zvtuaisf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uwpjbeew.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2yflhxgas.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hdemjxwu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2muqmodmi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2mgasizvp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wnxsdtgx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2pnmzdjzl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rwtzukze.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2wtcxqloh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ptvmazxe.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nzqinnsc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2praekuft.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vcrulkqv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qetkhkkf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kakmyzmu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ysvjwesy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dckjqcku.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xufkbpsc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iajfcjod.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uodtawui.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2kcbpfvln.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2goaqbhrg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2krxphwuu.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2yigsiyrc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2xusppvvb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2duuejdps.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rkperltq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhteetq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ahzypxac.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qzirxmoq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jbigvpio.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2nebrabfd.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ohqmxguu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2duryiuwe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kdckoglo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zbmlzjlm.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ljwoxodz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xquyxent.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wkedaorx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2tircrapv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ccnwiodu.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2opjmijua.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jhbvuiuk.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bwkrcjbg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2tbgxhxck.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vzyablke.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2sqeyxfnj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zfgmtyti.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2dwdqrnra.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2chmbnkca.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2uvqkokfa.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2fpxanzrt.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ombkqaji.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2xqictynh.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2adnoiyik.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2yljymfke.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2sttceyfd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ajknfnyb.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kvuosclo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2dfaiyvba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jhmsvugm.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2rwzyxbxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nntkimfb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mphzmlgp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mjpomamw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2edhalamz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2evnpkuwh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hcjygsbt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2flvypbjl.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tsertqjf.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mxfxyvqw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bjcajkmn.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2neflsgou.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dttfzylh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cyzxlchk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2bdhwlbsj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2sntqkzbi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2asshctpo.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sewdcaqk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2wygarsfn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2olyxwifi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gpontyjq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ciyxcxch.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2iyibdbgv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2minvwygt.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hkhpetil.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2bduqsgui.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2jnqgewom.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hjspiqcl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2votkhdsa.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2gpepabtc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2gvauipqs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2udjtfhik.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ocdeawtb.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cnqmkwie.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jjnzblph.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2swvnpwua.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rfesjkxk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xqkmtsjc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2iytsimhf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2bfxtnpmf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2kmqkoxrb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ftecgvxh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uawuammu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2xxmwlrug.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zebjddoo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2occucjwb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2quazeauh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cuciwrmw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dqmtmjto.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ernzoqzm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2suaqbrmf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fklyiphn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vqhdytan.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2skdkohvj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2cabqjzyw.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2lcrobgta.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2twwcviho.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2scthqcon.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2hfpnewzb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2msgghwvj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2najtgvjx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2haowwyib.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2oniclybw.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gdybgowj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2besqxhct.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sahhqkan.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2trqvesmi.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2lcjrbapm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pjhlaajt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzvncnxl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uyrzzayy.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jirrumbh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ycmpjyfj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tbhsjfun.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2axmvgovi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2axlujgwr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bbpwfdsd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dyliyvqu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rjyiprra.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rwkzicnf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gvfzexyv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uepxprmv.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ewdmqazo.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2qajktpwe.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lidzvwuj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2bqwibxjo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2hsamiykf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bjlqtzoy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2mjfvsroi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2calgsyjw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2jgrhefvs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ypdakosq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sywtubbs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dexhxtxu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2qmnxunnt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2srahluia.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2cdksrqpn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xmdeyser.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2syipyhje.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2caabmpfg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ejhoxkqb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xrtjjgrc.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2zxkmradc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ukajjjjz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ajwgesme.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2qqptsmde.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2kiuqalpw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kpqauurv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ucxvdjpn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nfftgpoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kmzzfrvq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2lxnrbbuh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lhvmylpw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2limgdsav.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2isabjpgz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2shczsyhb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2yurzvwco.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2keyydsct.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wqoedhny.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2qevwegcz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2hnthwnuv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2guowckre.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zjrvnhdk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2uohhkwjn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2yjblhhrg.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2sxoktxwv.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2vrnzwbsh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2lazsxbne.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rggyfves.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zslzkswj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2ylbhfflw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2kuthpxjb.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2ndkwjtma.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ortufaqm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2xnbnoeja.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2udewsrpm.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sccyyrtx.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2camiixrc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2ydhgleyg.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdzaktbe.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dqhlmyqp.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2saejurid.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2zobkcsjd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uiaxowfc.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qnwxugbe.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2hxgemhjf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rvggntxm.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2bnhbabrw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2jqmbvlhc.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2rclsitqh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zppgrjmp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2budszdac.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2sidajboj.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lhisqqrr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ltrdogro.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2gsezqzhx.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fhnmmrac.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2panvpudu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jyptywkh.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2zzwtqnmg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2watdjqpd.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zhovyncw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2yikhvssd.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2nsronwtq.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2litsyfhj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2qvyzrnbt.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2maehjxzo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oayfdqdc.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2qvdnprux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iuulfryq.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2dxyhyqim.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2xxkzdynp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2uvdcytid.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2wdxkxsnl.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2xsdopjtp.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2txsldrdk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2csksienz.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2larqescz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tfhtqopt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2zcovxtyb.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2ldnwgqux.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kiwkuhhi.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2kslznhft.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2bksjrxlw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gmpexaoh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2wydqdwrf.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2awczejxv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2juokxkoh.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2yubassjs.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2uxlfagso.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2rknlbnvv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2uzzoddku.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uzqjeoqb.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2umihzbbr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2jsnmljvm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hyduixmz.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2mpgxmjen.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2iysvcmuw.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2zfetoxeo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2durtbuvn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2vlnfkeaw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tkahqeeq.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xtfeadow.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2vtubvtaq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2eoneerfj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jfdvuusm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2uxfiunfv.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2xpoergsg.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2qwtnlebh.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2znwildov.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2aoeuarkr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2wqewdfva.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kxbzhvya.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2tbcnhfku.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2okzslhgv.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2slcoftym.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2gjrclkff.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uxncijzf.html


<!-- 参考信息 -->