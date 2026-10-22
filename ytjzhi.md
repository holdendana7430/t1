代发 wailian999

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2kxyscyeg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rwcwpbxh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ugimrzap.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uhvnbcrq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2mmhojgvr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2nibtbfgt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2acrorgks.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wmusrmwx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2blqwubwc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zlcgmwrr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zslhenzy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2drfqgdzh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wpxzlqcl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2znjuutvz.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rlfulmas.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2mcsfxorh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2urqgxpgh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2shqfhqpj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fmddpseg.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2anbycfzh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gwkxzrxx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2zgyxudjr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jfggygko.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wbeqjymq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2svvojxnw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2pfmgvvxf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2loxajsvk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2gexbalxy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rglbdpjs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hicczwcl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tdpsyuck.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2yavxnypb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2rgeuznxp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nrttnyoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2shurqgac.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2crlbjuvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vpgqcvmp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2piqsetzi.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2witicgyi.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jltqyzrh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hjvgnmxh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktzpofcl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2phnuykpm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2wqriwmtz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2afionflw.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dcygcgli.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2bdzenmwg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cpqgyqog.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2penanmfz.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2varmtwty.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2zebhbrgc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ijrrwzvn.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2oljntszd.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ihrvhhsv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pdfjsvqp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2evffllwt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vdlkwvcp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2cnfealvw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qdcsrnpy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2azplttfx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2eiwitpbe.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2lczsqutu.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vslddwos.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2eyphshqd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2teehctjz.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qauaeenf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2qiobjcnt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qfcxhdkz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dghrwxnc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2maagbokz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ltlugwoa.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2iamhcino.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ebprgmsb.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ninjvymv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2thhahnya.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2uolhbvre.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qjsvyeuq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ilfavquj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jygnhisd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rvqunkbx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2radmpdil.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dbupucad.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2msvtvkhw.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2kdcyyhvy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fzqasjnh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2neahooqm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2valqmlcq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2zuzeahlw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qqgssqtv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2guoyapxy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hoytuztx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2extxjlhe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2vggnmnyq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2inudhvvp.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2nghwajnj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2uuebwznv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2eihxyvfb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2oegwlxtx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2agqawikf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lyikmsby.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2gxovvujb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2umapfsfx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mbrgqznm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cnxqfhff.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bfxfxpux.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2yfhcmllt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vovfqoqn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hmuoedzr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2huzzqosl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itujjrnn.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gnbvboxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gstejchm.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2kqslzxwk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vidpuxfx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ysmdenlu.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2botdqipt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wilwedtv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xumwdeeb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jcqtsfxu.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hulgbsaw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pkliqhdq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2dxradlke.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jmwzyvjl.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2parrbulm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hcbidmrw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2egfahvdv.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ehecntet.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ddzutxpx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2epruixsi.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dhhqrdub.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ovrfitmq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ipzwvsii.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vkjkpdyo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ynmerxbe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rubzlsef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qltbuywh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2qwbvkjnw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2kzouuvve.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2answgfdc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bddgzubv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2osecajlp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rnuabohk.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mjzklmer.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2azcmkqrn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nrtthgdb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2xvhnkuha.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jdjxizck.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wgfuvtxn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2bcvrqxhb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2oahhxkyt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wntghqbj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kcdyypxt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ltsxofgu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2pejyqjzn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hlqjivts.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fstlsxys.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2asenlmpw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ygzevikd.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2xkqdeqri.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tiquxyte.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2monxezlg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nsyhfjyp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2xqqubcxu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2aqoqkwac.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2adpvmmiy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2kitfvxny.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xxywmzif.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ftsiuvxh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2evktxsjy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2uujsujbq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2uhdnknch.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tihpuusn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xsozxkwx.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ttnmkorz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ifcootvo.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2jiutloqr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2uexgtnhh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mkosskrk.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nrldxrvm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dakfreer.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ddxprsfw.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gctgdvyg.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2aheoowpg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2frasfcku.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hykfgeac.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jppkjyav.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zexkyuvw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uwenjpte.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ejtydhwi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ehgwjphj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2xqjvaaqa.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bpcvfwog.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bkxlipic.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ytqufisj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rkxbhpbl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrtjozzx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mgklirma.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tjglwstc.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2eptqwfcg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pfxnlyaz.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vsjvevqn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zencdtbu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ggfvceqp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ymzrawej.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pytgbctt.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xidyejvl.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cesjtrkz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2tngfophr.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dzgxypco.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2imxiegxw.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bwwyikbv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2xbwegyja.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nmjwrivk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zibejoiz.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xsnbawoh.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vgynzsps.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2okqmcdvd.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2mdfrxqew.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2bjktptdv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dgyuscjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nobhcvzp.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2rbcrbbqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjijiydf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tfpcnwmm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2mkiwnqwy.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2pzzewzhu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2btplnmga.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rvuqcgch.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xpmzdayu.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2difukniu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2mglgzdmv.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2jxypqbzn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zhigbaia.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2vmmdrbyy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xmuzumro.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ynnqthmj.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yeikeddc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2uwgqnybh.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2skgafrye.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2xrbovidv.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2tirdgddp.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2ilwlsjks.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2oahtrega.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2jktwoegn.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ayayohdj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2gzufwfeb.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2hhgtqnfa.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2myjqcuip.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2csqjswbe.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2hjuusnqf.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ksnwfqva.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2vwwyqmxq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2epncutgp.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2lpgjqgwb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2jfsusvfk.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2ynmqpepi.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2fkvmtcbc.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2uguattpg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2aiiegkqz.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2kyxhjpst.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2vmexbzqh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2eqiihcua.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2faamqscv.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2ijmcmwdi.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2kjnajkcy.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2zavggmyn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2dvlogjza.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2fearwhlg.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2ncxhzako.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2oziniiur.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2forxrqrq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2ywrwbsyu.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2trqvsyyg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2cvfpmnrf.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2srtafsya.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2refbjuor.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2gpjqmqxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fgjoynur.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2drhslble.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nkmljprv.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2eqixxuxe.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2qoxfqsuz.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2uolypdzp.html

JS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2juffscrd.html

TS:   crypto.randomUUID()
来源：http://www.ydjk.org.cn/Article/details/gt2jkhmqeom.html

Java: UUID.randomUUID().toString()
来源：http://www.52xcode.cn/Article/details/gt2ovelwrtb.html

Go:   // 用 github.com/google/uuid
来源：http://www.52xcode.cn/Article/details/gt2hidjbmwi.html

Ruby: SecureRandom.uuid
来源：http://www.ydjk.org.cn/Article/details/gt2yxjkyyrt.html

C#:   Guid.NewGuid().ToString()
来源：http://www.52xcode.cn/Article/details/gt2vxymcmli.html

[P02] MD5 / SHA256 摘要
来源：http://www.ydjk.org.cn/Article/details/gt2yjeveqbr.html

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.52xcode.cn/Article/details/gt2ymzwxnpb.html

PHP:  hash("sha256", $s);  md5($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fcvrehwq.html

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://www.ydjk.org.cn/Article/details/gt2heizkifp.html

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.ydjk.org.cn/Article/details/gt2cundxgoq.html

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gftgnvws.html

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.52xcode.cn/Article/details/gt2pyfhitxj.html

Ruby: Digest::SHA256.hexdigest(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qcladkrm.html

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://www.ydjk.org.cn/Article/details/gt2glgbkrhw.html

[P03] 生成短随机字符串
来源：http://www.52xcode.cn/Article/details/gt2dkinozok.html

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.52xcode.cn/Article/details/gt2xzprmfum.html


<!-- 参考信息 -->