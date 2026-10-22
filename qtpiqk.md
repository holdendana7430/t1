代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ellsumbp.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hsybduqk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qxukadvy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ojhxvqqz.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vixtpouv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ahvlfmie.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2hbhdzson.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2uiigujah.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ofkvtxat.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hkbuovil.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tuutuvxz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zzdoifid.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2iznkyojp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2deoptpoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpshthzi.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qmhkqowa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2onjptlbc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2hfwbldlg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2sitoqpaw.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mrquajmx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zvegmezh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2czntsirs.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2xmupfoag.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xcwpqjqn.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2hksejfor.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bynexqrr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kpjmqqoj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sfzfverl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wpudisgd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2kbuzvsut.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lmqlikuy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qmacatak.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ltcflrcn.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2jmxrazqo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nstudzox.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2hkhsdrry.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2nlsytydy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2wndbcynp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2hqvveqhu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2dranumvs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mnbkbfmi.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2tsxdzitk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2skzgcfpy.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bwharuhk.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2eiofusrk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2kjxmdsbd.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2vhvukaop.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dffufmxr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pkjibrme.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ouaubktl.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ysqcwhua.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mqofnqhk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rnrpfqvt.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ybgwvlld.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqpisvzo.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2whruflki.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lxanehef.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dsbtppdo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xwaxbcmv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2izlspgng.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2qyzqelxm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2sptucywx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2eqhgcrej.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2vljhcpvz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2yvncgmsy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gsgmulse.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fulajpzp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2akjqtxmd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ixdktpko.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2dzawudqj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jfrwygbq.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2bpomjyxw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2sptgsrsf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jhdwldkl.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2cuhvzwlj.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lwjlczjg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hwninuos.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2moyeoceg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vdjsabbd.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2wdikthef.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2crjdxruh.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2mlefcwec.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ugmcdzyj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cpsmvzep.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ucfgtoff.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ydrojcxj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2sbpnhqet.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jhljqgso.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2oqmwaxgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xnojoicj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lrpwogbf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jytfyxvv.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2lbfycyzv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wgqbndek.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ulmuwywr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pousigna.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fpmuswmi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zagpeijf.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gdobbdor.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zoyfercu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qwflgodo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2coxnqazu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ltmmtphq.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2gakuwxhz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2hckxrtxp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tqiybahp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ihwxnriv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2tgbslbhc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ahfrebyk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rdjzmqsb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2yslaslxe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2xmsxftyu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2akxyzbvw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2bgxadmni.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mkkmbtzz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mvinwnrq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2vhnmrakj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2wyorrxtr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2jspwzqwi.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2llxsppsq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2odgstiiy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2cvggdkyr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qcpmqdul.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2fieluljz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2ztxphcxr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2njkbrgnm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vnzjwfdb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rvwtnqrj.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2jfjnwmwr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2veqdtztg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2dwhvxowl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wuptedyk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2uogtgnwt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bftxddvr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pvxhrfgk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2jvgakoys.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2mcjeucvb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2boriqegb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dztvgbtc.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2fkwjytck.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ndnpbgtu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xfioevqp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2qxjuqdad.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2egbfqplm.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2showxbag.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fhwgrono.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2agzjonjf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2awzvuwin.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ymnysafn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2heijtfub.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ykztawfy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2enyqilmt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2yieyeejh.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2tozevwkr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2lxasagfm.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2wnyvbtzw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2gklsxxaf.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sgldixnq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2khpydhcb.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gcrvvjfd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pktaloym.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ghjgnwln.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2omfvityq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bcmqyclb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ezgtxgdr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kpfmrliv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zbxheqod.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kequtpoq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2wnteyuvf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2qplxipkq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2adggjpxx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wuzqtltd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2dtprroyp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2bekmcyvo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2lifzrfyo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2zqgnnumx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yxcvcgsk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2uaqpdyia.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynngaytj.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2tbwqfkrv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dkxbyefv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2iburkfip.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cgjsnpuo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2awbkolyf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ktiieksw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2spuxzbpw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2egwlburq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pwyuydkj.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2skuhoowd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2itrtroqh.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zldpwuqe.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2fpgsvdex.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2sirxjvfp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2huqqeqed.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ogxhhvkm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2nvfxdwah.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hfdtkoqo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bbaduiyc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2biytjjjm.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2atorayhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jbrecxtc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2jqxyvuqw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2desjhzbc.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hfbcfruv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wvndfkly.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2lujydjkw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2pgmrcibr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vjeibmzq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2oljxgjsb.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lzofprtu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qiuiwutd.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2sbbilbwv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2hrgewfil.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bcxixnsf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2awbbchwd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2paapzmfh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2hvthlsbc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2idomuihi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2iedjflzi.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lbnxhker.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2ihxpueec.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2flbshdgu.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2hxwffoqg.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2sbvprnbk.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2whcymaob.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2lhzvrlii.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2dwxxxesa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2fmcwqsoz.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2cavnatja.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkyytrnb.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2qfbnvzxd.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hjhcoruw.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2rtfeyhnj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2xhufzfpl.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2jocymxpx.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2jtjreozm.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2zxubzajf.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2qkpqmhio.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvmvqmsg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2gxrjnjbz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2ojiqxahw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2dojavvfi.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2iovteqsj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2kbxkcnax.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2nsuqrwkr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2jszzebyl.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2edpuyuvq.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2wtejqohk.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2lnagebjq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2suhosawk.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2powjhhvy.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2sqcqjvkw.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jfmcodto.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2gnpqygkn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2xcnsnpxz.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2opwddjbn.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gesajotf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xbofjean.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2uqnvroma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqmnrfgh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nqzisxlr.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2vwxoxosa.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2xxmlgcmu.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ujgiuqih.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2shcslnjc.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2pxwspeyd.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2czccibmk.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt2mlxysoac.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt2setjkjwo.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2gihzwjdm.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2butmcuor.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fnwkussg.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vluhuede.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2nqhfdalu.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ucvtpaaz.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt2tcfoicty.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2bbchtxxg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2qkevcelj.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2hakfetma.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2ymatduzv.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yirajoxd.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2gyoczuvw.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt2krhmabeq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2ksyltgwk.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2wlefdxkv.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2bwhcrbee.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt2ojgohomo.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt2yycqajid.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2ifdsforr.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wletbjjj.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2njvsnlax.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt2ecauxtdy.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2kywibtou.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt2slrjpphp.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt2ffvhgxug.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xtzlipym.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt2ekrtoytt.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt2uzlvzoix.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt2jswmnuqb.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.52xcode.cn/Article/details/gt2nviukwrv.html


<!-- 参考信息 -->