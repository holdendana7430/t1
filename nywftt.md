代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ellhbroc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3noazprem.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3fwpdquyp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3zxojxykw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ubsenlmb.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nshtjxza.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qhohfuvv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3strkhsuj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kmccsaep.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3trsuutrq.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ijnpwkqc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3spykwheq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3rixdzpqr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3syfnwvfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqshogxh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3kikooanw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3drbkgfto.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zyxaceyn.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wrksgzeb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ymyrnahg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nntrqfvz.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qsusivgr.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3mrmjrpzr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3efobntgd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3eizmgxfh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vmfxiudy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qdsreehm.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ehhmzyjk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3rpjzzxkz.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hdhndreo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ovwrnmzr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pjazulju.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3helnzynb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3qyyjwhnu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3eiqdxcid.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rvbnwtdo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vllugddj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xtrzmjvx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dkjtrwir.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3evtkcgve.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hvkqdvmm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cerqacem.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3ttkesgha.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ugxctfuo.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fnvwsdem.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xuasqwih.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3bldjumnk.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xsombcrs.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wodtyldv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3rxcgyhps.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3vcwyzkqj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3pozhwgvh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ezzhzfsk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3lwcjkxwo.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3eqqyhgla.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3mgntbvub.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3odnshiig.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rydzgazk.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ocutdyfk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zzcrmefw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vpujpbvi.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3cwvrxnwq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ieticxsl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3rcwhodsq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tjwbkjax.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3vmuvfdax.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3vappwcvr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ameeoncd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3lpjgzroa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mtoxsvnj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fblkielq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fyxpvowu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ezgrwlmt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3rwazbsgm.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dkrgchmq.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3flageocl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fugvvyyx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3bdkjzimp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3vlbvfzxg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jahsqeve.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3qrynveak.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3efjtuhkq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3uohdxdsq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3abntqmmt.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yxyrcvqs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3bzcpeike.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3stxfoziw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3icjaoboe.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3vrkckuaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxmeyfhy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tcnywsjq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hbkveilq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3zzgwcfms.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbegyqok.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3qdmggmyc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yeidekvw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3astvsfdn.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iefweuik.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kxtfilgr.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ihqobewp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nmbxewil.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3izsgjgra.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3qffwpeif.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vlpabxln.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lnddplkd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wktyehbo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmjkdmv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3atxbdzxg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3jputpgxp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fcijqxrz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3pwivegeo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3txeovnfe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3hjvfmcqj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fbbjbayf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3lycmxbjq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3nclhgdip.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3uiuxtxlu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3sxckibyu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3glmbxhsc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3hixlieyq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3upvkgtwt.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jsojtfww.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3exjariao.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mnqgcdup.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ogvyroxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3jnecrcql.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3imgjgdey.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ijmaqsyt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ziojcpuo.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3icvnbgjo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3goplamvm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tnbxvdzn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yaspfznt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3otnxhejd.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3dsmluxii.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3dbrgktcg.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fwqueyqq.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mcryiizj.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3xslosiph.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3tzcidksy.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bfkcigaz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qdfsvfhs.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3tdubkotr.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3rlxhuioo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3klyhxrxv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fyetatpd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gcwryirp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3bvmtowox.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ixzejris.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3xqwoicza.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3avgbdsoe.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3anevdnys.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3mjtbjehu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3hycqzram.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bqitmghp.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3dxqlbkar.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xwcnffzn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3bxnpthip.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nhvwtvgk.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rnjlyrxb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xxjbfhpl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3patgnleu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3rtoglims.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3cwscdwyn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3nuctrglc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ysqekkvw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nefdapcd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zdywvqno.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3tqfywhan.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3yvsldvbf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gkiozdkb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vwqsncqi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fnphpcso.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3cfdxrykz.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3whbzdmfd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrioqlib.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mqehuhhn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kafzbuaz.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3mynqjnje.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3eznqycxw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3okagxzri.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3sphfjjnz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xcvusbdx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3rtyteskg.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ucraexca.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3dloivkpi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zqigoaji.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3urxxkhpm.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3xvrfaflt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3mgpzqozk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tyjamvlu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mbgkzbsa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xeaqxpvm.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pmuuctkf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3midqktnu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3irzxznoz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tejhpryw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3cecjgstn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3wyslffjp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yobfqldk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aciqirgs.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3hxdcqeso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ndyfaito.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3euoixnek.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3mpxgagaa.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3mqosuqky.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bkfnsluk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3fanmyeah.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3fivypqhp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ealtdfue.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3jmdivvbt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3akejrvfl.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3vgozjyzc.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3jatoxmmi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ipdyfzkt.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3heitaris.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3fpwpbbev.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nzmeyxik.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3gpibokyo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3nqfnbycd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3skmfhwtr.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3eqbsnhfj.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3fmqtoogy.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3ueybegru.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3janxprag.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3gjbmxabj.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3hvzsxagq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3hvhhjbpy.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3rivjpnnd.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jybrezcb.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3lxewiaeb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3rykwarqe.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3vlsieval.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hedeybok.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gjpyvyxo.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3rdjqkqzz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3tnboccdy.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3yfhekdup.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3scgeuspj.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3hotwnmjc.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lwoiqdup.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3ozjxowhn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3stgvdenc.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3vrhjstsk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3hthyapri.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3tdbvrtoj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3awpebvwx.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3wffwbdlj.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3vtkwyzaz.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3djtnjnkf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3kpipmykl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wlgvapzx.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3xkuoxjmk.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3dleofbwy.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt3weoxvncv.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3vmrwdezb.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3igrvbijd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sjcylibs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt3fwoxtlio.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dverspum.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3iqvntwzk.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3rcmgglvr.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3inogyhev.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fnapweog.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3jnkljhgz.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3qwizqmbh.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3okpjyrvv.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3idzhheta.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3gupscngd.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3eyaxfzxf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3mojtmaer.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3trsiksrb.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3vikkgjdl.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3qvajblck.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3doklawvh.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3xojlaimn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3wbykmcim.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3wmpkoaxt.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cfaupizd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3immajomt.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3msuinttu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hofapxda.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wsdjcmgc.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3iiuqwwgs.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3lxcwbrkm.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3uctocehn.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3kcwwxgcx.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3xwoaozgu.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3xkboeadz.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uaklbfck.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3pxojlyay.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3lpalohna.html

Java: list.size();  map.size();  s.length()
来源：http://www.52xcode.cn/Article/details/gt3bgmmedik.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3fsqkurkp.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ffbrvdqj.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bcdtqzbm.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3hyigaisd.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3cxdixnuc.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hvjkapyk.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3blmqlktq.html


<!-- 参考信息 -->