代发 wailian999

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rwrnyvfp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rwuhewiy.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2kujlqixe.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gqvjbykh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2grnlxcel.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2zernllfb.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qhrwkprm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dmuwvbko.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vsscgfwl.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2icmwkigv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mcjrucqp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dwiainoa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ibvgjxph.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hqzbeaxl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ixwbtpwe.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rbiviayj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2exoucfov.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wgprtbfh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zsylgzem.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2yzituuyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrxollhx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ikihvswe.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2rjtafpeh.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qfqdmbgw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2nrczgnhh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fgpzteyi.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mtzgxrsg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ymwquoew.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2dxaiuyqm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fjhiltpo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvurryxl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kaxeivhv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2udomrusy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mfomdklq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2cjgwyeqh.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jdswwame.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hykpaepi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ulcjyfyr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bhqnzxxq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2njmbtaqh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2sfizenoo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zmuucvue.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vgevxitu.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oerkfgla.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2inktanls.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2jtvxwqdc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2rntalvmw.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hhxqmwba.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2coxwehvk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xxcyqlle.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2twhnfdec.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jjxkstie.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2itfhajiv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2umqnboms.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2htjroata.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2boiyqqoo.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2bbdgvqbt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2odnfetgg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ntwjrilo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2takykaau.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pwezvsvm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gvfpiqek.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tmqlycvd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vzfvppfp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2pfytsdzz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kvvaepfq.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jamlfyjd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2riyrwrrx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2urhhgygw.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2dbmsximg.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2uqedmtfn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2umdlknum.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2ncnqmdsd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2hkvysmrs.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2soluzoqr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xvbhpzlh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2kdnsopjq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ifcscnvu.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qewblmeu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lgzcjzof.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rxacuouh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2fdqzcxfk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fdnozlrj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xcvdenob.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2lnzctydj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2conwstjx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rvrqujai.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2chyrkhco.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2xefhgyvl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2yqcttelx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vylqlpjz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2eluiuyhh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2whvywcqm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uzgapvfp.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2bafwgjbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ilariaom.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jyvnttgh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwgzushq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dxnkgugq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mcmxxzmi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jagnietg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jenfrjak.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qfnybmsn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2kamyjcam.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mgorbieh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ocizgxrs.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2urorpudp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mtsdibhw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2oxyyuyfd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2udxssedi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2mavrcdax.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2iwkjzfnh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bsklfuyr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2velfpipc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2cuigsmfq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2apmuvwyk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2bqmkkiip.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vhmyetfm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ooaqfajt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2azxacitc.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2glscxpcg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2blnfaous.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2frkkniqa.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wsitvrrm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2yztuuvae.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2mnfepump.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rxmchltl.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2pptllyku.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kplngwug.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2limkwzwj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2bkcalhtf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gofedrtg.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2yykzhsfz.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2risvcums.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vhtyuggx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2djmayfqf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yyzstitd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2cmtnyhno.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qcfkrrqi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2djpfyzdf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2tnfltneb.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2spjlftgs.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yfxlkpgz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2raijdkyf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2isrfefrl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uvqcoeuv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2kqauqwhe.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2iauqwpdh.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qnmpdnnz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2skagstgx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ubkchboc.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2paxhlpxs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2setahgua.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2suvslfsr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vyajznbz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hncvctgc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hhmijgqs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uxvwqohv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vjgbdrry.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2sjanbyzq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2weeyfhme.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2nnaehknt.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fozjsmoy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vakpoeox.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2erdzjgxk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aqvlhidb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2vfwiggab.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aflvtgzv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xpkryluy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uobtsths.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jsxzcrgn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qaknxwkw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2cmhxjtse.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2nnnzlpjd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2zomxfnuu.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2inhjmhzc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2fdqtgmej.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vglcjkgw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2eqrmtabk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pnhljkdq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zennfouo.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yugvruwa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2rpzzidsu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2urmsigiw.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pstloeoe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mruhtgoz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2mvxopnpb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2jyufxcpu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2toaupzku.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zbpmxloc.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2paukjzzp.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xerdmtod.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tabdyjga.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2qdidnknx.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hdeoahnu.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2cgceycoy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dgrojrrg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bdcbpopp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ouaegebv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xiehmlvp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ttdafpai.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qzjfhahy.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oemoyabi.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pskkdxxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eehahbgo.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2krhwhaoq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nddkfwiy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2hztalida.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vncmbkhw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ykdfpzlq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2qnbafxvp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2iysjzzyd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2fqvlzyzq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2oajemmom.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mhoxjquk.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2dpnrctcv.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xemvqlkp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2zpmbtndb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2fnytmyku.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ebkznzyl.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iknnfpyl.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2rapexkxz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2frjqfptr.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ignpkzqi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2fwxshsws.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2pqdrizbq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2afbqbnbh.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2lbtdsrde.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2bwwcvrot.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qbqqfddm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2xzrxkjdc.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2wovpmufk.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2evfoevea.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2zedgetoz.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rfdwbdic.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2anvwwdhq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2dwaexnzj.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2joggyjxt.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2oasninfr.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2kpugoblr.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2lyjfbwdp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bfmkldgd.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2kgaacvpg.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2pmlkcgql.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2rgtkblik.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2urhjoyoo.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2icpsorvg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ldlgcipp.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2ibhaunhg.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2tuqaobll.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2dbwxlcjy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2hwznipeo.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ywktvkpd.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2olzzkdxs.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2fxzmtiuf.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2cowkycsf.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2jbuodzkv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2lllmxjhw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2pfztxuxu.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2jkbiuxgg.html

C#:   Parallel.For
来源：http://www.52xcode.cn/Article/details/gt2ocuetxum.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2llvlvnkl.html

P. 常用工具函数
来源：http://www.52xcode.cn/Article/details/gt2nvifiqeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bteewlmu.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2ryhqdtyt.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2ppxofvdi.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2igakhnjl.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2bsodksmc.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2qkdxuvrk.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2wabosrda.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2mbyjwrcd.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2gkfsldrv.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vkipqkfu.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2wtfhbrox.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2zmnpotiy.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2cgbwgxkz.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.52xcode.cn/Article/details/gt2wukrwchh.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2oumqkikm.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2goiwqlgx.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2qsjosphu.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.52xcode.cn/Article/details/gt2ixtnprkf.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2fdcqfaxw.html

[P03] 生成短随机字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qwuoifhe.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.ydjk.org.cn/Article/details/gt2ixrdltjl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2yrnphuxe.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2erqxpatn.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2eqvesnjr.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.52xcode.cn/Article/details/gt2xdndjgab.html

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://www.ydjk.org.cn/Article/details/gt2cdvmzztk.html

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.52xcode.cn/Article/details/gt2hvqpcgsv.html

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://www.52xcode.cn/Article/details/gt2jjavyxvg.html

[P04] 求长度
来源：http://www.52xcode.cn/Article/details/gt2dyenkbjk.html

Py:   len(x)            # 字符串、列表、字典通用
来源：http://www.ydjk.org.cn/Article/details/gt2oaxbyfxo.html

PHP:  count($arr);  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yzqgizfi.html

JS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2tbwxgxzc.html

TS:   Array.isArray(x) ? x.length : Object.keys(x).length
来源：http://www.52xcode.cn/Article/details/gt2amiaoump.html

Java: list.size();  map.size();  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2excvcrip.html

Go:   len(arr);  len(m)
来源：http://www.ydjk.org.cn/Article/details/gt2yxkefgyr.html

Ruby: x.length;  x.size
来源：http://www.ydjk.org.cn/Article/details/gt2jciawoer.html

C#:   list.Count;  dict.Count;  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wrfsppno.html


<!-- 参考信息 -->