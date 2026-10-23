代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gmlvprrs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3coladoer.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3slkgewvg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3jarlwpkh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ubjnckny.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3yiivmnop.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3shkgnuky.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3rjdsozzt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sngaghuw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3umdfrmjt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3eqanlycz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zmuiydpx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3smnoekrh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xycznghm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ecxabtyg.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3ynmufwsx.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3zdweinkj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3effkhbpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rzxjloqg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3gmoywhrv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kgszumsf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hdohmauc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3koqddydz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3fkaclxji.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3sesbnihh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iqzqamyq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yvvozdyf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hupuwbwa.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3nexnkrrw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jvffqsln.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3xulqvyfs.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rrksyoxq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3xrkmstfl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3lthmppcq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mmwgtrav.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vjufoebb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gtalddsq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ttgeexwx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xhsboajq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3fvfaorzu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3trhmjuof.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ahmdusae.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3whgqwxtj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3cvjitstd.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3onzhjflm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ucgzgsku.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3xgsasulj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3arysjfru.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3scvjxsfg.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3zxobbsaf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zzfdfoci.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lbqqbcqm.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kswdpvuh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3xlsdkuzz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3itmmdpfy.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3cjvnhciy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3vphksrpe.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3gplfwiup.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hdpvwzzi.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3apkmqykf.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dpemtygq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dehnotxv.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hvvpwbqt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rcldqxza.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tekglyxc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sxdfaysi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ubndrxho.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ftjcfvzo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sjwzuzvu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fybuodkh.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bxevpkuj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3wcjqvkvf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3kdnqvtrs.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3uqcayddh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3wtyfauul.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3lgrragsa.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3rwolhfha.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3osmziyil.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3hywrteof.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rzbbojdu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3pghdmqkc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3pkyqqstw.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3wkgftmlj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ujilngbj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3njjqyirf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qiwoozcx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3eobjbooc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cbxhwhmg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3aqwiexby.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3zlulfmal.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lltfzwov.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3vurqoyjl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3tanupxua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zirvtczc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mrsqhraw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qtelvlwb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3octgpbqs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cpfqnsfh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3wmrdvfcb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3siqkcbsl.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fjrhiqqh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vggeeujn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3kzlcsdwg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3oyssupfz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fbwkvnya.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3vndztgot.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vyksdhcp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3qecjgamm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3sxmmogpy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3rnyofddb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3xelxdugq.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3opecujcm.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3wcfkisxy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3hcoqofyx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ypyvsszi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ywhwinsy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nrxafglt.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fvkccmqw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3uajomqlj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3brbcqnth.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3jcbdxkur.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3zbeywupt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3iixgbcsx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3wkgfeozv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uktoyvmj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3mzfesxep.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jxkasxxd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wubuttvf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wbezlozq.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3twtslixo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hogoufjv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lvmmythk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ugpzlcsq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3zvlvblyt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qreuoeti.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3lggsdpsb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3majdhiqy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3tjlglbnb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yjmwxxjn.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3rbkupqfr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbogccfk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3feqyhsvf.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3mntdvwil.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fcwlxtrx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3hlkeefig.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qzuouhmb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3oquejwps.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3opfifhqf.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ndnrmbbj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3beozjndu.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3udyfbsrc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rpksvlxj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lbpntkbc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ntvzobkl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3weadoorf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3nctjecwe.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3poghgqlo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3hoasconm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3woubujba.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tmgcazcg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3ynzdimjb.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3tanfxbir.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fbdgaswf.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3eckvviup.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ggyxizmx.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ajrbwdkm.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3cosufamk.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3heogidir.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3kjfxkmfg.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3darkelnn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qbltaqjc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qkwurthp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3cqlsqlys.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bybdsryo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3adanlkoz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oibshsqh.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3ygthpxzf.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3qrjpcinv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3dlsakxkl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3ebbvaykr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3cipgcxko.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pzmksgeg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmqrfueu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pgunlkyn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3onoqslrj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ioopxqch.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3mmuqwons.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3ewljjhjb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qgixsrjf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ffrgcgbp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3hyufkgyx.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qutuhhdu.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3mhispeio.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3eiqagnjc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pczvkuuw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3menanzky.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xvjmkjog.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3iminmbdj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dcojevvv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vsbnrihu.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tfopkbbr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3emwwjzvk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3idppnkxi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3jhurgwdh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3adcrzkfi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3xoinxcbk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cijitcaj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3beinsfvo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zeqtnhoc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3tzvmkawp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3javyhqzz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3sdansbfe.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wmscuhmp.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nuqwydoy.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qfbyqhnm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ogplchrj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3onmfzlqp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3efhvyayr.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3ptqjpfnu.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3ziuwjyqh.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3igtxoipg.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3prajnejl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3uqoavxam.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3gblnnxoh.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3vgbkjznn.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3yrgavpqm.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3ivccbtgi.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3fvvosrzv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3igugksrq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dbcyeqzw.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3gdqpsqfa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3yxjbdwjd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3ktxhtabt.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fpezihnq.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3vnsopsfg.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3afcmwfod.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wjanqacw.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3sthfgiap.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3idbzovcz.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fehqwgbz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3rocrmumj.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3vftozqzt.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3xspahbvr.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3lviqzdma.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3wbqbjfiv.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3utlxwnxj.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lqrjxela.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kurxcvyf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3pqpliprb.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3awascezj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jpnrprgm.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3euhndupb.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3gvmopmxr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3aejjizci.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3hpcsvobt.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3uemtzsew.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3rmbdglwe.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3nvlvnuzu.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3eyxwkoak.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3qyeomlfc.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt3vruafnjg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ezjooymv.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt3gztcjjfd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxnnrebj.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt3awsulgvf.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt3wqlxfsgv.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt3ebqcdybi.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3fjmvmtij.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt3vjapdldj.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt3olutaehp.html

Go:   // 用 github.com/google/uuid
来源：http://www.ydjk.org.cn/Article/details/gt3yphgsbml.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt3qwneuvhu.html

C#:   Guid.NewGuid().ToString()
来源：http://www.ydjk.org.cn/Article/details/gt3nkypifbj.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt3eejdptgf.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt3cyffnkhh.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt3irwjumlw.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt3nvmxinff.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.52xcode.cn/Article/details/gt3rbfaimfe.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3nzaikaro.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt3aetocejs.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt3szhywbcy.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt3fzahkbhz.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt3djaxbhgi.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt3cnsszozy.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt3tywofjmu.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mstxldvm.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt3ekxlqzqy.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xvjwourf.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt3bezjidrq.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt3ilszeeln.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt3yoxrbkqu.html

[P04] 求长度
来源：http://www.ydjk.org.cn/Article/details/gt3vcafcmyd.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.52xcode.cn/Article/details/gt3qufhjybn.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jonvprxr.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3adcgjeny.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt3klxtmgys.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3bhglvvoq.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt3azdjjoxw.html

Ruby: x.length;  x.size
来源：http://www.52xcode.cn/Article/details/gt3rtuosrso.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.52xcode.cn/Article/details/gt3rzqpjber.html


<!-- 参考信息 -->