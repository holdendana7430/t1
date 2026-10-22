代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2beqojtjg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2vsiepeqq.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fyktaoao.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lwtrwfag.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nkocxvkq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vdhdmxos.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jsivnulp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2dwlyhqro.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2czswbtbo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2tcyhggco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yxinxerv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2etsgmqgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ubozgkyf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fzvzsucd.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bowactvg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2fdvwuiyt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jslfddzo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2crzzjyhz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2eiopbloq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zhezfaba.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ozobvqia.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yolysopg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jnihgucg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xilrhszq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pycboohg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kqkaqcmq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mzqsprzq.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pgkvasnp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lenesczq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2pflzspoc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pizooyzk.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vplumcau.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2psnczyvh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2keetrvps.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2myfficcu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2cxoliksa.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dtzpuhwg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2xwlnovdz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2juhxxeum.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2vvzsuwnd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2werjcxqa.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2crrapmrp.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2iwbxbhgd.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vdhwhymd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ibuiapwa.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2hbrsboue.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hhehnkpe.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2gsldxasc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gwpcbmmf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sjyqvszw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qvqxobwm.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ficivewk.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2trischxb.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sokodjii.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yhgsztri.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjdiorxh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2gbnizzut.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2lqznjdse.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ceerminz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ndsabcch.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2llubyovf.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cklgyyzq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zgympkqx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2syjeurda.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2desamjru.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2yyhhkqpy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qjgnjbbw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2wfdxxzzy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2kqejjpgo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2uqseypzt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uieezhxd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qaexvjqk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hphvtcot.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2diaafrka.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2xmnbovuo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bpzepqae.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ydljxjph.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2apukbibv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2tuucaiyx.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vmamwrxg.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2htvnodox.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2wntarnsu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2apoctjuw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mtsyanjr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uieoxkta.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zztsqziy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2xeiirvmg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvntkpkp.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2knuebgay.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zgmcbpcm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ugiqmdxe.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2tkqkfxyj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vzakmtwr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zoosfsna.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdyjeznz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qbimlpnq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bztdpbgz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2udnucovh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wehpvpvq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2irzrsdar.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jmptcmkt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2rctqcmum.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2fmmlsrzr.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tglqahxe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iadmjydw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lnsqzlyj.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wmrjvatg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2clfnackp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sznwynwn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2serfxlxi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wqggympa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2hhifqkqo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2lpbbrvmu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2hzvcfcgd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wnywhrrx.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2npdfbjvj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ycgedups.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cpftfdal.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mqumhlky.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2shxicmcn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mwpaxawg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2quuevpdu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ddonoiep.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2oxlxhfhu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2stkwdiig.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2owuqfjfl.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2fmjxmrxk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjeacqdq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2apxdcdwh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2uouvkwfu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dlrovpkd.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2oqkoknmc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2nfvktapb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2budxhlsf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2njzxkxxk.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2djjxmetb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pdjmqyss.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fbcziidy.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2nqrtvwpo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lxsqgtrh.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2trtjmyqd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jyttmxgm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2nozvnznr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dlvqnmsu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2cjsudvua.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gxhvrcwi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uxbcrztx.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hiblzhnc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rqsoakos.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tcqochgo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2toisfxot.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tkmaxvco.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hbnewzzo.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sknthjbu.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nkdtfief.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hjkbqryx.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2riykakpi.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xknkxqkf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2uidsjual.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rocildzn.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ijavovig.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qackecnu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hecwkxct.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ekywsnys.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dzugjqtl.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jyoguxsz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2etojfybc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xroouuwf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xodqtfwg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2walejylc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2utpnmcyn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2zraswcwe.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2jqeavdbn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hklnhfah.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2grfgtaqk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2gmviiury.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2knrbkowb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2frzgknjh.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hixoyrmy.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dyichcfe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yfliufjq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2luvxwgnk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fztrhukk.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ofjjjvyq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pfiafbbv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2utgbxept.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2cmzaovgk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iaunhyoe.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hlxccoys.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2beqcieny.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2psxckrit.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2zdbjkztf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dttunodi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2inmdituc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2xelkzlib.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2yfjdpqqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2boljteuw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bvaxvuev.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tivchptp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ijawjbes.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ewtikemu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ngfyqeoc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2tyoetyon.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ayimwurw.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2lawsuyiq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dxypgjlh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wtoxwgau.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2jpzcnfnj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2kvrigion.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2txpsbbah.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2ixsztvgv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2welckhyi.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dptwkdlb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2vhrrddqr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2qbaekndf.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2vvxhvdac.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fkfvfard.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2bxogrgik.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2whlcsydh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2etirskaq.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ooxpzqti.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tperzsep.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gkshkzps.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2iihupzpl.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2qdeizwzz.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwvgiosd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dgegcfmo.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2edltwajn.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vanuxrmq.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zhekdfqf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qmvwultj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2rqmmwabj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2rxogncqv.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2ugpnjifk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2yapofjnc.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2lnhkbfxq.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2atysuvzn.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2ynywacwi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oidcmhlp.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2idayvmir.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2fwimceuc.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2aetdsxhy.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ndnlfxwz.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2kbouivrp.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jlmvwgvc.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2zxtntjxa.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2hoqmsuej.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2rucjseob.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2okekfytl.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2tumzxcdw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2wjwvmwmq.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2jaxpdbah.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2kgrssehx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rhzblwdk.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2ffdnbadb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jynwrhyk.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2mvxovpmy.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2gvdlatbc.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2baucnsui.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2kfmvbdnl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2alksppsj.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2biqsqpss.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2btkvevxu.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2minwvxdy.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2tbcysvwt.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2flupvkny.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2mkckrrjl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2vdxxctwr.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2lzpjjkzl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nldzllco.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ubkfzwqq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2nwdzylyb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qwylvazc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2nlecnfvk.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vxxocdtz.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2jxxzdfqt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt2ztdkluas.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hjanrava.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2wfwzzbxg.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tokxsyfv.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2fcmwntgr.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2faigzvtw.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2koxnmzcf.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2zovtwxcz.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2cvfoinpy.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ivvcikrh.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2slqjgifw.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2jqsttxxy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2hcovmlpm.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2mhoferes.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2evnlckzp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jivtxoyg.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2chrgvlge.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2csrmauet.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2wfyqdzat.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2tdvwufsk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mytmsrrx.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.ydjk.org.cn/Article/details/gt2xrdttgax.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2tfdriwnb.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2kgnlgrdu.html


<!-- 参考信息 -->