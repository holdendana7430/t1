代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ynduwifs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lnpfkzoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwkkvsso.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xjnznivk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kfjhzvxt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2anghuihi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lhtodcxz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ocuqhavw.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ewkfeblq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2srrlxrnx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2mcgsrrqx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zcmujfmi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gpbkkfda.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2viiprjdy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2tlawqtpl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bdmdxjke.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tzbnjjwu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2euhoixfy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2swfwrpdc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vpfjpppg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2msnchhkq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2kesyhuxp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qpvuijhj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ggvozjje.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2pqoosvtm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2udmlsocp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ypwscxqx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2whucayed.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ijlkcxvx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2rvrlikqn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2dnxrztid.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zequjbpv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wqaftdsy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2htjindda.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xxdebdwc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mghfokhw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qfkbgodi.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2aizjfaao.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uhszjcnf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ikhmasmy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xsoftrka.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ffjgxprx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rkjgdvwm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2swszshcf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2snqxuphx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zudofezw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tdtigoby.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbangzg.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kpgqjegc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jvqqypqb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2sqlhxgsz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mhrbbtyw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2adkozveh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kwugptoe.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2eutbkijd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2abyeiksk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sjyxfniy.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pbjfsnew.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xmhhhaxp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fxvnrlhh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2myjwbbjh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2eqizgieh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mcmekyfo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rhaueivi.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iydybkrz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gyqqlslp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bhxhqffp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ekusltnf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wxplbhpr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ssdvweku.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ozfbrwvx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ekvsdaag.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2gqnlrcmq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2hivurgnd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tbxbhrps.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2bmxrgluw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2irtfazqg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qaudttbx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2gucvszig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oskcedbt.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2tmzeceyr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gpqfkyiv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2szicoqir.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2cxxhylnc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zbhhixxt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kdcsdxte.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tmsobqeg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2rervpaal.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rxqybtgx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2abtucxgu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2sykuycve.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2woqodkrt.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vdirmyov.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2secelpnc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ovbkvvbh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zjcycszu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fpugikug.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2fekqpppd.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vpvndqge.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bhcbsgmz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hhjleopl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bujveovy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2oivdrcff.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2idkvdlhs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2hdjdwlsh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tzayyfuv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2prvcqbmv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2axfmvltp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wzuzwxme.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2pctuqusy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qoeoclom.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wwzkuhhy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rhcgkwro.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2evyebtiz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kvtvjrze.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2azhizfie.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2aqkrzgrh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xmrrpszu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ogkplwxp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fyfioacs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2eimaxega.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bpuocmjr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2djouozdg.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fjrnzepy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hdjnmkyc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zdbdgflv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vsjxhxpo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ixdiuzrl.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xhndmbqs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2spwjdphh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jtinhbpr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2imdkccxz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xkidbelk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2douzpqju.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ftkfwhnl.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2icmyrfnj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2ugmktexr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xknhuhiq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2gyarnmex.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2zjmnruem.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wwuspbbh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2hyzxrooo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2yxqcpkyv.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kdbldmue.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rblrjlij.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2kfbirpqr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2awcoyhlr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2awmxgpdq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2glngzjyb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ghedvmfs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2kbbdcysq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gcmgeygg.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cragjjtv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cnnyghhu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mxutfsvx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wqybtwud.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pdoeandy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2glvzhywt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2upcdhwbv.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wizvgfjw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2okcoxkkj.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2fxwkogqb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lriusejk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2jmitqerv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mzltblko.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ndqlbnuc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rnmiiabg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2vdufwtsy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2eltqbwjw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2cmcfszzg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eurbarpg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2navkorwo.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rgapxtvx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gnvwiact.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ahdvlpuy.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zmhbucce.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2kdquyroe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vlxvyrcv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bzaonarv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2bxflfnua.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2dqtcuxar.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dxmqapan.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vohdhnul.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iyicqjak.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yqodbqww.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cnoqjmqo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2qlbizyju.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mjydcpcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xgeosvao.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ydmkckin.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnccuzxb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dawkejnp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2jsgkthsg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mgxvlqor.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2hipjjzhb.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gqafxjyv.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tdllgdrr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2pfphucmg.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gpcwzrne.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2krotsybo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yyweeiat.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2qmsssuyf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2kogynzhn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2uhhbfual.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2kbuumzfv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2igzzrtgd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2dvfaesuz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xwlfqtvh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2kkwhcloi.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2kzakguwv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2tifwsdnu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2vdebzkli.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2pndaobgo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zfgdgwrb.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kprsydli.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2dedyvjos.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2xoakuofb.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xjlnttgn.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zsotphlc.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2nwfzuzqt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2peckigti.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ngenuqex.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fmfxwpey.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ttrjowks.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2cqbvgrim.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qnvtuzzp.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vafvnvhm.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ixnksjgf.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2plfpapdu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2yrfezbqo.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2wncvjvqe.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rqhnwheo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2zbszufhb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2imtiduif.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2mazuggon.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2auqlzibs.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2krtkftml.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2pumktbdf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2pdovglyy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gfdphxik.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2dcrlbzcf.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2svtugcgc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2vefijzse.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2lfofiaku.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yxjuoefv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lrwgzsfd.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2isuwenuq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dnwnjnfw.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2thgxbbli.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2afquilwx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2laminvtj.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2nrokbqvv.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2jfeikztb.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2fmxjuapo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2qsomojvm.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2qobrilue.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zgfxdroy.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gpcliror.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2bhektnex.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2camezwac.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rhuysrop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2rrrcrcej.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2hovoqhrp.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2esflhtvu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2wrpqqkus.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2irhkfgti.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2pbqewcbn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2cffxiuby.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2cocifyon.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uzbmgegn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2lvyxysdp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pojxqqmm.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2pqfkyizo.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pfppliuv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2browjrzm.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2vyvzplnn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2anzdchik.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kcebuiqu.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bfomtwfg.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2frasrejy.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2jvswgemg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2poaesdaw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2vtgmrgjm.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2mdhvhluz.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2rexdekox.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2upzasgos.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2hqyknffr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2lhbehhtn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yatfdpsp.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2lejydzdj.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2kdijkixh.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2cqjktwtf.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2gbaotajh.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2qkgxotxx.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2dtcrktya.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jvgmfpcj.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2toidcepp.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2sbqbvxpi.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqnuxitt.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2qfbdconb.html


<!-- 参考信息 -->