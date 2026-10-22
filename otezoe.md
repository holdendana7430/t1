代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2ynpzupyk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jwgrnkdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkqwjvmv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2fzfhzsrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hspmhxkm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zfgtysla.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qkjvcmrd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gteqomcb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jpbrhdbx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ubbqxmwb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fxgmdery.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hcjkdyne.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zrrctfxh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bvhxzlyx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jemgaegk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bwhwqasq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sjhaptbz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2attgxmzg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dwoxtznd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fbblxpyl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2odvufvdn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2bagngwjj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xnrrjpso.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2yeaanuiv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mmosoqnv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2erzywknx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kupzeojl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2akqthuly.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2issxjdvl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2sqdicwyx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2pzbtvbmf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bqzudgby.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2tlxpekle.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2icgmkyct.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2kevbilyx.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xdyeebut.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2utkuhuig.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qxlusfci.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lcconzze.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xodvrvcl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2smjxnlor.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ecanpfqi.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yzcmgshq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nzkszxmj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2brrfpfve.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mwcjooen.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ewdnukum.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tlxtrbup.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2gssgkygf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2aisznjlp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ttlvvxwb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ebjgorsi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zswhcyor.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2msnbfxhf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2olxxizek.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nqscbvbm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jwxasyan.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bceaxxdm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qpvqkbmo.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ytegahdo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xisusopm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zgkwhzpz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yerfxmny.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nktulaxl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dpcrlfkw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ffirjkvb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ziqgakdj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2wgpqdscq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2hnvnjcqc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2nuvvelkz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2juornodq.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kehbooay.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2eabfcjpl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zvhmbiau.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2cwjwfszy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jjqfqfha.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2avyokmub.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nbpddqwb.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rmzgkjlk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzdcpwcz.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2xfkusgtw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lptkoswf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wjeeqloe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2sesywhui.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vytqdirw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lhilucft.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2npemrfsk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dwnhdbol.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uyuyaeby.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2uzbdrwvb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ivqjimgm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mahosryg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rkitupbm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kwjjoprj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mfatbmve.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jeydjzjs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2ljszlhim.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2nwqmdqef.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2idmozhso.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2tjxfjhzl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ulzoigfh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zgetmmep.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2dphlrhdt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2pzjbpwwm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hpwvihkx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ooagjmkw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jvddyhjd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mhecxtsa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xqtlotqk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ridogmck.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2imxzaqlc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hcxkvwph.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lwugovuf.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2augbbnzc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ovdxysae.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2sbzudqfe.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gqwrvmiw.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qskeriml.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2hulicgqo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uieyrfli.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xslmpwvn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lbtproff.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2axcjeiys.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qalxnres.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2hyqwxduo.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kpoynewo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2tthrptlf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2utksxhfo.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2isqlkgxf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fodtwnsg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lhqvizoj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kutvdwwx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2abilkbbq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qzigkabx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2acwwpwjm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2gkkgmblx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2iezfkbhs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rcjkelfu.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2bpxuvrgt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2qlehqfvh.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2uokcieup.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ntzitmmi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rfnoiqeq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pxkhghqz.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2vdfbyrtu.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2vqmycyow.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qaqxejng.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fumgmnau.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vhjnftbo.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2iwoyenry.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ahckplmt.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2riqghevp.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2rfoaaydk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fcsncqun.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cdnaxdqy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2twygupyq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ykphuada.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fkbmufpa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xwejfswf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xarveryl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rgzztnxm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2eismnfwp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2zibnmmfi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2wzxrqspr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2cpjaygua.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2rdempzvl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipwesqon.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2nbvqbzxx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2medwuxzy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2brhxkqeo.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2baerybgx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2zruopkvc.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ecnoatvb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gvwmrefv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iymfyvlm.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zknngahi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2octyajag.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2cknzafsi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cnlivesg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ujxadfcf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2mihccfod.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2unmzkimo.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xzsjapjt.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2aemnctpa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aljbujrs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2sqoendeh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2glytrpcw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2iiqjtxks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fiufigyx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gzzlcvkh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mssnovgm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2vmqmfdjf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2dfuonlja.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2rqbqvmxf.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tfxrjjex.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2qieislkg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kdtcowpb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2eslthixp.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2vbcbewcu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2blmlnray.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2cjwkfvgg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gqjegllx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2esuataop.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yhgikxjw.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wjtggewy.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mepzgvnb.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2rllrfgri.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xbtjkryu.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qnueomdm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2pnocznyv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2cqvxhzdu.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2acezpgtx.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2jlmcbauk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dsuhmrbg.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2liiralfa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tztydxsr.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2bukgnhae.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hiukjxab.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2nyktzdbg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2siqiimxy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2gonjizqh.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2cytsxcug.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2klzuxdlt.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2qrltfhjc.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2psxlbmlq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uhsygvne.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ywtzzjae.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2uwthzpjx.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2pxpinthx.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2fjrqrmjj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rfeoskpg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2avlsslje.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2tdfryipz.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2royeauaz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2clqctpyo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2tihnnzjt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2tvqwhevm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2gvntvwod.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2tofovhgf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jcutggrt.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2bjfkpcmh.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2jpzdvwap.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2mashznpc.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2babobsrj.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kyenunvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxytnucx.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vsdayebk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zicwagmy.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2oqldpqgm.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2tplnpdbk.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ixmqjeix.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2oapcpvnz.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bvetnczb.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fmpjrcfl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2nsjihexy.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2rynxzngd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2oybtgqqk.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2tjbrjngj.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2uwtvjmrb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aitzfaau.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yngptcna.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2yothrwcp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2pqyiqlzj.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2xpvtyvai.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2snvdopcd.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2mtbbjmyt.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2cpkevzrh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2pnicbgop.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2mtmbxbrk.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2hphfmcmt.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qtbqqbke.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2uhakpgqc.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2vzwdwkqs.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt2diqakuxj.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ojqukcnj.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2jmhgdoos.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2moajnakl.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mdnuzfwj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2bxxwyofo.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gewbwzav.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2codtpmgr.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2yhvdtyok.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2hnwghmyj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iaqcathe.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2vnbtnsmr.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2mkhgappj.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2vnfkhuwj.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2tosomnfn.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ldjlueml.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2fxquushu.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tvwwmajz.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt2zxciwbzv.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt2eqanidyg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt2rtwenyjv.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt2jkjkhruq.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilhoivxp.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.ydjk.org.cn/Article/details/gt2mmdzbldg.html

TS:   if (x == null) {}
来源：http://www.52xcode.cn/Article/details/gt2ticytkog.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ysztinio.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt2pnqagddr.html


<!-- 参考信息 -->