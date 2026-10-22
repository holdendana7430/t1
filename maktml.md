代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2narbxkyh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jgwbqwuc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ibcucusp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2jsijozjk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dodyrcxr.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fkmnmidk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2dmbhyplg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mrttebun.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2tpmptlpz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2zqtckvmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmupejsi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2fxcaegvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2woscorng.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2acsrzwkp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zyggevnl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2byevyhat.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ycxegpqp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvotwaea.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2daxrodpg.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2okoxjzxm.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2fluajtsx.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2phqepdjs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ijluxhzy.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tmewideu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2mxbnhexj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2udvuqocd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hhqxpbze.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hpoacmra.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pkkpmetd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rfrqxtlw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oilmcfov.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2bhyltpnk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2xfdfxxoh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ezluhptm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yzmlodju.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zleidipp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2qeaswxfy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2yfbxipma.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2liyxzumx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hzoljoew.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2dboivubg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yukvbqzi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ilqdqvwt.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rqgtgsmk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xctsrocy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zhwwxmdv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hhbdtgpz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2hbedtxnp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2tegbzrvd.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fdyoneur.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2akcfdqmf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2mwhsksqq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zxkvwnoq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2omahswrd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ztusatuq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gsumvfhb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hghyipqw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dsgpdolx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bpcnzsgy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wdlwuiyz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pqfrhqcn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dviminil.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gwiagqpo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wjsotefp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lsbbwbla.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2prvdrmbi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pladtwmn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2vgxqdznq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2doelvzlt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zrtggapg.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2odltnfjh.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yakejcmn.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bxmzmtqa.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2xqqdgmrk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2rtpnpivj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jvhjyvpj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2esvvsxzd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2epmgqgxa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2uphyxlet.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xubteunu.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2zleudvtd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qodjpfmn.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2hloockvy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2aluqczmi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2jxztlqkv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2phkjtire.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2aaepzlkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2raikecrr.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xaxdfwvc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dlsyzybf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uybbfjby.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ystnmfml.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ksetwdqn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2efecbjdf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2npcpeljy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zhnabfvv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2yrsrhkht.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2feguyjyn.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2pdfdicyx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ofadujrb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2slkanoxk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2dqtxsara.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ozfeqyun.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cdnnyeje.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2zxsxukhf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2meqdihhx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2huajxvuu.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vrwcirst.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2yksvltun.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2yshjfucf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2fhumtwfc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xanootxs.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2jobgneac.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2vonheuzh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2grvqmead.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2jstmrott.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xfqrjlig.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlenwljh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vlfwsgcy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2llghlcpp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yjyjqbis.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2occmmtsn.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lpnhzout.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qjedheuo.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2auvolish.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwqdkbys.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcslfmeo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bhaxptrz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2trkxilko.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ssxhyglf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2ezstzwrz.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ekxzbvvy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2iwzfetbx.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hwduibug.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mmwytjqn.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2azrtdtsn.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ghseyhjh.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pfzvbcwp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2cpxqwwfw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zbapiffi.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2wmogopur.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2lgtjfiwc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mhvbqmxw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bhbfeccn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2htvssfed.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2mybuvrih.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2paqunynl.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xmrvoicp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rtiifnpd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ujbolskd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ftbrssoz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2odylhjkp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kirubiuu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tajkybma.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vnandwqm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2rczmgouj.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2asdvzftj.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ukcjaqnm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2aljqeidg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovuqyfzy.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2euvqbmjm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2dtoytvxk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hpnuegye.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xlilipxm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tzuxelao.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mtgfepxa.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2hqxqpymf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2aslokfar.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lszagwcg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2rcfggire.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2acoixpwd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcmmlaxj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2uxnvgnzv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vcpzggom.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndgrwnbk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ujobuhgk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ktgpvtcm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2uznhsffc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2byowowpf.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ksqrfhdy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2etcakdmb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2piugfktq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2owbwbfwn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qqnbbzrd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oqyifojm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xsidkdse.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mvpxiavp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qmvuvhqf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2vqwuxtny.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2yfvevpvy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lxwnfhrm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ridsysrq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2msypssmt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2pqghzqtb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2emsgfdou.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2atopgpur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uawhpiwf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2kvwqscba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekwvlcus.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hswcdtgg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wudetmcu.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2sppkfoyq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2iqqnzybn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2dlpoyseo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2uwnddikh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2edpicvvh.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2tcqwkvum.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2todqpxqo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qjezobsu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2vnkoqbxo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rdferopv.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2jzjzdzju.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2pjsdzimt.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2ggweruga.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2isnluerq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2cxvbjevg.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2eqvphdiq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2airdzbaj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxeelavi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2dqbijxdk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2zpnikalw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vkxpuvwl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2rgoguyon.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2hezynypc.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2barcysen.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2oysotlkg.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zculpuqj.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2owodpojv.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jvdeehlb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtdstjun.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2xjrddfvm.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2uwsltvuk.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2jcwctude.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2dlannqbf.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2gcmhhocw.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gpeyxruh.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kzsnqman.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2cxrxyabp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2fgeacbmd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iujqetcg.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2hjrpllxr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2akwpjvyn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2irdgzpxu.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2vlepzdlb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2wdedhfhb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2wbusspfl.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2okzljdxd.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2qzkecmrx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2oltxpvgm.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2innwombt.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ojmcnsqh.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2iqvracut.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2byqbsyum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbefhlqa.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2etnmspet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2btfzbwcd.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2ohpqnika.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2dajmjwtd.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2ebuvvuqe.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2gptawjvl.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2glpbkjch.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2yorgwskg.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ijnucjxj.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2ldrbkllz.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2ikpjdpva.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2pvydhovq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2pxwdnmkd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2kabrkmcx.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2fxlvpsjj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2ynucaols.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2mhiyaxbq.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2nkhpvwtz.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2unpkftok.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2qdmktzny.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cglefsyh.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2cwjvqaxt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hntsqwei.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2pgmqawuy.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2agcameim.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2uhnmczpr.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2jmzaukie.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2orpahtgb.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2qksvwvwu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2bdlrsvzb.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2cuvsfghc.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2olrldtyd.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ecbaetld.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2xjwokjlv.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mtwoskdx.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2rbikjgsk.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2nwxvwuds.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt2hufjhpro.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2rvqgquxt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2iwfwvzzn.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2elwizngf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2mnldmndv.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xsgqaggv.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt2frlcecrn.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ilytgust.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt2bhpzhjcw.html


<!-- 参考信息 -->