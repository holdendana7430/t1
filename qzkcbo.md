代发 wailian999

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2quxrguws.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xxiruwgi.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nhkjjwdv.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2aptoiqqp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2rkhfkfou.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2smpghuzr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2stwngljh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2eshevncc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2qggspgqi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2pffufhwj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zgznrimn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2oepmfqzf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zdxzgreq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2pjdjoajw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2mvpgtdkp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mpfmurdu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2vwszsvws.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2vovgwwsp.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2crrirtyi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2kjmigoch.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2hpxcksnb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2uvfgynec.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2giyyudqe.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zglzczgz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hturtirv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rimyfptw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bshlwswq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2njgmwnip.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2svkkfhgt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2dwqnupvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nbfrxhpc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2exmbbida.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gjezbflm.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2swjhnfnv.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2rrsnzbqq.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qjzoknpq.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wnpoejwi.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xgymgjlu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2qcgyhfyd.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2tixcdibx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2lxjeacoe.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wjwvmbwk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jgkzyzvw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2diybrytv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vsmljhua.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nmztrptb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ikywuesr.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wyupgzsh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xumpfcjb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2iucugfnn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tclzrkms.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2oagbyplx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qcmcrpgl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ppekduev.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qicqpjln.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dirzvrbx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lozgetji.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ndxsxbfi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2kiynbmld.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rhvngrpq.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2qlyyalzc.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mjhyppyj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zuffrfki.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pdstcunn.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2nvhvnskt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2zhjqnklv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vlhqemmr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qgpdxmoc.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2lgysxhit.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ztkqahrs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ljbsican.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2nlrmiwrx.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lqddafcq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mixvmtcp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mmvbttgg.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpqqulbm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2oslxwzbe.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gkkrlhep.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2pbgsiomk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rugmkohb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jmhfdtgi.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ufshjllp.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2klzkbssj.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2fakrezpn.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2edhwfwcv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2yctjmzxi.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bwctjyha.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2eyywxzhv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ifavgxcb.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2jxfmipwd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gigplexd.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fjltzxkh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2tqvptybv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2lmdwwjki.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2yxjhisns.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ekbzrlkw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uvledavi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ikwtycec.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2fbdjzobj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2wbmyzgub.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2symilvju.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2mngenjic.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zjgvawyi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2kwvptimd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ghigaida.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rfshqsvu.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zzqdbbvn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zjcebtdi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2fopypera.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zcnwsoog.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2rqegtixb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ttansnyn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fovswsar.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jazqilng.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tayrpxdd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2zpymvkya.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ljgwramr.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2tzpmppfp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2glcuzent.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mwehvjrh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2smabhamq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ndervtxk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nppvmqva.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2hayjnefq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pkeijgwv.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2xzkjvowt.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2fbqiuugg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bayqilia.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2uknvxhyq.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kzdbwklp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2grgapagt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2xeriznwm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ppzdijiv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2lebdfptl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cobbfztx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2lughpxtn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rmggmyfg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xiwnyira.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hhcgbljj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2repoflcz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rlldcwzu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2mvsqgfmx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ugtjlxhz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2grjypygv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2dlhrsvpj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2glsuowio.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2tgyyesyq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ffjtdyxu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qjlkwkim.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2jmvpgnqk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2faiclzhw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2brepdphz.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wyxzvfvo.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2oelmafuw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mgostfrl.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2eospbixr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dxiisejk.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lfwdcguf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2fdfuzwqu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2euplrzap.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2aamscfaa.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hcombubx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2zubmhppa.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rknshvma.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2icwnslcw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2rvqfceuv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2tpqflydq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2aqgtofru.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pztyvrqr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2venevvpi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ddchqlee.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2eatippsj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2jztwrwhn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2edvsquqb.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ngviaixu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2yfmabits.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2pwoqdzuf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tsrcbqxo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cgeuoqid.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2izaoblen.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zgzdekks.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2dibwscsp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zmibpyda.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2uwafuunf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2upksvwbf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2asxtqlct.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qbnzkujb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jkdgsiaw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vazwcbwm.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2wvtgtebm.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2vbawhwsu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2dmcwiuql.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ylndqzmr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2zvyptmly.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2fumewbui.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mlekhsgv.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2aabqyatd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2inoyuznk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2essmnltn.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2dafffvhh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ekzhedyh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nvlcitgs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2slrxdlil.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nxpymdce.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2potrvwgd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pextknqk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2swezszlz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gosqnmva.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2rncctpqh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2zulthrne.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2abgehuiw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2yiuupibn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uvjhnout.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cshvavzn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2pyikcwuy.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fwanfpbr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rhffzuaq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2eqdldqdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gktisotg.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2zlmaqyhz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ckbiuizn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2bsrdtodx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2judcvtpd.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bttwkoms.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zgnqjftn.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2fzijoksu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2wtrlceck.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2quxijwds.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2ebdenabr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2foirfjdc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2baibwehp.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xjauzchv.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2onscqmxn.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2zuqaehqi.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2waogotuk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2pjqjlwgl.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2yajyqjet.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ozzgibxq.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2cqwilbsl.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2byjqyyjm.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2sgdcwwwo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2nvxcmkrl.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2dchrrpya.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2klfbgrbf.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2tebziliw.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvzfxibi.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2thgdgzsb.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2merfobcj.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt2ozdsjjbe.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ditntcbx.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2qtqgfzqg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2skqiptun.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2jkvyjbhx.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2bsepqksy.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt2zujvposv.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2lpyibeqk.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2pxrcwqgm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2mydyvmlu.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2zvrmtnci.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2ysdtdmxx.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2mbpivhvl.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2yiaspwyz.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hieiqiyt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2mgyxyzzq.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2bllyhyqu.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2nxtzjbzf.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2axezqalb.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2hvorjgpb.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2jimxtrif.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2fdqjyfoc.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2kiibmniu.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2damrkpsl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2xcyakgez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dffdagnn.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2oujkwchy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gbjllzas.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2hacsxyoe.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2blidwbvu.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yvsmhckr.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2ajndiyli.html

TS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2vcsivcez.html

Java: UUID.randomUUID().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2czsnvwmk.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2ofanwzel.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2ocspaoos.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2zsbnuntk.html

[P02] MD5 / SHA256 摘要
来源：http://www.52xcode.cn/Article/details/gt2dotaxwil.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.ydjk.org.cn/Article/details/gt2kjijektm.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.52xcode.cn/Article/details/gt2nowhrzbl.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2edcahzxb.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2yuhewcmp.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ebhevlpl.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2verrbsoc.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hddkjuuv.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.52xcode.cn/Article/details/gt2vovxlkyw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2kbkkagkw.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xffyjupl.html

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://www.52xcode.cn/Article/details/gt2trelswgf.html

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2dlwjilbs.html

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://www.52xcode.cn/Article/details/gt2qcfxwbyl.html

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.ydjk.org.cn/Article/details/gt2usxwoxik.html


<!-- 参考信息 -->