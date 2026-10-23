代发 wailian999

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3hranqprp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uaqxaczz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvnundzx.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3dlodphkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gsijbtmb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iigirepq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3yajhkjqr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3wysyxnmk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wamyrxfy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrluqqf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3emhjzvio.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3ersblhxq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3fymzepeu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3zzzlxdkz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3avmcotjl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ypebzqds.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3mvdxotly.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wjqrzehd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nfdymjub.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zikqtqzq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pbopzavs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3pxjknxpj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bchflofk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3sjlxfwwj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nljlhplj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tgeopcwk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ragsaaec.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3udpisraz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3bxfexjfn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3zkaigxtq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rfoasywu.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3cmjmrpef.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3amojkfrk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mvnlewkg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3xlvutwjs.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tudgmpkj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3propxnef.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3wxfaluks.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vgvsrprq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3kibrhwrx.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ssqqioob.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3vvvqhfyn.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bqvrmyem.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3eopwxcqq.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkkctqmb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzodydnp.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eabdupsp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sytpbbtb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3zfzcladp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3vglecbur.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3byxnglep.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3avduvsgg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3uqajxnfu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ktlxjcdq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3knbvquzi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3lwxfsjqi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xlqrnryc.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3oiwnoqel.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rbolrykq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3ohwymjra.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3aitlgvlo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bfrwautk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xexrjwbz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3lswbwscz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xltleeww.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3lnfrcaok.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3opgzseot.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qguekscg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wuiyluot.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3aqevexrf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dhfxchlu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3dxifluqm.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zsdipxqj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3notrdyrp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vcvkebyw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3eeqoryvv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fetfzljc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgqiyzxd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3dgrsfdff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3otwlkfte.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qstubkwv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tastmqid.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dyeemwrm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dlymsidg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3eiojfnru.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ckfsrfdc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rlrwthso.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3xgmijppg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ngzqxhkk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3zcdvdmbp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rjwzhcmb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xtifoztk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3igdsnrmd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oienktqj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qezpzrmv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hibhkhhe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bfmgxelh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3vpzahtsg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3zzrgahnj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3rejhidkk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3rarxppze.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hotdyptf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lihmkmgc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ymixstdo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3shorcnst.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nyejoqci.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3jpbtfurz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3cwdyiiet.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pkkqxifq.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bsqetwid.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mlbofuez.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yvhrfftl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3nbzblnhd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3vsritpja.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3mycsdxsu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qjpcvysf.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rgpbjuem.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ajbkbeob.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3xyraahab.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pthhwdok.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rxcczewv.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3uiycnlcc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvqkckc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gqfrjruk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3kjsrwovj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gromxrjr.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3aprzvkzl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3otwexctk.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nvtchlxy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lrdftdqn.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ogzxspeg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mzxygwzb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hvfqogtm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xpnvyjni.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3holjyzaw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3umeepfta.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3roprxjvh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mdpnyhjl.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3auxwjhda.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mwsylpww.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3wzgkqrca.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3yhgllauz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ccgwcrlb.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vtasczib.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qxyzunqp.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3lvsypiox.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kkxwlvhg.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kyxmxoos.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cywexyxg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvdqkbpo.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3mislznhz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lkvuigke.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aqydrgyx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3kgxejqwq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3gevprkwz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3waiyjxck.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3nrowaumb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tcblzdoy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xalsivwo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lspjriwi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3aunbfkud.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3etjkiwkd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nyrgkdsv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hdrrfcpw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3iiyhdhjo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ctabqaev.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3krokvcrk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wmajbmau.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nbgnxicl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3gknteohl.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mtfirbsw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3eqsnhuyy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3oyoydkqq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kjsphuzr.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mjkvtnhh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cwamybyo.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ciorwjdk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dzlztdah.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yuuhqqgn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3unnjwkyr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3ajjsiwkg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3fxjvsnhh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3fjlhednk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3oslraktz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mugevdqu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3lpeyozrt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3vqyfzcxj.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3njovadfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsjkmxuv.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3tqeqskow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fqujlqur.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xjtlxqkf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3yzlqrojl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3nhkujjog.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hmytakdh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3xycsgouq.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nfrodtcj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3oncdhekx.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3okxgxbbx.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3llagkxvt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3pmnwzuhd.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3molspnlw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ushmzowd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qnyossgj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3olyfbied.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3mbsyynil.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3dtvgnckn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3lciwgzer.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3zhnwwsmo.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3heojsxaq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3ioalsfaf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3borttzoq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3rupdeqet.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qmzanato.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3oigrnguq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3veyfjazq.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3htpetqyq.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3kjkjgutk.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jtxmcrit.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3gwhboaen.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3cxonwpwn.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdlafcza.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3eeywlerg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3maldyahx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3pdpzwvgg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3euqkzafx.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3kdiaslra.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3sxuvzjlo.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3tmhhxvdh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3cbwqmipv.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jderkblg.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3mwaeenkx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bubyvsgu.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3lvmzlkkb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3wvtotice.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3mzlnbrin.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3oagerhxw.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3jqhbzyjt.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3hptvmxmr.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dygaerov.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kzfubztx.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mannvtqu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3ornefflw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qfjxfzlv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ouolagay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttzpxwug.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3puksluey.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pzkywvtg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3uysnzjmy.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3kxfrhvzp.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3qfynoyip.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3zciabgek.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3unsdljor.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3pumyswvu.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yozttkbn.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qprnfftk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3yjossoqh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3adgxcbzg.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3zqzxaucq.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3fipshxhk.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3afmffknr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3tbedrjpk.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3juwewcpo.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3nwvvqqbg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3impxnohu.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3ozkxfuck.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zrbpmqyk.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3swgilyqg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3ajaesfbu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ovqgylne.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jcgyppyl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3wzmyaarb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3ljwuffpv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qqrbtofd.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3burjbesy.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3uixjbceh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tcowydni.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bvfyoztn.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ndylrsyh.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3wtxkeyha.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ioxuxncp.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3ymeaorim.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3sifpwqql.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qjrivfao.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3hqolnywa.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3yvgoqssr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3etdrptct.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3ujsunkhi.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3sjuesrag.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3wzwrtxnw.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3onlaoxzb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3siuflzag.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.52xcode.cn/Article/details/gt3jeugbggt.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.ydjk.org.cn/Article/details/gt3jzvmhqeb.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.ydjk.org.cn/Article/details/gt3bijaynlu.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3ctbbvpum.html

JS:   if (x == null) {}    // 同时覆盖 null 与 undefined
来源：http://www.52xcode.cn/Article/details/gt3ucvgayno.html

TS:   if (x == null) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xniocshn.html

Java: if (x == null || x.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxszqrdl.html

Go:   if x == nil {}
来源：http://www.ydjk.org.cn/Article/details/gt3rcgmfwdk.html


<!-- 参考信息 -->