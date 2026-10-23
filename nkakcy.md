代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3nldsddna.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3riwrtwqr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3pmjslvrh.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3deunbikv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ppqidxlj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3upnjqkwi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gkozshkc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3ukujxodr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdkuemnq.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dxkapoyk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gcvmbhwa.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3mgvdbeau.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3cqimnmpw.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nnmetqdb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dqzoymqx.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3alwozbpw.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ebspkiww.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3spfprhob.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3hnopspba.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3titardtb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3diumyotu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lkewzuem.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mbjsokbj.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ucrfinap.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zmqixoaa.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hrsfuwqn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rfuwudkg.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3gclytuej.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cbmbfddy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3jkqycsma.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3dmgmugpk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bqcyjiml.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3smlhqvor.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tjtqyneq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qjocxbfq.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3bvegjebg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3aubxxyej.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3caganrki.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3zntobatw.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3eohflxtc.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vprmpdml.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hqasllrn.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3wmlimqhi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kmsemihn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3dviptakj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3kqnbxbep.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kidszygg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3jpaxtguv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lwaxrrhi.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ldhbwaic.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vuaeiuox.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mfndamzq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xfxrlkbw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3irspdbdb.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3gdmhixsp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3jcnguusu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3epzlbpyk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fithjrzp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lygtornf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3rqkcfwhw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3arrungyo.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3hqvmbecm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hnuwdygv.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lewasimh.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3baprzevu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vuhtedfp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nnilujbu.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3glpxxsna.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3cgbqvtlp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lbjjgjmd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ihcunmqe.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3gvugrcma.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3hyduhoot.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3fegoerwm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3atuuqvwk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3oontfioc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wcbobnus.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zzlpbcyn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3ppwuxtxg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3ruppipyp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3eehzcnfy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hqpjlqjf.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xykohith.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ydqauenh.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3daddauyv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hscuranh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3asigftnf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xkjttvrx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3agaceupg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qhpuzovq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xsypjbfj.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3eopvxpic.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ecslhkyf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zupjzucl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yiakzcea.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ptduddqr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3maqsfkmi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3vnwluoei.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zfpegwlo.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hepjnocj.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3ihacydrz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dbmhsqes.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3ogavgwxp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3aoyejwso.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3yteaojzd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wgemhban.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qppgpary.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3bblttqvn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3rjnecvkg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3gacefpgh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ypsoqxwl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xqxkelkf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3utvjgffs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jeivqnhe.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eegwvzqd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3pkbeelqj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zakppuve.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jjipdcxb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3clsiuzhb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qbzouyju.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fzsoudms.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3flqebkbj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3eegufmkt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdwbidgg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ocpjfgns.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3vtverqzx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3opatgdie.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3njnkbbyu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3vbubnuaq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gnrvtvny.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hynokmpt.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vbdesywj.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ffedioel.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gnusigon.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3hjxfqzyo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3vmjspzpr.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vtpejvmy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mxklqzfy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3zabvlymx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3nhfvomid.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dyuhrnhw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wplyvhwd.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3isaiipgi.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3hhwwuotl.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ddrgzwdz.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ajoarlnj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xvvzhlxy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3zfqcmmtj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3mjvqbnpx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3kjunoykh.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xmkxiidi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jgahfzqf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qoszooxx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zztbprej.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3urtywwaf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mqlxvcjl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rocbfqhu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rugfhtvk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hljhkuxh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3uwpkkwja.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jztnqwbd.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ttqzlybx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3vbdnjdgp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jjycnffm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3gjgomfto.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3zqlxkuaj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jtwzukuu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yaohbxbc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3knbxjinw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ppgxdlrr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbjkjcno.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jtbbmcio.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zksobgqq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vojlaoqs.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bhflbwyb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3cigzuspm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3htbgaijj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tyxvzwax.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zovyvyoq.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kmswqawa.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tpvjsihg.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3aplnkpaa.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aetyctpy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ngctrhuj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3juhzvgcb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jynpzonn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3crcodmsl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cjyqsdxz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3uidjuefs.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3moxfvleh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3fgxqqlos.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nuvqzrpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rhgeckqj.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3exakoxjh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpecbgjp.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3sdfuzbyn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qnpoyvrw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3cnoeqvny.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3crpkthft.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xkrhpgdj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3gjbbdcfx.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nbbpkhlu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3osipmkig.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3fkbhjsrf.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3ivczqcov.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3ovhequke.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3xwnilvif.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3pczxdpjh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3giksktbh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3wqvoaivg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3nvhdzrga.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rtpqterz.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3qbacdcpj.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3eeijxydx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3wdcadpeb.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3iritmgqd.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3mnhuvbox.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3nbmnrgfq.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffxohbgc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kowfhowk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3trmtrumh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kgkwkevy.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3nyaofjwu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jezrosci.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3fycyyjkl.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbytygeo.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xfazelgs.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3qbaukfot.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3fizumamd.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3rjmmyloq.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3jqrdkjkh.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3gibbyald.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ttjbbabu.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3xecsozgq.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ygwajpzz.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lkxorqwr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jhbcmmfw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3xtzqeiey.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3pfdktred.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3oivqfddl.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jkriktjn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3kxkjwsop.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3syuoihzj.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3qnizkfpf.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3ccdhwfto.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3govcwzkp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3blyuesib.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3ixrhfeoc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3rqlmpwiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcfdfgka.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rjivgyqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3igajkdvc.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3lynmesyy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3swshvewp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3nkkfzlfb.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3wsoqztbo.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3bjynfaea.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3gsvrhbwo.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3iayykvpp.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3uwewxbgd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3gsjodsbj.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3exrqffga.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3rnrcnkfg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3csczqpwg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3pikeuvsj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3ctxhroxz.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mbdncfyn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3yuyoasxb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3plcotenk.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3cgogpwuu.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zxrjpabt.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3jtrwrsor.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3liluwfhu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3kxtmtrlx.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3trkspkjp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dffvoxov.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3audxwgrc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3rulfokor.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3fricvqmt.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3orxucdif.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xzcuungc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qiarjwbd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3zdgebdqs.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3licmrpbn.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3leusmars.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3xjnruccx.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3zxtziaxz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3uwkfuswa.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3tiorgjff.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cibomeef.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3zvmqkhyr.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3gwfzxbax.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dkapmhaa.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lesegsqq.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3jutihigr.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3yrihlgxu.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3czrzytrq.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3flupweon.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3wqqrsaht.html

PHP:  if (empty($x)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lplhfpqf.html


<!-- 参考信息 -->