代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qddeshva.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2xausjakh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2uufppwhr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qfqjhfas.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2emptnira.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kuruxzcf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ujbooepy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2thythetm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2yowqyrfe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2snltzhzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fqiyrxwd.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2lvqqpzpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yihhqdkc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nqyjfhov.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2nxnnolax.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2tnpvhjkk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2lviocixc.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xschnqvq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fqzqhktt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pnxdyvln.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ybachkhc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2kakxyaxw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qzxruvjx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2myfblsxo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xwvtmesc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jqowidbt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rvhldyjs.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2edyqwxsm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nbvokwcs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2axpmqsue.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lwfinsnw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2kfiyoasx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2knuujxlf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2exethxmm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jkktghwd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iieyguzf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qgzcupcd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uamojlea.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2adoumwfr.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ljgjcjiz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2njmlsxtq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2flgkedpv.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xoltorru.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qbsruyxx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cinmvkwg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2emqtlhvf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yshehrkx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wnkguulm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2iwrkbigv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lgohffxf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cjgiyuhg.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ptalxljy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hxaimxoa.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ikypttjw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2onjirray.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2miciqzoe.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2byzyucte.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2tdpouweh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2lgeujmak.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rcxtydzn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2zcecrksg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pnehtcll.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2crbpqlvj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pgbdkpxy.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2igkmkkqz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qpykhwgo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qtxdblrf.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2jtqeaivt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2wnedwpnx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hfpsrtjr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dtywuzxc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2okubruhz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2zjxtgskv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pljmjbgw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ucizkrit.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jbinfcon.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sikhovky.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ecbkmojb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2hdngvymn.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2myllrvdb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2nhbewfpu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2foiaelra.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2urlpeqyp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2jastezud.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dnjuczhm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ryjiuzrr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cwjlxyqr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldnjgbnx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ljkppjqs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bvmfohln.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aitkjttb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ttwxhkhx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uibficpz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dzsskfzo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sieqlium.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2huslviex.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mmqclmnr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2fmcglzvy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kvprffhk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xjkmcjdd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pzqdnqpo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kdlmvouc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gtvnmcvt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hxpazklx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2igpemqvg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dskonrps.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mupswjfd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ztaaptdl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2edrqkelq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ifgvjebn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qyzpvcwc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2nalzzhvl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lypqspcy.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2owjjlidg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zqhsmwzc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2qnmuhimb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2foxcltps.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vfxckneg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ntvahgxq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bgsdlgfk.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2cwxakusy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pybxfien.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mqmadwkq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bkviyanr.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2idcpfrdb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2pqjxfotk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2nwoctevc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2umoygfhu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nvrenwil.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2qktcmlzs.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fphvdecn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ezzstzvm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dqqsmcnt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jyehgpcg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2glvepued.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2votyanye.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ujtajkxi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qmccvpsq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2gpfvtheb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2qjznewtv.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uvulwvvn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ifkmrhiy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2plxhzegs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ovuuxxoi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2awnhcbxi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gosoeddn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ppbxtmyh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2uvsxbwgw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2cvswmdax.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2plekhnpk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2nlwujtsn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2rjxwspep.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lpndzbmy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qozmgfgz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lawnyxqr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2gvwyuare.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2txepniam.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eyhfbxij.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2oonalldu.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2twicigkf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2slmkhead.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2rmvvtifq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hkvkuzff.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2woznevdy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pbtwxcxc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ewitohvt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zicgyzkl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sxsvmcun.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2siuvqzmu.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2opnmdwlh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2yekyhzoc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ozbftryc.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jgfgznck.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2auprggtg.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2wzoiyokh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pkxxinnh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ggfgeuah.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hnxonjco.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fnaqypct.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qifjxjkm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yzrozmzz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2duxxduik.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wzeenafa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tqvpzkdw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2cfwdjptq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vhzgeiuh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qnhetttv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2njuchaft.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ukwhrvpy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2iuulfani.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wnwktgag.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mfyjeymr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nlvnwqkd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2fgxumlda.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2suvuanjd.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hnfotyor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fylfseds.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2clfcevds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hozfulvs.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2gpmbqssr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uxzzfhjj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zkpxznly.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2wqwnzqpy.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2zyzbmuuu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2nlhpfjpj.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2yphmislb.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2letagltl.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2mpqrgbmu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2hrfspvft.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2flifmacg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2xkdtrlra.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2zoyfhday.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gyqpnzwv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2mentizjy.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qbrjmiob.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lxuthpdw.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2eiwsndpv.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2xjokvkja.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2nyjgdaqq.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2gaetibsj.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2qdbftiee.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ncsosgqh.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2byfnjcbb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2fysnyhao.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2opzgkenh.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2vflwpesj.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2utukzvre.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2rlzbrpsv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2afjstzmd.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2yzszguas.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jjtfdbue.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2rwlfalky.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2slooxglw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hsusocaf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2nqsfoidm.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2igclmqbq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2izcajkyq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ighqqqhf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ldplqdvn.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2wfjonghu.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2dvryscbs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2lgcjxfgp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2axywaiwz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2hmpdotil.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2rwasdwpv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2tpvzevdv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2kntyqagy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ujhcovrm.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2zvhjlcrm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ndeupkru.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2gacxaume.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2ygkjxpob.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2ruswyxmw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yexjbjtq.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2yvtvvfbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ebrkldhx.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2cynwtgac.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2snrmztbl.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2lcyfzyzn.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2zzsmlcjb.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zavfrinc.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hhtfxwvv.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mpjkmmta.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2wuprzuzk.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2gugragro.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2didusobm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2vtebvblg.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2arbinfby.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2oirrgemk.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2mpfulxeh.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2otlwumzz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2pqjvykqg.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oaxzxoze.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qyzljioe.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2zolgauxn.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2rbtqszst.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2fxotoaak.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vlhktnwq.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ostrrvgl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2rjliqhzb.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2qtgkxqbv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2pzrcvriq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2rarsxhkg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2yzuhjmoh.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2ehssntjt.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gpyhbjdx.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2oonkimbd.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2yocjolsa.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2vzoravtp.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrhnzzx.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2wkwnivie.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hjqbxkar.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2lixryptm.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2wowtzlmk.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2axtwtgmk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2dnkjjdfk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt2qmexospr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2scvroujh.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt2emjxttmk.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2vmoeyscb.html


<!-- 参考信息 -->