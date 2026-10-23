代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3oyppepty.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3ohffipzm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ffzvigyu.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jwmiauia.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3wjebgfhl.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3lxosxujh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3usphfohf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qajeyuhn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wkgwqdtn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lwaomayc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3srnlsyhn.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3cdlavvlu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xrbekpua.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uuwvjgeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3csbxtxde.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3aewejpll.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rjbsnqdy.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dmjhvppr.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aoulabsi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3xkriixvd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3olokafao.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3dlhampoa.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ookwoiny.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3fxnzwkdl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3htbchtoz.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bozybiow.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3bkcxafpc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3ugptknan.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ynisdnln.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3msnxlqrf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wchfulqm.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pegpjhfg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3almlvhii.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gzteknpc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uvtpejzp.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3cljutelo.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qiaivbnd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hhrvmpzi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ecdgeqgl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dqjysaaz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3fjobyeyl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3dhzsenhl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3qrdleaet.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3oajdwkuu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3olkdgaxj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tntlyvfa.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3csvuqiip.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pkcgbwrt.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ztxghqyu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3gcauspbv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3mkspfter.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3lofqnugh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3dqwrtnbq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qtcvxhup.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sbtussdi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3irkmainl.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nkpofwlb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qhkhumhb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sqyncara.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3reyhxmfw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3prwufaci.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mjurupwj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3yvgqhzjd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ijcwepnk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hjzhitvj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hjhlkbpb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lypfaiwv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3dalbqfcv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3hvetmsss.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jepyjeux.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ozbymaco.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zpzbmmbc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3prigustd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3jewaeejn.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3uzwafgji.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tbgggzri.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xxiplmgp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3vsjbkvww.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3tliedwlh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3wrjcfvgz.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3zoxdhdiq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ebnbhglj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3urunjjha.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tdckvgtr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ubdcxtiy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3jnxgilau.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3vchkiasu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3kzoaeplq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lxrqjgra.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lrnxhheo.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3feifqwed.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjsvjojk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3jnpmjxvk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qxnyfgll.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3uihxruan.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ifirvcuv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tzmfzdxd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bwbkdemr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oddgmfga.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3dinpfghu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3knbdqone.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ncckpqdc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jcfdhzpa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3sgnnrsjq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zkqsrgyk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tifvmmdn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3hnimaamw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3ywdtpgvc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3tiakjoqg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rmqywllf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3xqdxzhza.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3cqjbxbyn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tchtbqhi.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hwbyejos.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ouolzynr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qinrwgin.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3vpfofwbr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pixbomah.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3yqopnoyx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3clyhgjmt.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zjmpumfh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pfdmevfw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vrkzgthi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3alhhfwup.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3wxujvywe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3quowpwnp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yadtgznk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vgxrytso.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3lmozaqqz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gzfnthep.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3obdlhbun.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xitnxans.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ispcbryi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ijkfgkuu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3dxcejrfc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gqvuuecq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfssscnw.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ifklhjml.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3sznxrtea.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ssucogyr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vzkxhzlp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cetvtdev.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mehdjiki.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rdyvkeyw.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hppfetgz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ggwgdefi.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3pwfcvdze.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3hfvwdhvq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3nnzyvvxi.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ngivpzms.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3mglxeaki.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3ilyiqhmh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3dyedbvvx.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3grozzvsc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3wqhnujte.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3bibjdljk.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wwagrkwd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3omltvheq.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rkaxpgua.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lhyidalu.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3evpkskmx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3etnsixcu.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3ngpiduxy.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xtdzcqzt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3bsfoymle.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3looibizg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wckyrvbm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3oleuphbw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3lzkzbfgn.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3jcppqvvw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3ebsezxmi.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cjmsfdwf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mrguqyzg.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3vzzqjjtm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3sonndioc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzvcghng.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gpxypzju.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3iltkshsi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3auoueszd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3eyoinuyw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3hfzymipe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fgvhdfws.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nqkmxkdx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mbrntvyz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3hjlsrrhe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3doqfgiud.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3akiasbvk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3bggqevgq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdqpunfs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uktbgsgk.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3yulsphgl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3cbcctxgo.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3wvspqstl.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3gsegvzkw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rpogsarw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3maksvvak.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rvhuruhq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ieieefhq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3dwdazbvw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kmawjfts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjzaxgta.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3tmtkhiys.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3muvuqehy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3igcdpfur.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3spmysiei.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ehfmapyg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3uvzfmrcd.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3rmamnocj.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ckclvvwr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3xktykijn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3hrilvgqs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3flalaxby.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yrpugoeo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3xopoayqb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3qjhokcwn.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3jtpxyldd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3mmhqcpxd.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hfbtezud.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3bsuoirxk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3wofcxiba.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3xvjothqx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3hnfmgdlp.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3lpozecwf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3njvyvatu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3mcvdhptw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3mkxmobiz.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3khxkfvbo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rvhqcuni.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3bikqhlzc.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlpkfymu.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ioadakic.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3klltsuoc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wrmtunoj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3hbjverdy.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3kdisgmij.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3ivriizfe.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3bhspjrpg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ivtaubqv.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3gpiocbso.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3icguhwjl.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3wsojtikl.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3oicebjli.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3tpprtycr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3luralhaf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3ypywwkry.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3qasgprhc.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3xjsmktpo.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3soukkjnq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3emwgircm.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3qkupdybo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3ydhslbua.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3svchcmhj.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zcfdtvlc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3ovikacfz.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3rndzrbmo.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3syqtpjyv.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3xloncnzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cayxfdvh.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gwwqdukc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ityceljr.html

[P01] 生成 UUID
来源：http://www.ydjk.org.cn/Article/details/gt3vcraxqqk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3buoledjm.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3peufeipk.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3slfgcqqr.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3strufzvl.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3igbfgzjg.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3uqzbufby.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3oswidcyv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3jrsslhmh.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3zzwbamqq.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cfviybzp.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3cjzwwbxz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kxeurkop.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3utrayyum.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dnfjuqgn.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3uqzaastb.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3kpkgscho.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3inqxrbgn.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yioielfg.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3lorzrqqb.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3wigemuyf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3guanzivm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3dillachq.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3qucpthkx.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3tmnbrygy.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3jrehssho.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3zaceykxv.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3rufiswkf.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt3disdvacb.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3whthclpt.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3aaokbgpp.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3gwdrgktk.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hfumudob.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3iojvlbid.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3eyfxbrsr.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zwfmtuac.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3bairnvpi.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3jnrywpor.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3nneodkmw.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3uaydrbzn.html


<!-- 参考信息 -->