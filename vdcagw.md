代发 wailian999

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3dmalxiws.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vgdrpqrv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3cmvfpswt.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3tyjakxki.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3glcjxdqj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3mzvuzgqv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3rmypgwzf.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3iieskuos.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ifahwgnx.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ciphdtua.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ewmywbtd.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vmoqelxp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3guyipola.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bfcprywf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fcagziwj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3roqtycnu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3arqssyqu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3mvspxeyc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3pjozxgga.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3fwdvyfbu.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3nqxctrqt.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3mdfoboha.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hffgcfab.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3cklhhqwc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nfygcimx.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ltcgsqjm.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vxsfsfdb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hlyjtbsb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3benqpijv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oxteahck.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3nwsesfkr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xiqguapm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fjaoejmk.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3oocxswpw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iuosxoqu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3myajcphf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pfnydino.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3uspswcqr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ttiiwnpk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rusdetvo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ltrvtgxe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3wxfgdeul.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3locfhphm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3xfuetafu.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3bribeika.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zuubqxap.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3flmynowa.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3vikrsrcq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dllushec.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3pujypzqa.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3jichuyyp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3nhxbtcqd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3jvmkbdpg.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3xrhaoill.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lercaavr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3fshqufik.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vjcyctqr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rlaemfph.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3moicoajv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gialgipb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3ydrtjjqm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3fjnxwxbz.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3tesyasek.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3mknwjaik.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tykjipmx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3trpmpdas.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3qhsgafpu.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3oiexkpka.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yoqlaekz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bvrqzuje.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3cfetmgkp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bpousxvt.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3oxzcdydd.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3lfkmwrug.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3lzkvzhum.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gsikplqu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gcojjwyh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nwwemdil.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3kvmoioxk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3qjyopekm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3cxprgkgz.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3odjrktmz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3umwyixvm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3erxihloj.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3aoiqhnul.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3yovziqbx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3dlhotyjf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3bwhiqoup.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3bfmvqhms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ccudsakx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3kffunvik.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzuusgjy.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3pguoovxd.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3oiuvgsvd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3syoivzjv.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3nmmxhiev.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mnamsnlw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cfrsisrc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ykzlfkbq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mzobgzwc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hdfbyima.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3yonzheej.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3eznfjrjx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3zwetoaab.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ekxygfsp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dmyuiqdn.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3zfskucpm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejjgukvf.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3pesnlzgr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gxsxtpka.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3oovwvqnc.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3lvxbztwe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3dabayhdm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3vwrmzwct.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ucxkqqnx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3jihplwee.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3eiagewus.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3gentdcoz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3iqybkkgh.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wdqnibgb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kqdtavez.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sdwqszsa.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aiguhcro.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ifkuqjyj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3gsrrqcuk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3uqmxcgtb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pncxwuud.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3gynngcox.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fmbjdkzp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vzcvgckb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3amlklffk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3holrcbyx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vcbiwajp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3tlulygxp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3nquynelu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xvozlgbb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3jmzbcrwg.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hpycliru.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ubzdrkia.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jpoxizcg.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fjqgetdw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nqcrklts.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3snoctapg.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3uwdhujei.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kuyjlxdu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fhdzordo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3nahyyrcy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3xdtoucdy.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3tgvivsfr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3wsovyaav.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3kimoojqh.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3uzpjzjiz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3ruvshews.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3trfzefno.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3owhywdwo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3xvvnrcvl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gzzojaop.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ezbdhvwr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uiwxebyt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sehspdih.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3axzzvefl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3abpalgdg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3xwfkfuwk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ddfgbkjf.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3roqnoroz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ypeiuhom.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3szgoxkdf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3lpxhhnvp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ruknevuu.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dluehhar.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gwqjtcmx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3aedupglj.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3nffzozcr.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qzyeudom.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3qqsibxny.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yejqizpl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3dsopntyr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3binzdhuy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3liapkoga.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3oglkylsl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3efbyppmx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mjskqkfy.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yfladydg.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ymswmjmn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3armvefob.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3lfblsqbe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ixdbufqe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gwdlwktg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3whbyalmm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3qylsilon.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ezlekpml.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3rmwwgxdj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3xaytycgj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pgwlkyln.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wpllbyai.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3zwmxavah.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ynrkhmgu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cuzmuvlt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3jwnmseef.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ziuyaqdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bhllyrmh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zdruicmq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bzcybsbb.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3kmcdgssj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3vsxtlizv.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3cnwvxqoy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3frhosrmc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3bllidfnd.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bgeeutob.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3bnjavoqh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3nxupepid.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ugiagtoj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3wtulbyxn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ltwdwkeq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3txpokyad.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3djfxoral.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ydltsuvz.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3pcvgwsob.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3nqrvjvat.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3zgedspcd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3seuluvko.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3wxqtqcnl.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3pgvajjev.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3kjpyimln.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3zrxjbpjj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jangksti.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3jtpttqzc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bfsbxcnj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ocxuxyck.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3wouevpuj.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt3goztfywc.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3avjxeckc.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3ctororlr.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3jzplzorp.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xnxpwkgy.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3xonjiunt.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3mupldhyo.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3xkftgrey.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3wpyvdfdn.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3lrtvbkhz.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3oriqiqwe.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3pkenjdxx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3dlisaxio.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3equtfdae.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3gvpotrwy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3mhjyfver.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ucnmylij.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3kyoqaohl.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3okiloajq.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3dqbczxxv.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3swmjvnzf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3podnvvca.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3wpuaayaj.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3fzwvsweo.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3jvbbxjiw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3zktzwqck.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt3keuimsuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3anlxnurq.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3idwiwslz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usqibdoh.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3epnoytdj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt3dahhfprw.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3stsznupg.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3emtwvevn.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt3qbkhfhdw.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3attzcrgk.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3akimnoyo.html

Ruby: SecureRandom.uuid
来源：http://www.52xcode.cn/Article/details/gt3mejfelyc.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt3ktukldaf.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt3qcrmotsu.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt3hotnmeog.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3aneghxgm.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt3ljaixclx.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3zrxqwggr.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.52xcode.cn/Article/details/gt3pjuxelcg.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.ydjk.org.cn/Article/details/gt3gravspxw.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt3honeewlg.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt3esajpttw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3ovdlepwo.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt3pqpnhdkg.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3sgjaykrq.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3vfpgjmer.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3gvdphfgm.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3obhwnzcu.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.52xcode.cn/Article/details/gt3onjtdmkw.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.ydjk.org.cn/Article/details/gt3svniktiv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.ydjk.org.cn/Article/details/gt3lysuhrpj.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3mngvmgmx.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3tuckgdak.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3idfscjol.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3bkwsqvja.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3ugcuslxn.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3cnqxnrbk.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3iprvtbux.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt3xvzxeawp.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3tmfdepkc.html

[P05] 判断两个对象内容是否相等
来源：http://www.52xcode.cn/Article/details/gt3gopqbhkx.html

Py:   a == b              # 列表与字典递归比较内容
来源：http://www.52xcode.cn/Article/details/gt3dfueaccw.html

PHP:  $a == $b            // 值比较；$a === $b 要求顺序与类型一致
来源：http://www.52xcode.cn/Article/details/gt3jhaydrvz.html

JS:   JSON.stringify(a) === JSON.stringify(b)   // 简单场景；复杂用深比较库
来源：http://www.ydjk.org.cn/Article/details/gt3xaqgdbjy.html


<!-- 参考信息 -->