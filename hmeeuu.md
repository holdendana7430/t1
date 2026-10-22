代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2txlkdbwq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2muydqoos.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2mzdosfjx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zjmqotjb.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2spbtwpcc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jcihngxn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vgeqwukh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2wrzpgrrd.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mjuldnfs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2poqbamjp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2taoszkvw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2mukotqzz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bwxtokfz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2afvqkfkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nigxxpqf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xsnyflhp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xpmeamga.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cpzsyexm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2pwhvclsn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2liasksvj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbcopag.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2csprexka.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xofdzuxq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2foohkica.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2mjflmkdm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hyiwgwuk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gxtriybe.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rqoukguv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xlfwrxbw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jmbqbjbz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2uuzdlrdk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ccsjdubu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eikvdids.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2luwzfpqb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2eaelekca.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zcasgbln.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2kudbcajy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gpskljnd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2efubrzjx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qcsrgqjc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mnoyqdhv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fzsjqyyk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zlfyrplx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uaedizjg.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2nukwzkee.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uenfgsuv.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2evluzzhg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2jxfwcicb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2obpsyzho.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2haxpnpbh.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ifephalu.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lbpubxnv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2neubmhie.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ntlwzixs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ysofvrkx.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ovsoadck.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jettgzzm.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pfiicxos.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bjwzvhyk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mxfugtad.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2hgsuplbv.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xsstmqna.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lutneddi.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2aweyuplj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2qfiegufv.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ylrkowvr.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2sfuhynwe.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2uxznzrgr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2boyfysiq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qjylnvrv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yfvswtqw.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2sdtuocuw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ubtbldlm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2atcunrzj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ddrohsnk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aermuphc.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qgujoozg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mupnndpj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gvqyxery.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2yrmzwmhg.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tgztapri.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2puzkcdfv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mgjbbsfa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qkloxrgb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rtfcounl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rtgpzsnu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qtjffrci.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2krqvopuw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2rlpjjlcu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zcfqhxrl.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2xgrhthwt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lsariszr.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2gzqndlnm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vlqngtps.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mavontiv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ouylzzom.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2xqqekzod.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2errsasny.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2frslbcyu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2xiiemsbm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2whxvfqpr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jrjgyxis.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2jafwzfwq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mmtsswxe.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fmwklxzj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2eiwqpsuo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2zfggiwne.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ycvjarwl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gdawjvfb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wbxxqpyx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2avcfdfdv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sqepasls.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2lsiufnry.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2zculrwoc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2lhpphhcb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fxqzzwmm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2bzojqobm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ayjwwqdx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2zvogxija.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2pitgxtml.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ipkhgqxb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2awfdwzxb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mwvkcsnu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lmamrrjx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2urmnhtmu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mmprjgrc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pfqbukmp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uijqivth.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2wisfvdlr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2udemovds.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rotwcsli.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nftjhzke.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqieabwl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2apedzqbm.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2hdvlvnow.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2clnmarin.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2apziqvmf.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2cozsztma.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wjkuewci.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2arosfblb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eppuwmsi.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lcfvveiz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2uwcvvafu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2kjgcbhqv.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ejngzgzn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2utrdwsph.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2prplhioo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2kgrlsyhe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2yzvgzgrh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xodlctcj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2iubojsyy.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2rrgdbzih.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2zkmvziwm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2lgmbeiic.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2sqaqykhc.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fiomdaof.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzoxbzac.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2qtmdqglt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zylevzis.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zweichra.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2docktzrb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xwcggsyf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2efgqrcrb.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vsqnllgx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2knfirwzn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2whwhnnva.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xtjknvdf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2idrecnid.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pqlqyqfw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2vmryvnqw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2sjvctnxn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qltuummt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2srswteum.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xfhokjyr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2qqbctned.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2grcvorah.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2lygkcagi.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2dgxvfpte.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpbyfseh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2comzyany.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2yphlgrzk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2eewtlsds.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2thuwbgmp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2vtjzggyh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2fwfisqhr.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fasnkxss.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jnjhactj.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dsygpimf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2gyvonjpj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2rttdgscv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bmfqzlwf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pxfwtkak.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2sjpzkrvy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2oyjzpzkv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2apecntmi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yjmubbuz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2smcfuyxi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mamflktm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2yburdjad.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ykdxbdjo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xhwztnps.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2ddwjuzxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrqrrdnd.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ikvmdtau.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vqijbxin.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2apxwijtj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ysrcrptj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kwhqqtjo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ykauwqpb.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2blqstdfz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hlqxqnpu.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2hdofyope.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gtuzjkyn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2oiwzipsi.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gjsjedul.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dbzxwtyj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dczqispn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dhkeoyot.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mevxkgtl.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2lhynswyq.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bghwbdhl.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2ukvbpkwl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2llsouxnk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2ouhmkpku.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2texfgmzl.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2ybkdhezs.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zlrtqror.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2hhieuasi.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2fbxmyaxe.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2anaumyhv.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pbauaevt.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2ujtoffxt.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2hlngeaiq.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2enilkaqf.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2irgwypfz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2fpymgnnj.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2swjvmglw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2urgfimcv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2hugmgung.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2gctndwqx.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2shhgyzex.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2qkmtxdru.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2hqdkibnw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2qnsyibyv.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2ratwbjri.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2mnvsexqo.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dfdbylzl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2saoeaexx.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2mbueijwv.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2trwshfqd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2urympwes.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gyxhuebj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2mrxsyfcb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2hwpevmzl.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2aqiyudcd.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2mxkhblkp.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2hbbutfai.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zfpafscw.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2ubgobxvi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2glgzbtxu.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt2bdjiqzwg.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2bphuzicf.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2jqvubkhd.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2maidznxk.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2zcemvtij.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2tvejgbjf.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2yfzgyanm.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xrsaqdwe.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2cjgmjjhh.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2drodlzrf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2wxoxhdzd.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eteeptnn.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hzgdflxo.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt2imfswnko.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2eanjagbf.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2ccxnxksn.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2zoglvocr.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2ysanoper.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2nvbkvjtg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2brlsfrya.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2kzcfggdn.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2obxvbbsg.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gsdsrrwo.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2frcdyyit.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt2lvnaxkpd.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2trhpucwh.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2pcbjxuci.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2ilgpdrqd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt2srrjzvmb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2evjfvyej.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2bmaqzijr.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2gzjgpwyk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ginlwxqg.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2hhdixwbq.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2gzizwzxh.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2hmsskwbh.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt2iqpqqcuh.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt2fsukunye.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt2ssfwbeyf.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt2yulfnccs.html


<!-- 参考信息 -->