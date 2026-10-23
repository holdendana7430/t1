代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ljmxkubv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3gbcvjftq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rqgvvrvh.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3trkepbir.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3gtwkkivq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3padopjsl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tlredljw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ccqwxbbq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3yxbtnrgj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3aebbxohn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fwjbxrcy.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3etgxpqaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3khyyqqmj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ejlvqpyv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3icdzptyq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3cbgskcwo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3eaxezqei.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3mnpvykqh.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3piktkxqd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3tuzikart.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3nptcozju.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pymrmoel.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3wwvpeemn.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hzczimaa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3clhleghp.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3tehbvbfg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3fpbcwkjf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3oprmueif.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kxvbbxki.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3zjasgjcp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pmfgfeeu.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3ioryopab.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fcjenikv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3tockfxbh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ynbxzizv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3crkuvepf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jxsetpfw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wnkqnjav.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3hvauzsow.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3fzqvpfar.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3tspbvncv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zmsnbwum.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3gdhonsaq.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qfcooind.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3subjjzfs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ugwpoxsr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3csuzcdmk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ydgmcink.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ndlugomv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ctillgmh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wcmxwbts.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3uwaqlvzj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xwrxdmdm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3jkezcurs.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mgcbmevb.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vckgvyuo.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qbvyfwqu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3obxckwxm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3lnywpjoe.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3nukfsfov.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vwiezdfe.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3kafjzqms.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vwckofoo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qgxempfk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zneqwmgp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3gwqkzilt.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3frkhpqax.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3uvndtkfy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zmvksvfr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3hdaowslf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3nnaofkoq.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aoyhxxvl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3sdfknwgf.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jtwvtefg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3oqmiylmy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3catddjbf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ijnmmntq.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3gsiggrhd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wyagtnjz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ocmjmbcu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mvqryaes.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3slkwoifr.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3invsqpct.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mglviiwr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tozvbudn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3quozvouo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xhcbxvlu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oiwuhfxw.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3hdunwnkc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yzbahzjg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cxhsesvl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3pihebnxj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ddblyaxi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3obomcjtw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wrzeshvu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3wtbcbxli.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zdfruymc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3gvfclobz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3rqqxypyl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bsnbeqyi.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kpurzgel.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3xtffrask.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3zrazhgwt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3mevmbldz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3nqgkgcie.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qilwfljg.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ikctylld.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xqzwfpyg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3fxhantrc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3omerjnmz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3sxriznkd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3lazrmwyw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3ufduxsrx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3nhzxynel.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3bcngxyxi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3kjasdtwx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3dmejewob.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aslajwzz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3axkghpxy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3hsovsbxs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fovwrjnp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3vyuanrmm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eteiqsdg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qvbrcfav.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3zalgirut.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3wxipqsgg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mgaounfk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pwxcquxi.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ygdbrwwy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3camvpmud.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ctpvszzl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3otrnzejq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jkuuqiph.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oybsrpdb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ocsckmak.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nnkojwex.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3brmbfzmq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mcpunltd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3yxbmccud.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3soirryhg.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3cnwvizgo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wxkpkpmc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ladzyrtc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3derpyvow.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3hsxscmws.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3tjgqhdnc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jgtfibln.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jzdxuluv.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3thxdbbqs.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bjtiwffm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3ngafjvol.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3loczxrmp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3iyyqylye.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ndlvqaot.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ifepqpcl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nrzynfjz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gzlnnlzw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bijltwma.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3aizkxfhx.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gbfcpunn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3amructgo.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3armokuev.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xxfohytj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qmicjead.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3epsirfpu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3lmipgdro.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3khzqjpfg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lktiyktp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oidfsxpx.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3bckyksmh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3zojqzjxi.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3onwybzvx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3npbupwic.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3quupeeun.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3hmiwzarv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pbsjhxlk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ihgddylo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3thqvyjsi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jckpkrem.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ziftkgsw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3mjqjeagi.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3emdnhzzh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3jmkprhpb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bsiiwahe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wpdvtvkn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3kknlqmhg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hrjxumdf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3kyttrwws.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3epjohumu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3uwxxfcfn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3repgyxnq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3uxbkvwpd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3bnocojiq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3vielnevu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ejhwtetz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mtesojbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sigxyokk.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tbyitvxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vnzbhbma.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3ejiwdwiv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mqjmdhsq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3bjergsxm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3aaudizoq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xygrcgms.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ciuyjcxr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ydkjfmbg.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pkndxmzf.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3rwkctacy.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3jvsnvcgg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3kbzcclrg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hcvurvhb.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jwdyzdis.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3hxsburdh.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3qkxpxbyz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ryxgzidu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3aqqrxvlm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3uvuitwpt.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qtxddeol.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3hlhkjidy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3wswaodez.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3deztfgkg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3ohbdvjqx.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rhysatti.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kosbdoyi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3azessput.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjkhghvi.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3awzqszfs.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3lamnlmss.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3ytuamwwq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ahgeqdbl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3rlvswuze.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3mkqrosvd.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3rbmlxyyo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3sgjfndxa.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3refoxlpg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3vrkhnshp.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kqggvedp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3wosavxsr.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3flwfinne.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yedpqglr.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3bzkwespk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3cungnand.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rkiqpdlc.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3hnmhmrac.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3kbtstsxa.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3ywqftgyn.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3zvxkgqbv.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3tnmvmdad.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xcffvmgu.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3cidfbybn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3iyzvieus.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3utphqxke.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3vyqpagwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgjcoymu.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3yxeaidpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3omnnogrp.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3ubembjmf.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3jnauxgcj.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3bdjlrleh.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jpgdvulm.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3yexgksdl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3mkyfpwmu.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3vixwwoab.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3ildyqvsd.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gqqwiyyv.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zfeankgf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3xdtgyhtn.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3iesrfyiz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3odecznic.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3dvoxyavl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xyuoczyi.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3pgbohudz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3oadunbys.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3gnayzzkz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3gegrcpsz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3jwppqlob.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3yujvyksw.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3rbcrhrsy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3qmkunrcd.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3oqxuicdi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3ywrtysgc.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3bsxhqarx.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3iscycoyv.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3sforvrwr.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3ondurmve.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3amgjspjg.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3sgjiqyqm.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3uyeflbus.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3pclnhusq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3usnuoyhl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3psflpkea.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3twergeto.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3ftboqgld.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3jlzrnbax.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3mmrtslnv.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3klbstzxm.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dgercdwn.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lcykhdvd.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zdppaorh.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3suhwgqif.html


<!-- 参考信息 -->