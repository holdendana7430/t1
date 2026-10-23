代发 wailian999

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3iviwfzph.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3cgzsklzn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3rkeowomr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mjhvdczt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xmxcnwcw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qzgwszdn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nywilfwk.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3uitmtllk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xnqojoxf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3vvcuhuzw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lxjuzmpi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hhzvqxrh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zthrvryz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3grynwpzq.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3schimchr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3zcrionsb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rexbutqo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3nueealfo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3svpqbltv.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ftrpphrw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3hietmshl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ixwumxdk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3oehypxgg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sogvcfyy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pobrsftl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ujaqowab.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rzsjcdrt.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3qxzrqvis.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3weahzyfg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3xmlsfqfe.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iyjkdwou.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uvcekvjf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3hxsxdmfi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3voliexvn.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3iaytsrha.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3idadzffk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3kkipacju.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3tnjqiamw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3jzpagtsz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3iunyadtm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3etdhdgbn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3mfqxhyan.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ncoaurwn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zvugzzny.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3qowlbtxg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3twsxdhuy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jmbvjxwk.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wyodxrfb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3kytgqstl.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3frwtiblw.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3svxftulg.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3pvfnekcp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iuncromr.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xgqcgkyu.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wdgqaqxp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3lxfmbjuz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3omznlbjk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3haajksin.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3zuuusqfm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3xpkxnewy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gmmbejuv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3suobgdmb.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3sslqkunp.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zenezjuk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vttugrbe.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3pswiyypc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3keczrwqr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3xuwplwmr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pzwxmdor.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kpgzshse.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hyfhxzat.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3idhozczo.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qozjrnre.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3oqcyszwi.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3waevwuzv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3jyahxpjg.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3trqfzqua.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xxizyrud.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3skxtrpou.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hznekrly.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3rqyqtmlf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3yhspfxjy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3nrfwlrov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dmnshqrz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3tpdbyqqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dmnvcsvo.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ntnhxijv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rnqsqbpy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3qwybolzw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3opvvxjck.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3obeegycu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jweujvru.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xginxzst.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cgqsmzls.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ibqxstmg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3binkkbev.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tzjwusne.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3pdnmfeot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3nhzvlszy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3krycwxxd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wuuvkjpq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sorrdixj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3pgvfnkxe.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3jdrvjfhh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3crwozqgw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3fietpqlr.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3yyprszxt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3fagsurpf.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qqiyxexp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xeiveikx.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3bzyawzbo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3rdtyawjg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jmmzhlrz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3hycwdeqv.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3rxlanjdp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3vumjijfx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3eiwleinh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3hkxvqffa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3niystaxt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qyuleaxi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lkpntmdj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkimzhw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfqjiubi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vstvfrwv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3mjrssovj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ebnfiqmp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3chpmeraq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ovavkcdh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tpckbyfa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3jmvatlly.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3unsuxfvl.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3bjoibzqq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3opoxvljp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3thaiorcb.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ytpucnra.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xhzxtnkv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nmcwoesj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dlxqufum.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fevcwdwc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3lhutulap.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mfxwifgc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kylklxsd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3gyddkbdp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3rxerstsk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dmsoexyb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3csjarlzn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3ygrfeahh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3gmuhxwgi.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gcrvvyqo.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3nndjltod.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hihhexas.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3ocaaxybq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zfprjcoq.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3zhmpuvrp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3unoxkadb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nkkypcfx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3utwzewzc.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3gsilqbbs.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wrsgvogn.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zqxnnyta.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3mgbxpaqg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vqhwpfxn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3updpspxv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dqfazmyv.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3rsdkqtbc.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3drnfcafn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3wsucklyn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3gqdohpty.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3scfcdlma.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3uoeldcgk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zbhlenxc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfnxvgqr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3pwvicvdn.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3vaikmutx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lhlaltyu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3jqapslzq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3ruhmzfnm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqhyarnq.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mgybrbcb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fiovakei.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3dcrhiqbv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ljeanqqx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ojamuvir.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hbrhhfnw.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3azlpdihz.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3uadpajkw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kwxnfvss.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3vryqxyij.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cjphdqsp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pvosqnfq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3azkskmfk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3xwouspkr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3csiwmvuc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3wxgqqutz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ediposxw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3apmsmlzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhsnxcqo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3pxdltdan.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ldigudbv.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3iamjfodo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3aobpnqom.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3abwwzxoi.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3aqavarjx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3jviugsxs.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ltnlkgsm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3uxxvzpgs.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3ylzdmojq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3cdzxbaor.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3iqxnbcaa.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3itorqzij.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3evifmswd.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3purtiwca.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3jzcjwsmi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3seqawumu.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ysghxkkx.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3cscpsull.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3hvolatjm.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3qkkytpgf.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3dmyghnye.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3asprmzay.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3kswwxzge.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lxuseayo.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3foqhxzhk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3nmemcxez.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3qwsawsiz.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3wxjedajx.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3uuogfxhk.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3mawaopwp.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3mbbfhqyo.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qapkzswz.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3qthnhwil.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt3jmeluhim.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3xomuesnq.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3riolbpsu.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3xanrtmcw.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3szntiiqv.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uyrabdvp.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3qmuscbol.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3oonsbrqu.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3nubceraw.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3zymlcjqk.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3tratncnj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3dkrjyuqh.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3jkfmiytq.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3xnrlwvxb.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3abrusnmf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3zkakofum.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3zozrtfpb.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3jejnmxyb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3ubynhxsj.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qhgaaukm.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3gwjovpco.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3pdhtyufh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yspskyjy.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3atshshvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zlumlejq.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3pctxrvhu.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3ljkrtmsw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3akicbrer.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3njsxyxdg.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3dileexpr.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xwhpgzfd.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt3yoqmozfw.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3vtjqdvtm.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3cpxdobgc.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3onjnchko.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3ybvsvmfl.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bmikgcot.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ydogbwmj.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt3rspxvovn.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3coklgpya.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3jeniuzml.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3obpfeqdc.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3iylfuteb.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3tzocihrd.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3heavukls.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.ydjk.org.cn/Article/details/gt3nocobqcv.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vljrtwai.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3iozaypza.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dwdydehg.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3iaudjwus.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3osgzqwde.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3nqgzthym.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt3mnudqqvn.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3lkxgfdvh.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ufmzojzy.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3qjuzwhkq.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.ydjk.org.cn/Article/details/gt3haexhpcj.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bgzzebvw.html

Go:   len(arr);  len(m)
来源：http://www.52xcode.cn/Article/details/gt3fmxcxetz.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3ypbazktn.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3pavuerdq.html

[P05] 判断两个对象内容是否相等
来源：http://www.ydjk.org.cn/Article/details/gt3whfdqnkp.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.ydjk.org.cn/Article/details/gt3xikwxcqr.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.ydjk.org.cn/Article/details/gt3hpwidqud.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xgvhdfhk.html

TS:   JSON.stringify(a) === JSON.stringify(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nwuphgxy.html

Java: a.equals(b)         // 需正确实现 equals；数组用 Arrays.equals
来源：http://www.52xcode.cn/Article/details/gt3lenmvqzk.html

Go:   reflect.DeepEqual(a, b)
来源：http://www.52xcode.cn/Article/details/gt3flwfabij.html

Ruby: a == b
来源：http://www.52xcode.cn/Article/details/gt3jqvzeaer.html


<!-- 参考信息 -->