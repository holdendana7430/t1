代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tnlfxaah.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2laerttwe.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nayjqanl.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vnnxjqgw.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wbtbmdrf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2wmlozqww.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vbwdzhag.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qyduznev.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dzdkhimz.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2mqovccvd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2fvoxyfzx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2amljphfk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wytcyout.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iyhaxsbr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2upskneyz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ilznemku.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fwzfsxll.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dgovltgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mgyoqytu.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2gdcylvqu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2focnjmby.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vbguxwkl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2upsmyjmg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jlxcmdpe.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bogpubay.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2cikvzrps.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2nynmagqn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aipfwyet.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2jimjqtwj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2stgcdpjr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dfrzatnl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ltwhvvnf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2njyzbibu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jemwflab.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cjgfutpe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hvczyvzu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cbkeednk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2esheqesp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vhkyvrem.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2gpaixvub.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uzgaqksp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2rlqvnszj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nhtttctz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yogipqmp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zrebayot.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2vdezdaur.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cosuhpsq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kahkeojw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gzqgwjoc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2evyjhfzw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hlhdveon.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2kekhhodp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fbyqavkl.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zkyriwgu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wyclollj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2yuxeuiru.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ocnishjo.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2dcrgdgwv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qammbuxt.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wnuwqpdp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2quefephh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmfnvjom.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ckozqgyk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ixdffsvl.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jgdwpgdj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2niopzcsa.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2odfmmlgb.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bzzodehb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wvgxheev.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tvnczmpf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lcmlskzx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2rzarptyx.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2kqndrypy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2hndxnvsw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2orgozcxk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2fvgswnvg.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mjrzsvhw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2zqndhvni.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vqwpxxrz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2comiyqsg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eiakfuvd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2shjtizxd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ixuavosw.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2yxlaubep.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2xhkzvwmh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2wjsifmii.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2bjhxusoi.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nvcyzikd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2qbirjrtr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2safbwpia.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2cphaifdk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2anlthkcx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2xhlnobgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgffarff.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2auwnezan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yzgxnarq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ghgmqliv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oovpgyrk.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2asrwytyc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yjxnvkkx.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ifqbhqtx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2eewumali.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2etypnuav.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2cgzdthiu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hqofjurb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nhlhnmoz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2lpsddobc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xtczilrc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kxongkzw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2bgamqgxq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2amprualz.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2oymqsbvy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ldzwlyep.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ptorygun.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bzpndttg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pitxpsai.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bbxwryyp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zgchgsvw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2knzrbmzt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2cwtehzkn.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2uiacrbvc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2vbctjxgn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jgyinepv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lrgtzisj.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pteihzus.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hxnqjend.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2feudfsdi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kdpwnieq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2moufawoq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nhifaebk.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qkbrcnru.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2upgotmfy.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xwpnqhcz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2naixceag.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dgzpdcys.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2frpdwhnc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jcktynec.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2owtijznv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fvdbenbo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yjstylid.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2jagknktj.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2eaojzvkl.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qgjqcfal.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ndcjbvin.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xmtwitsz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2emxzfmea.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2zvicslnc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2sqnwjrhu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zlthtlgs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2exzlhscx.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2splyttvs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2wmqilpwm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rmrtrjzy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hkgacpal.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2wkmaoxhm.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rxrkfixr.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xhksusiu.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2auzvtcls.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xopurkuj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2kpwxgypf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kzxjfwpa.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qgsvezst.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lumnehck.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2eazbhzru.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ihdqnorg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iirtlqbx.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vnmjydeg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2infwmrnn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cylkqrke.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2tprzcqko.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2feqzfrrd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2unxqiiyz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2tvghbfmm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2khgvzccf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2pykbteco.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bsqbbzaf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2acymbqtn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2xeqsisil.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kisedssh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2puczkenk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2vqtotjie.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xhitxdub.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2hindfkuk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2odpqsxeq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2eqipxdgk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbyisekl.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2sfrqhlrm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2pphlgsgj.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cqipdjqt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iqoagvnx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gbbhwfzt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2sfunjbty.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lpgvdmfl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2iqwtmmpp.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2trmhwhsk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2bhafajlv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2rjqpzzha.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2mtmpidkg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wqrwefij.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mttoibfr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2whzkbjxz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2gcrwuyge.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2yklbqdqt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ipenkkkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tkmhjwdf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fkibbkiq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nwrcwnsy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2rsgdrhzr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2xrtcfayf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2akwsqqgj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2bvfcadpp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2wsrjdnjl.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fsiyhfot.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2blhoacbr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2gxcrjofr.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pdvayzma.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ujuhgfpv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2akgihygd.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qtckfqov.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2apoiqdpj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gewwvvex.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2gkbiunll.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2epcktqto.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2zbplpgig.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2qwruskcq.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2hwhycjsc.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2repgaigh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2vvlzjhrl.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2mvpgzkbk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2mrqicaan.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2nvgyjaju.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2iejnfyve.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2evjjpqhx.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2zecbahyt.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jxjgdxsy.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2ypqpbrrt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2vszfvdwb.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ytfzzakj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2acyhmamk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2grxefnvm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2ririywjz.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qcsojxhe.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqlewlvt.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2ognqpwka.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2afqwwcvq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2aracgnuo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2oilchzaa.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qpqepeml.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2fqysdtrg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2adylqsvd.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2pxyrrtej.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2odufthhy.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2arywxgpr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2xxsxklpk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2qyoagofs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2aedfjsbs.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2btkmkbej.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2sprugerx.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2ujlupjdm.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ztbrlxpc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2yxsdinkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewtohzod.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2payouvzi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pimcetmx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aoxukngx.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2cyfzqccb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2usiusamo.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2xfpmnvnn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2fxmrotaq.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2qnpijepl.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2rgivbvwo.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yfdfpssu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2jihrvaww.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2txtaretz.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2jmykwjlw.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrmziqxs.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2laivwxhr.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2xkbfwmtw.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2apnkltwn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2iqnkcqku.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ynrlpoai.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2edfbagim.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2byplkykq.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2jmzsxlev.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2hbqfpjqj.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2oibcqgpu.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2vfdeklnm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2sqztscdi.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2wvsfgcqq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2mgehxqgq.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2xwyzljnw.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2utjhnnkm.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2jvavtiby.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ybaeqqlb.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2wjnzhnza.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2nmakxakv.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2xndhlgvt.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2xdvznhhl.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ffylznaz.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2bvxjrhwa.html


<!-- 参考信息 -->