代发 wailian999

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3rtuajdzq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3euqkvrof.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ecmfmzut.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3lnvavcya.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ctadlggy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3lpcdmuzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yvuvmqaj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vrimoxqx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lqkjrqyg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hybdifad.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3lvbeojpi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3tilxttrv.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3ptmjwzkq.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qwbnjkdp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jxiicpjv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3lsgtakqt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3rknxragw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gjpqnvcy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rfizqkez.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lnpkdake.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3lsnkvygf.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3maniusnx.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ewvuspep.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3viirxrvo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3iwenlezj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3qaqeihuz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hifkgtsu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3alkcmmsj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3nxleygbk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3juzqswlh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ytftqfib.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3joeigscv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3tusdxkci.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3qcefapeg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uewyeshe.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3eenvugbd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ubnygwty.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3uaeeobfm.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3kvkljiya.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jtmdzvqk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3kdektdtg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3uwtoajad.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3pbcemelf.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3myrwupis.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3irzsxzhg.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ufnqxkld.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3suzoldku.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3rssxngym.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3skfnkufi.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvuqquyg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yhsvrbsz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3isesqynd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3uhqinopw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3vewddnya.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lgvrdfoh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ooiqgtwa.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3xtiqehvv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wbcypyen.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3dkexvgew.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3roejmasa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kyxbnsoq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3lqbmydiq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3aaucpltb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gcxchozz.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3edijhfdc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qsysouyx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rbgubvbu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3vmtvrqyr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3rpphlajk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3ihsyqdul.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nhslbkde.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xoijyxed.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3tmayfpui.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tgppudfn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tmvajjtl.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3noeeffsw.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yyrzaygg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3gcrysfzt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3obwxdpxg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3dxhlltgo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3gfkykijr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpuhgwgh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3addyeerz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nzyzqroj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hzsroljc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3vgeuffvh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yuikffww.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xzffbrua.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hxeoqdpp.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xlhcmeph.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lpiktwtl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tixlalny.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rmwwlmsr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3vcxvsyet.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ljmlsxau.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xkfjxqrq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dinondpr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ptkrzlzf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3viynvrlf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ehvyavgo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ioqogqds.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fbxiisjh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rnstxpun.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dtkpgebn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kqiigdnm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3voyiwbth.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ubmmeilm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3veanyrwz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3kemcfzxe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3uittretq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3stbmludu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nrbchwxb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dkvdjvgg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sofnexrn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3mziodfjt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aynpcjmy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3utxjyxgl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3weitujen.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3qdixvxkt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jdunnwpo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3rdxwrdmt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3amzdxali.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sqddfwsp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tcyibspv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ndhbijfm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3oiorkkli.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3hchaqfwl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3inaviozo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3dgfnruhq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fttadxat.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3egroahcg.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3syoknjcu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ahcirgvr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fqmljqoy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3onzyqphl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3ywthyhyw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3efogdtem.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3msumingh.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3xrxmhmuf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3gwoodqlj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3nbpklgiz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3trxxfmlw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3piymwzcf.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3buuhvucj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3obdzpyxr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kgoxhbwo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3liaqjfld.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3nyqcbnic.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3eghrwfwt.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3iregojup.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ehkspitm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3elyowsls.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uchrwokd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jtrtcbmq.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3gwysoaas.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xcxckrmn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3oumktvbf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qyjtgwue.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dlimfqwb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pqfibvee.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ktrfhieb.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zjzalytx.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3imscazkk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nltwszxx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3zrzmnaps.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3uuzykhtu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fngbnxwv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ounsmxhk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3jxqonzgg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bnnrndya.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wegctxsb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3odsczuxo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xseuwlnl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3vlclgeng.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3pepzzhpo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3zpwhagsm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3tilfkgtf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3etypundb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ologbkrl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wwrijloo.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3uycajytb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3hivtddvn.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zsqyfvuc.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fmrxatwk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3duuvjnzy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3xaganrbk.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gvzpdbgq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3schyklji.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tvipfbzl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3umurtbcl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3rqqatkao.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3umrrzjou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqwqjdup.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3sylhiejy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmzgxivs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vheskxus.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3myfhmoch.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3craoddek.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ggvtbsok.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ymrlynfj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ayfwgtwr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3vtlpgifw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3poqzkhfw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3ozetgmce.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jmthmkgb.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3yfyjwcoh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3npvdstua.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wvduqotq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bfnpjznv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3egjhmayd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yedvjsjg.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zfjvdhkr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3xipgfeyg.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3mxxdjqya.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3lipprgjd.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3sganiyoy.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3nwearbya.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3btgthwje.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3xiuyycmd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3kjlmzurk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qbmpfhbg.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3qbjakixc.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ruihmltu.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3fvagjrsy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3gjdgainf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3lyiupdex.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3grllscqq.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3dybkriew.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tgazrqje.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3mcawzciv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3smbdyirg.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3gydyiark.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3jnbkxwyb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jlwgvmtd.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3lthtjtup.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3jwiusjsc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3onkmpmbr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3fsjussdb.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mspjmwag.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3deaoefjt.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3qckpilts.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3zxovibec.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ubrmskbs.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3dxoudsfh.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3eqlchmws.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bhtcdmuh.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3vtoexejn.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3qmilllne.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3kfzgyatc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xlabtdpv.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3rsmvbgph.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfhqmtyx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3mbgtaecr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3yoozults.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3fjointfr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3didnmwtd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3irzqzpkg.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3htlwxdbz.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uvotqbsc.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3bdevpcut.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3vsifdyqx.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3xmsoauzx.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3efbipyxp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3seqoiqok.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3ymdlywxp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3vpycmuoi.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pnozhpro.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3uxfhafbp.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3auqcpczc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gvyvkdwe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3imxqscgh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3lugoervw.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3uyozmxru.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kqtqiocj.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3sjjknbfp.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3iziiiwwf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3rlliddzf.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3gkupphuq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3gebkhcxq.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3spfybbui.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3rtmembgc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3egjbfqft.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3nunycajm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gfiugqva.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wkzdoous.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3xpmilqzn.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3kosrahjq.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qtyugpym.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3uvwejfei.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3gdpsrrxr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3mplupjvw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3dvqhqhfa.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3mzmhzmzh.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3cojiefhi.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vtbgdwaw.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3gsiscrmb.html

C#:   Equals(a, b)  或 StructuralComparisons
来源：http://www.ydjk.org.cn/Article/details/gt3yulblwqg.html

[P06] 综合判空（null / 空串 / 空集合）
来源：http://www.52xcode.cn/Article/details/gt3ifxjobuo.html

Py:   if not x:           # None、""、[]、{}、0 均为假
来源：http://www.52xcode.cn/Article/details/gt3lwaufavd.html

PHP:  if (empty($x)) {}
来源：http://www.52xcode.cn/Article/details/gt3lczldnuv.html


<!-- 参考信息 -->