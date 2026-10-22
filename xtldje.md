代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2fqddmcgw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2wpudhvne.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2csxsyyen.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2bnojwbie.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2hkhiloek.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2gxfiqwqf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sswusqtf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lnbqjxbf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2iefwwtjh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zevgtzdo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ptdowocs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2upfwjfpn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cmcywutx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2camcianc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mfpfelij.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2zywqbrus.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vgwftlbx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ekatxooj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2vgzlrznj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2pefmccqr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2gtkkqzfp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2njjflwtb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ymrjblue.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2exbscuos.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2uiwzwwxl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2wxwyahcb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ecylygca.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yfynazto.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wjevkawf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2iqvnbdor.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2frcrpgdd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2rsveodij.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2eopzgnyr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2tqvowtpd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tkcrcbxa.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vjsscvxp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2fwalvciq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2lkvutlje.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zlkqtxkn.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ugnchvdx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2nzrcjisj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ydpfairw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2uzffsahm.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fsebqmgn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ehzxugrt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2hwoqxpmm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2dyovbnvh.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dcvlsoiv.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dmwsybuc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mhigeyok.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nsnakkyf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2dcefcxkj.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2tixnedjn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jlwiglen.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2okuirihq.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ozrwagza.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2erintcdu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zlnvheaf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2etlqbgca.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lgughhfb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pyxcpuml.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ugqrtoes.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2suvpbaju.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qsagjxju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyqphcuh.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vjrcwipi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ahoegnjx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wwcmdylh.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2dpukzqdk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tmxylawp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nphrrisf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ksrzxcwy.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2imnernlo.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2luqtaczs.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2uizwgfku.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qrbckvym.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2vhticzud.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yfntwanu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rxjudfyy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2psohlcrc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hygbldqz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ohwlfbul.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2afufaibc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2fpjupwix.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2gytizala.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cfcuxgun.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2svfhwjzp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qnqqixmr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2wmeshfjo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2vwijpkka.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2idgamkbu.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qfuobfhr.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wzcocbus.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xrbhcpwa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2axjvdyyo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fnjimpkj.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dtmtxgpw.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2izdvbmqw.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uujfuvzm.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2xmweqarq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ydkxojoq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2zxxcxpgm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vqqeakuf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2znnmptda.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wukqqkfq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hkioymqb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cpivmoub.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kiqcszde.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qswehbjl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dzsvzkmh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lbofgjbd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2jwwhmvxh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2keuskwtb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gllyyyxd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bujylsed.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2wfrdlrvv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2uwnkkeer.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2telzookp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wavpkvts.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2kvtvbtap.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gwfnnphg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2aspeyihr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2tbcvaanr.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2kgzczolu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2minzkskk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2urxzmnly.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2mbtbwchs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dcsklchs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2fahwzkxf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cdubtzkx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2rdgwyknk.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ezkkxltk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kgkqsxye.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qmjcqvoz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ppvsyqmx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ozcknxxh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2vsbfahmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjolzsjn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2dgqqvdtr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kurdxkud.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ygwmblwj.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2krgihpxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2plreilzp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2wluagwfw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2baoaxfqb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uxoxuoib.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gkqdjzls.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dmvlrltg.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rgueskhu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ehrqafda.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wemkkfsd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xbfstpzl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tdjikpxm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2kzzuiimd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2adholopg.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mlhlqpjj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2xbxvtsrh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2guzumrfp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2dhqyljyy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2nofbmusv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2nvdnrtxd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ccjwxike.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2hklidken.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ydkrzqip.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rphnnxrc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tbfclrzh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zaysnlse.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hksfrncl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nfbpgmuo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2npaxlfwz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2wqwnsmjx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aqnturku.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yyelirku.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ybsjhdrp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2osixtkud.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nyafvbwx.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2icmumilb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2knwofoaa.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ukcnnwlm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcufqifl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2softaewu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ybvxwrdi.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lnnysvhi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2wjwnykgc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ccivqycw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cviwfyrn.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cuvdovlf.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kvgqcntw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ibwfjczj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kfgaalnz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ehikcotl.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2xtodtsmz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2gyvmrhnz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ikrapiuv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2mkstjlfy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bafwwuan.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2npgzyvxn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2mrasfzzj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zzghjvtr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2lmrfgwqz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2xvifpddm.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2rvqennpv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tloyftvy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tybyamph.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2kaxxlxna.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2zywwfrmn.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fwhpowzp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fvujaeqp.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bqebwlkp.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hzqdgmxm.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ckwnmekb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qeybwrek.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2rpdukhva.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdsgwfwt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ikceupad.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qurthzkb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pvrlnkzz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cegfqtmb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2krnmvhol.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rqwegeko.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wrlyvgya.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2qwktaxxc.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2rusydwvv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pckjxagz.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ugabmmlz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ocxplbrf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dcnhdzsu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ekoitqkc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2vkbqvdfn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2vjbygpol.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ylxtayvu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2aifounwb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ftyfehrs.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xjysqbjs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ghwzpkve.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2zwbkcmlv.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xpxntckr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2kicbdgrt.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ztnxtbgy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2nojpksda.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ktcluanb.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wlnldyqb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2sxrgvhzs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2sfaoozcz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2jmflydac.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2kvbqhokc.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2eqknyngw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wpotcjvy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2snvdetot.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zgorjbhu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ocodphiy.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2dqhojqxp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2holhcslg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2aemtxnsr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2nltfnxor.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2eepgvead.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2pnbrpqnx.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2nzgejcuz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2xcxnyqqc.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2zhkocdkk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2ygrzxcfs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2yushuglt.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2lsdnziec.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2tzcffwhg.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2dnkalraa.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2nwyeyszj.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gfymcqkn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2uycxcdik.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2amdxeevf.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2frlxfxus.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2omarqdch.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2hejrzjgu.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt2krijybfj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2hkhkgdpe.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2vukkpgcd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2tutczwrt.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt2jblwgrpp.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt2ubwdiztp.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mobfoncb.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2giqefyvh.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2tqnsihec.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2ftkftztg.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt2fqucqcnd.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt2zrfxqvwq.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt2yztuigpu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hkpvpekg.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2wunykhsa.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt2ijjvijvu.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt2sjoaeluo.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt2eammmhxs.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2fnjaurav.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2tkbknvgc.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt2nwfucwio.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2iihlhecj.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zhccrslv.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt2yndgjwiy.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt2jftybfat.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2mouipucw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2wndirgko.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2fzvwehju.html


<!-- 参考信息 -->