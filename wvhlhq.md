代发 wailian999

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2qchkdwco.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2desfuetj.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hgvftemh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hpeflmrf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2glrjpdjb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2wnplryip.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2muoviwzk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2vcrzexze.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vjvqarup.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2feqvxqcn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ewfwnfkm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2qaermuks.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2tyaqdkce.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2ttlufmod.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ntnnvoud.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kozjcupa.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zgttfiii.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2titadcqf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2qwodiwjc.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2xlohhiit.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gnhrcesg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2zdchevkf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oztxafyj.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xmcnmwjv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2oirhraxc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pzniqqmp.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2suupdrxi.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fngcnbfc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2zgyiacoj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tpckngsr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2skdqdknu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cgnyxzhp.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fjansxec.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2puquqpor.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2radkcgqv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zscpqjvs.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2coeyztal.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2fsgfvchi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2gjvcmbwz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2hkrlhkyt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2qohkohed.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2xunhcrox.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2uhalbfut.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2srmvhwfg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2llrkjkoj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2rmtnscgj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2tkntxzcz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rnugqzvp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2jlogsxlr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ohasmlou.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phgsraml.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2axlicdjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qywqtiqi.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2tkjhzrcq.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2qwsrbwdd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2aeavihow.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gaoyypfs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2caefprac.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xxjrktnr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2knkjuoeg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2rydwfnrp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fzpxbozw.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2jgfzutdv.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ceawzabi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2iefcjbfg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ekpqvcmt.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2eabmcbpg.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dqxctpfa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2donvhdfx.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2twivbruk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qyhhadfs.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2ysqfncqw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2oigfqixy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ffhnvspo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xhdwzhkv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aslghutm.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2phheqmjo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2zeesvtkw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2hlhurdff.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2shdmezyf.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2bnjzmerm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2msvjtvgf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2woyhxwbf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wizjhpff.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dzkhciik.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nattjcem.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ahsjjilu.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2tvdphakk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2inweqjpi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2ohncxess.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2imiifqiu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2owspsihs.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ohiaqzhr.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zgiwinlt.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ahfmvdqn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jgfnopaa.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2eoctmmge.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2akwlhjpe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2pnppvipu.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2tlqwutzp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2brcpxqxo.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2umlqsqwu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ywlmfsno.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2krvpwfqk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lxyrgbhx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2uercevqw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2zddkgjdw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2nattrltz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ascsxzfw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2snzbcael.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ofxodehy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mkzyypon.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2eikxpqyc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2rqztbarr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2rvlmazcv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mtqxyyck.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kkgdqvox.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lcawwqur.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ueaovofo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pbnaxbmu.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2scxtqizs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ucykzmmv.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2dngoxhtd.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nrnsydqr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2sfbuefds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ddkqlakt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ywqgihon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mrrpjbdv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fhdytaat.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dhglupmq.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2aztxiydf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ynpycqrh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ujbjdfst.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zmblpcqx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oahnvnrg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2aykcsplj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2fyitugeh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hbryfjfi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qiebeijs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sgxvrzmx.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ndzjbnpb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xrdudekw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2utoncida.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fhiolbyv.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hqrduhdb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2dhpmlces.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2krtbfclf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2eablgenn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2mltghndm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jersstpp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yhneopnz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pyhjdvxt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ohxzgcme.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ymkiyayc.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ufexqroc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2egajvmyp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uebqpbir.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zygjqzqu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ztablhvq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mnrxnssf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kdtxpqxc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2agqdllln.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fxpywqsq.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iwtzhlle.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2nvxwbrtw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sznmdhky.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2khwsneur.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydckbiri.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wrytkqpd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2rgbgosrb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2lzwtbzsc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zscbeotj.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dmghdlud.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2jobhfrsh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dztxrkgu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mdatipln.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2upnltvnf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2deuhodmh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ohyjxhgw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2cjpwzldo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2klltnozc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2epruyxru.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zeyrxrqx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pdkemkxm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xhkxtvaj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vdlxcnhq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dluirxyj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xdvvyufe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2nztfnsdb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2uuaxypwj.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xupetokx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wkjdevch.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahifqcxu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2dtmxlfyx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zaqwgwyv.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yarjxdev.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dkfchtke.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzvshxpv.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2fogtxwkj.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nptajtrb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2libcarjm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kphdisdn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jqqihgqs.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2phyaguvi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2vitknfvz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yxjxmaqw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vlyfmeqe.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dlwwowgz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2glpzumio.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hmcchacs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2secidezw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fqkkwsjj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2egcinnua.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nneweoal.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dntyobng.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ijnjmxcg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2qgizwlhr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qshfgwgo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2lhqsaken.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2khnsodhn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ixyjdmiu.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tyittnil.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2zzbexrxy.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dbyidscc.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2luzgedpj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2yeakyjfl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mjgdduxn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2sqcjlhlu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2frtgivms.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2zwspsldn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mnwjggrz.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sxkzjaew.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2snrsukie.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2idvvybug.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mbdhejep.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nqajgiau.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfbmzsex.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2umpbsupi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wvnqbkry.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2phfvlyrj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2hwxfmznq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2njshjjpw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2tjubfbhl.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ztfsvnyf.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2hpmmvejm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2rcgjaqvo.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2tiegxufe.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ahkbqovf.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2zcnjmllg.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2mzpohczz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2dzoktixn.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2yymmbrso.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2whqdwxsa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2jrrgzxqn.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2eanypahd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2ydxrsdgm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2thuxfkqb.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2gmvjpzuv.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2jiucuotk.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2gfrbturu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2zrdnbvkw.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jjnubxyr.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2lhuytpzi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2vmcqugwx.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2xirdbrbw.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2gnayqcga.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt2ousqmjfu.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2laampbiq.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2wgmqatoh.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2fssajapr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2lfsmikro.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2cpfmqgww.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2uvbjricb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt2ajuvkbfs.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2vdhpwyar.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2azrcfdil.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2yiprbevw.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2bvqpsfwx.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2lpnbjahx.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fxyqcbar.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2dlbmzhxt.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt2pmqcbukh.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wkhjaxjt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2qyweqbwr.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2bwjinnag.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2olwxlgcj.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2cpnesnqa.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2isnztavj.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt2fnyylxjb.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt2exiabinr.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt2wdpbeodz.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt2yvqbqpvv.html

C#:   Parallel.For
来源：http://www.ydjk.org.cn/Article/details/gt2epjvrewo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uiscufhu.html

P. 常用工具函数
来源：http://www.ydjk.org.cn/Article/details/gt2kshztjyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmofzmmx.html

[P01] 生成 UUID
来源：http://www.52xcode.cn/Article/details/gt2nsrtxfbk.html

Py:   str(uuid.uuid4())
来源：http://www.52xcode.cn/Article/details/gt2jmxegtgs.html

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://www.ydjk.org.cn/Article/details/gt2oodxqxdh.html

JS:   crypto.randomUUID()
来源：http://www.52xcode.cn/Article/details/gt2bfcmwwav.html


<!-- 参考信息 -->