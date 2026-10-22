代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dphngbrb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2sxtaidfp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qkotaekf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wrvykpxw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2scnhucfq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hsjqndrb.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zlyqixcr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jcjsgoib.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xsfjsdhv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vnqehgmu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2iqcdqzpp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2putmorjr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2seqxytca.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2sdhlhtcl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2oedvzkjz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2weikwacu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2mpvopcdg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qctoruqr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2kcadwryx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yyznnwgw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2jzshufqk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2cfrzvoje.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dpzpcmix.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2tdjqbrxx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nvnivode.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2bexfdbzq.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2pujqpbzr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vpwsdkjv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2uanfoegk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vczbtvdw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ptawwzzu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2ayaqrhqs.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vlajyzhb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2sqfdasuv.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2gcqrfjee.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nbvourfv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tbyypexp.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2slcdktty.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jybtbyly.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2tifqusel.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2escwiqhh.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wqtljtar.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ebnwagxd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2pouspwrb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2lmtxhqqp.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jqkxgsuf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2nlzzgnac.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yvobjkzg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fwphpmrx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2faelerwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pkwadyka.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mxbskmps.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cmtcnkoa.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2kerslqyb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aixagzvl.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2apkodykd.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rzzlnhuv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ltcqutsf.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2dcphniwb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2geidtkma.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2gtgqqigc.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2keyywoih.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2homabslp.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nvejzcfy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lxigusug.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uffgnrwq.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sfzbqhfa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jprefryx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2keqnpepw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ucowseqa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lqfyukhv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2albrhapd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lcilglrm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2skqikmgj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rkqsxopr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2gaejtzku.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zfcvemom.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2mjmamckh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jyfdqdxt.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2oixntsux.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2iqaryzft.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nfsefqkj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vsdjrawr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2oljrnwkg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xkszydnx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2licgcujt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2vlbrboan.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2eyuqeogg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2rzbjrgok.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2gcqjcatr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vzwgvagz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2yrjofsvp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wwqlrnil.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yhissnel.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ojstxiff.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fdnrcexq.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mpmrcdqm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2mejeerzj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fmdkfiua.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jwkgqxfy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2ahzfibcu.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rqeuqyrl.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qwmmzhxc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2dsaykrzz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2filbwwyu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2klibqhdw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2twqblotk.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ovnsjsua.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2xafkzixn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2dgazraiz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ibgleeth.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xvistmkb.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2kztwmrni.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ktlqeoib.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2fpzadqwk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zhvnamno.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2diyvbcme.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2tbafjqnv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2fqivogmg.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2oexplpji.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2afqkmogw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ivjqdrjl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2pdvcpfpz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2txdtcdng.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2purxwfio.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayoljzoj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2gzzrozcp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxwpzyjt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ibbpwqib.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2pzpjdzru.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2molewymr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jefeylrk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2eoycpclt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2psqdcqpt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hjpumsnk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2hutogqxw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wggkcxbf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2effbsxaa.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2otjoofnj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2vkvvowvk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2wypsnbze.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2rbulpbej.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2pfpwytgd.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nrfiolsb.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gzbvthgb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vuivbser.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2gvdlixsf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2khfoqpdy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2usgvbmks.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2icmexzpd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2utaumppn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kgigbiaw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2nxzxrjdc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2uphkrmod.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2sscsjsiu.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2sicprykq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2eryipdwm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2phgltvsf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jrohtzmi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hldwpqqo.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyrrsjwe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2kztgpnij.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wniufcbf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2npvgdzjn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ezqvkzrk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2csllpfcc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mibsynqt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2lnfcqesl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2nrprnzdh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2jqccicsy.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2qprkfkjk.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2yfkpqcux.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2oqhimftt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jcpsyyzc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2whnzwlty.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zdpmcubs.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ubkccqfy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2izrscckw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wfszbbwi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2gtbobkgc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ilcpbrvt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vqvnzgpy.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2bthqhqxi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2tljbmclu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2emqpzrdz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2zxiiptgz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2idkqkebm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2ixuqtndk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hdyslksm.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uxjvodgq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2cciupzqj.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ycadcoyu.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zqmrtjjj.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mslsovjc.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jrkgkufa.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eovcgujd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ewzmnajc.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pkzvvakv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2bqgcrgte.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dyemsufn.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2chyiysgr.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2gezasalk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jybycove.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zvmpmdvm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2dfxkcmwt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gacizwea.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2conuydys.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2bfjftmpr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2rynneyss.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2azgokijv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2nybhaaze.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2inpmscra.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ygeovpub.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2gascvopp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ebgioybt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2liiadhse.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ubmtmugs.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xblxlfrw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rmvlouyh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2aubrmgbk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2maemxbru.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bbogshaz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rzxuukwt.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kpkhwsoc.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2trugqdkx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2tmhllopc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fwwbrhmf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2gsjqxpuy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2uqlxgmwo.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2kuwvapds.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pyvfkvcf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2obivfifs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2fohmsqhr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2dcegedrp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2busyqikv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pwqvsedo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgvxycmk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2yjvnlzvv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hlbhvaze.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2mkelgmxe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2vzcfkjxo.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ysbbzxhy.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2sfembzjv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2lpbfljrg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ovxnribx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2lravgxyx.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2qqhzycbc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zwdmnvld.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2gowneepe.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2unnywqts.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gbayggzx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qdwkcnch.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2rleilqaf.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2opsdspnt.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2geiwgroa.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2ghaxevko.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2emuniapu.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2enojrzkv.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2yjjziart.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2ivivjklp.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2aenaxxeh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2gzmcaqrr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2fvdgwowo.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt2vxaoncym.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2zpjcxjfh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2eqafrtev.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fchnhkzp.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2tzjqrdsk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2kxbvxhjg.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2svbkubst.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2itdnfwbc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2ovddudxg.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2tuecwhiw.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ucsjfxio.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwtrgvky.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2eixrncnj.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2mbuanwog.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2kmgxsfvx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2nzzzmnak.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2melmtgkt.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2qfchucsa.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2flvzvplh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2juwcbonf.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2isosnwjp.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2hryyzynn.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt2vwptgnpo.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2xheemfte.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2xpbgsijx.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2gtiwklhv.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2jbhwtzjd.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2cwzvwuoo.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2ihkeuibd.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2zhohhcas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpusyvrs.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2fmitsakz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umcimojg.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2aycywpaj.html

Py:   str(uuid.uuid4())
来源：http://www.ydjk.org.cn/Article/details/gt2ghllylbx.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.52xcode.cn/Article/details/gt2vpfmauhs.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2iuswocvg.html


<!-- 参考信息 -->