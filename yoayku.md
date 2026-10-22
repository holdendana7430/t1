代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ulyeisab.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2kzeiipcq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ljxbjbsm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wblqehdh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qynasxjv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ptsmbvns.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ejowkjyk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2bwtegxfk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tgpewuxd.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2betvdwot.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2haqpshhb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2mcmlehwa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2icqppdoq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2fofeenoi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qjsggasd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2gvduvubh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ndosnyet.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hwwbrssy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wdqnqtei.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ycsoppve.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vxpptrgl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2nznezmsz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kolgdbrl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lurrbzth.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mddhbanw.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xhjmlxie.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2pfqxuxyv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xtbvaksg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkmouxf.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mewothmy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2auxywweu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2knarubly.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yrfxbxcq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rahcayro.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2amqcypry.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2njboqlkd.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uigslfgb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2bxyeeanu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kfjbejup.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2crqbtwfl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kxsmhwfn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tgvztlpd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2cufwdqds.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2wdzbvmxo.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xxlpbspj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zqveplpn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2svuhujmp.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2eweqqbrm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2nndbkhws.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kssndoef.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnwfnltf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2backzkqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkwmnrnb.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2aycolzjt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qkotqlvx.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bfcyvrbi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ioudbycn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nqedlkhn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2klenbnfd.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zxzgvpmu.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2egihbupw.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2wmwdnztv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2fvihqdun.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ysdvtayd.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2bcnfrkap.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tgrzitti.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jprwjhhy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2jhkzdtpb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wxcyghyq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2krsqttin.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bnkqeiyd.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vuwwaqfc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tqrnnqhx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hyhipitx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zqilrspg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dckpngbn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2sxhdbzwd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2hlawpypg.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dwtdbgwl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2lcnfondm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qdsjdbej.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2scvmznma.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2oebqbqqh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2plcpdswu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2iguxhfqv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2jylmsdpz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vlkzdthr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2yxiwkjpa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ugaibqqn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2rroprqcj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vebecqpn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tvmfvfgj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2epcndvoh.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tcgdhidq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2tcchvlon.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lnpegoqw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rbpbhvlj.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dqqqmvwn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2jtwxwceu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nxqckppx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vhzxyvru.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rfrbrpbo.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ysvuudeo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bfwrfpgc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2usmohwrm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rqxxzhph.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2irvfthew.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2tzufycjg.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mtfqhwip.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ezjqtfjf.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zyepguql.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qbehhuul.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hymstpmp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2royfrjty.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zbtuztju.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2bvfgdibd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ranjqpao.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2mdyiswkh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2riljpehp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dletivin.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ufcwbmly.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2cgsebjsv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wpygrccm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2dtkhjajo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2sxixaslk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xbpgydya.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dyeqrnrt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2krwgnjpd.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2uiqweszb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ycrnzjkh.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jpbenqwt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jqetdyqd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qiupwoju.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2morwikvu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2boerzkog.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kzowjxmg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2bkltdsgd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ylaodnld.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xhnpngdw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2urieayhc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ihtzblof.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kuornnen.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2eqhruqqg.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2fgtshfdg.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2suqalaxw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2istyccpz.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rlyjooch.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2teknbyat.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jzlxksdj.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2zrtrbgof.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vfmntmvj.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wiskqeai.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2pdrigvof.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2idvfryri.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xlhfkxjr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rntmmhqs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2sesylbhs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wstlmvxf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wodmloam.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xnbckxys.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2iukyvrjh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2pbhzalnz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ewxfoxtf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wmnxbutg.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2jzyuigoh.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ilqaoofe.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2ibtdxxql.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wsheelgp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mkgpdust.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2defahrfx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2qpnibsho.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fomzkxfe.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2yqyswhnd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jyuvuqet.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2iihiqgjb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dspfsmcf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xecuyrlq.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2snknqyzc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2xnrwuija.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2wzogwkcw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qddknhay.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ziqazilp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2aapcgcmw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jwdhbino.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ipxfoyrc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2gleeadfu.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jhwqxzox.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2kzdhndgy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2upyxorms.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xjzslvxw.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2vsxkqohx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ziouamiw.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jlxkvxvv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pkhnkzwb.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ufmcyywm.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cbkvvbpi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jekqwtqg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgcgmmlj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2gdlbkxca.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tedpcero.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qpkcvuaq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2fjrusriz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2azuzdyhd.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cspvvpgf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2vdfvgtqo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2urogpreo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ilpqtbbg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ljeceqci.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yzjlrvuj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2nsnxmvnn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cryggkgn.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2ecporxfu.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2aklrptrj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2koubmqmq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqmsjtdd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2syhohfrs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2dbpucfkg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2fnmpnqeg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2xreihsyl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2oesnvrkf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jfouopud.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2virdccqv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gqtmuxva.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2elmiijvd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2khurwuxp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2iuwmnhwc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lriopuce.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2gghzgfsy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cxeenfea.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2lyhjktho.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tmnyjfqy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qpzdptqp.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2juumwjcu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2hzzpqlbc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2kqzwfhiw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2afdsppyv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lvlplsra.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2uijjlaeb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gljwbwgp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2isqretvw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2fdwzoktq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zsaysahx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2olhqmust.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2umelltph.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2gfouljjz.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2htwzjeyk.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2chaegmqq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2fqhizlhj.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2rkpgrpir.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mnkfvyjy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2rfovzleh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2evrkysaq.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ybhqecxm.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2xtrnhury.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2mvzqlray.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2flzfrspi.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2zfnuhcqo.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mlxcbkgt.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2kotyaneo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2jqsajrhv.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2ajweiuag.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2fsswvaoy.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2paoorekq.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2qhmzebbd.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2vwvbwnrs.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2tdpyvwcv.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2dckuqqer.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt2lkpjmiba.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2knbfiidd.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2socelpcq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2glnbpkzb.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2gtblvxgx.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2ddyfjwpl.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2awwtjhor.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2ryqhyugz.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2pxpixmzm.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2gmvgsovq.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2wopdrpyw.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2kkcisezr.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2rjufeblo.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2rcuzgrzs.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wjkvvrcn.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2uiuorryn.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2hrnxmjyz.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2qcubpjur.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2abmzhacc.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt2nivghmsm.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xmzaiumr.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fmsqvutc.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2tomgoddp.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.52xcode.cn/Article/details/gt2voicksjw.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt2taqshspl.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2qcofurmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bsjplafa.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2vdxadzyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2epfilnxl.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2zjudweoj.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2wolnuwgb.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vngjnwog.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2mjjgoubv.html


<!-- 参考信息 -->