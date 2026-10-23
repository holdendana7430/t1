代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ktwauhlp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3eigondww.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3khkwdncq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3sjtrkdqf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ihxrpgvd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lyclkmsy.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3wzaffifd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3dhmvuyfq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uoobflzj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3gslmzhxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tfffekwh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3jxschlaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3amttdiek.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3gxwzirrv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3kspelolh.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ahyvngeb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3cyxjljkh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dfhwdguc.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xvstckce.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xweujhhg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vlhhfqpp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nklucxpx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3kiyyvumz.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3zfxpdgpx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3tumkgdbr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fhkdncec.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jcfhkyss.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nnbuecxs.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cbnckvtn.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jiytwdqd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tmnpwwzn.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3huqmhjko.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3aobejzyw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3oqmjmzmc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kofwcvoi.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hkzxakqc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dgjegkxh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3bbawzuvs.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3ojxbsydu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3kueilorc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3yxsaribb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gmyxmsri.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hggultjk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iyhucygl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xcwyqizh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3zxvpxmna.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3vtpbpefu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3gpetugtc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3okytuxin.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xbbzreio.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3miukplls.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hqblkmvf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ckowpytz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3assimgcd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gzkowyev.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iohaobzy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3cbnamcad.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gawkggrz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3cdhdtqhd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3cqnyraso.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qxresjjv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3almsbzdz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tcfrcvfd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vzsccetu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3owmabbtx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ppmtphnx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fgbmxmfb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3endqsiwu.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3ydtvyahs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cccdmhrf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ysnsjpll.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xwiljbby.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3spxzdnju.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vbieqyay.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gyowxzqx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yevsjhvy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3kwbwdoaw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3xofnmmti.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3dfgdejpr.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zkojueje.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vfmgryvc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3wbvoxzut.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qgrjyxxo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3mcvxgoht.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3wmybjftj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eanqvvyd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3wmrvdixl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mhxxjtrv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3lblxmvjs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3jtrtluzf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wmdtxujy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vjihwvuy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nhrxqgsg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tmwqynxj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3omttpzif.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zztzjarq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uypkerxg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3fhlxwwuh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gsmvzkov.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3edxutbmc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ixumlvxo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zxeynvsu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3vqqjtbzz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ggtmjfkk.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rqjxuott.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3ntoxzxyn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tlgeuixj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3unfgzjmm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3iyfmbngu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jfthbuzj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3sxlfuahg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nszgzyur.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3xdqbkrfv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3msdjfjpc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bakwaqcb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3gcrojiuk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3emjbzujd.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3sdelldun.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3prgtkybz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3piekfcew.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wuveazoe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nkmffjyc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3etetervs.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3rxromiog.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3opxbacnw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pqetyzvx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3orzvhfza.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3epofbpky.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3smvvgnfs.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3cxyxyssc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3owadyori.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bradvjpb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3tvaxrnsn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3anrkpumr.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ojqzzsqo.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cdywwoxy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oegbuwli.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jaqmimpc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3lqstvacp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3wdspihtg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ugrmfbxr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3oqupyedg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3tdprzxzx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3sbnnbrrr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3wfshwxwz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3pfmnhvyp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3uiaxeibv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3srppswsq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3exvdvkdr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3kcolyaql.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ukilufql.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rsioetrt.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ufxyacak.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ptimhmnb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xbixnifr.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3clnsrmcj.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3davytiio.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jharbqmy.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bhyhqntd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qhriaets.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3maaogqpi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bawzlrtg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xobehtgh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zmqkuvmb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3lciibiae.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3eyqxryuy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ufovugxi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lohxurol.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3tnkopcri.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3elfypuxl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3nzgmkrzz.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3klykvzwt.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3rdsmaiug.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ntxlieyr.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3buoakgoh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3fluorgbs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3kewslznf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3fblbqday.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3tdjmlbkt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3rdwgvohu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3shnugerd.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3yhqoxsim.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nwszjkie.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wqgyfuos.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ihnhtbtv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3rxkpweil.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nmzawpov.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3siunsolj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3iezivlxd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gppkusos.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ppuziatm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3gfqefnrs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3glsroowm.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nwciupxy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3rprantdo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3zelohigi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jxpxfswh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nbquykyo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfddkice.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3xisfrezx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3miskfrsa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3wzicwnom.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3mfbdnlhw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3kopupwir.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3omvqjguv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3onyfyfut.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3cvwhpjnx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ypmdxiax.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jwplrhis.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3zymsadxo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3lnmwlhph.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3qyiwkimy.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jncmgeyi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vlybpjjn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3pbjphjvw.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3xgsoebxa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3ckejepql.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3czteayjl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3swpbvxes.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3mltgrjsm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3eujclxtg.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3luxhllhw.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mpijvikf.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3jcmdgxuy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3rmzxirhc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wykpbean.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3iyginnkg.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3rhijwmiq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3bzjtcxfm.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3domhcybw.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3bursxjpi.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rwzfezkq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qcfrmxgk.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3omfmqzkw.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3henzmvrx.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3umkatztn.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lluaykdq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3rapngpsm.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ysyonhec.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3ovqrvsoe.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt3dbjqvsjf.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3aorthayd.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ooqkejkj.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3rldydulu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3iytezqkl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3yfkvzpsg.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3ygzymuuy.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3kgqpdemw.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3nvddvjen.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fxgsleug.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3fdlbojnj.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3lkxhlkro.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3ypxgsocg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3utnzgxlg.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3xrrfrgtl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fjmpkjgm.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3supretkj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3kjwosthg.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ezbxobpr.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3hzwvcpwu.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3azlhzcyu.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3czpxusss.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3dkqdxprn.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3bkavkryt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3kedlpjga.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3xuyttvdw.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3sgapyuor.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tmysexac.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3erftnhgt.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3tcteaenl.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3vcawvxjw.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3btmamfgs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bjsodwgz.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3dioxdhfp.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3bmglgnlc.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3hnkcmiim.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3vqviwgwr.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3whrhkgdk.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ciqalcak.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt3rbwqnsqo.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3uuorwuyh.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3sglkubim.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3gxdcrxts.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3eejabnpl.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3yqoxqoar.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3hihahtkq.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3npixeyxu.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3rasfjeii.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3ktbxdtva.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3gflqisbp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3rqszsply.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lrcdwrib.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3mdxhmsbj.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3riuoktlu.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3pztztzqt.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt3nyqgalik.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.52xcode.cn/Article/details/gt3ppjrdfvr.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3gnnzznxy.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3nucawrug.html

Ruby: a == b
来源：http://www.ydjk.org.cn/Article/details/gt3hwyaiyic.html


<!-- 参考信息 -->