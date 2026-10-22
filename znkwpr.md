代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rktmhnfd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2wljffmlc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2pvpsjlrr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sxyuicmb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2nzzkvmxa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2aamcndap.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jmgexsea.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vebhinjk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2alwfrwqx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2swckepvt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rwjnyfec.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2sjqzonsa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gdwamlxc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mxvebpfz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2opobngws.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ojdfpahh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2drvliubv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gcifrghl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2fqoceogj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bszdebak.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2skfxgbom.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wvidarlz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mgzwemtp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2rdnnxeov.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2zragcpwc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2tmnmtreh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2yckxyuwk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2tbyxyvir.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2eoldxzrz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2modiczxm.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ybnemawr.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2ehmyekap.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjyltina.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xnvnwndz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qxdcsjgu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2psakfexm.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2eozduefv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2kkelpcwi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2roktzwyv.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2axgftbtm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2yyzjsxka.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2vvyclddw.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2bamvgptl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2twplhlko.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rwxsusge.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2igaagnmm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2higodctf.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nmbtjslj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2hqiggbxk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2piuxfmyz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2behjpzop.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2smkvmgtw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dwvpycqu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2iqmymvaj.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2crwmzdko.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2njbuakcf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yqmvgznz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2fsqlupxi.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jpfdozjz.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2rplgupfa.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2aurkipmq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jryadmtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mjobvxaq.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2axbgwttc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtxwyhum.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bggwjjdt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2lgtzcyyi.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ifsqvear.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uudryktb.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2kgfopnjv.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cwaorezr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qmqobbfk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2cepswvqc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2igrdtoah.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pxmiewhg.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qevqlxet.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wbjqyvvh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2proflxof.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dpjbjagd.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hxzwaryb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jafsmmiw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2orzmexwn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2eezmntlx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2uhmynpep.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ylenqvyu.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2ezynnhyf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yaigmqxn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2afwsowmu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dfiijknd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2klogfqlj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2denuryhh.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2titwhgze.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2xsjszsbv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jomgwavi.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xcjzlntx.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xgsyblof.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eatpitbt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2fdgfwaph.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ewkggpii.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2bhhpecoz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ebsldlds.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2ptgekbmc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wsxcnsjf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2jufglngw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ouuxspwf.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qdnucngw.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wqyotwsb.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2edhzhxgo.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2nsfzaane.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2xnfepzhc.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2fqwglchm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wiwctzdr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vfidpwlq.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mameybwt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2lizbnzbq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ifapkege.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2jhnfljjh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2unwlazuo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2adkhzgzp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2puaknpiv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tmluysrv.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2sqliwhqd.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2gilorynv.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lxnueipy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qyxonnfh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2osthvvcc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jkfttqpo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2gxsmxkog.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2qoqxteup.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2kompcyrv.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2zarujjgz.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dqkshnhw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kadimvow.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ueoklmxu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nkzllzxw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jemziptf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ollpxzuh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2junqndos.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2avxijjgs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thrirplk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hbmhpjkm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2feywmqwv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2fxtioynq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jwvgmyay.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2txbxdlyz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hiavuiec.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cnxdkcdw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yykkqhma.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pdmugops.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xjckvcwc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gssjhvii.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2aanrovjl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zaypmsrv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ntmgeoes.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nuwojlfy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qnqhqpdd.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2razrcmdu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ofgmrkfa.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2wlkkuwsg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2yxvzxxii.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rxxetlto.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jyyngrka.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fctwwtzu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zsnekjlf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zskvvvfe.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2xkehlava.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2esxcuqzq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2bjavktim.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2fipqkdnb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjdbcuwu.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qdhsbrbo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rpxzmdcn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ggqecjvr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2ykzdhmcr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nflcxjhv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vstxffju.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2eprgrluq.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2lomeafjc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2iyywefii.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2yetmpojf.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2rdslbwge.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2pihonyru.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2oxzjutqo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2uwohpbmw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gymwhwzk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2arvzxunl.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kjcsytwm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bjwcntqg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bueojjlh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2janlvuuv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2uaituwmt.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ztchnneb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sltyaxyz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ejkybqtg.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2fctzfros.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2oimjiilp.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2mscwrqtn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wcfeyoge.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2zwllhryq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2seuieyfa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2glonsvot.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2fxcxtyos.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2eysfzhnk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2whclisqq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bobaopar.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wsfbonsp.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2frmbdmsu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ybahxhvl.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2joqktogi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mzcbdezf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2dsokmpmw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ymzaqtes.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2foqjznag.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2evvttucu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kjifxoye.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nthrgbxr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xmpatrer.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2onuljiey.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2oumwzbuc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jqnmdiys.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2costkpld.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2itqtykct.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2nkarzvuv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gdjveafj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oehhiveu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jwcwzojv.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2tvjnrcvt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2udmizewi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2tsxsflkd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2ektziima.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qolmewvt.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xfkepjtw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mzfxpfml.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2mzhsedvd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qzlleifn.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hforzldu.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qvwzaznq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2lsesfrzl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iaokoylr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2roblinbx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2psnupftf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fpsmccms.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2hchpcprb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2jljqmnge.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cewwwhur.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2nwdyoogn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hqjlhdwc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2nlumuhek.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xewxiiza.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sovythdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2drzmblzx.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2sbdlpdgj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2zgxxlkaf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2jaluxquc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2gohlgply.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bhffwvtc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2muqnvvef.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2ltouekwn.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2qfvkjklp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2nbilsrhu.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xobkjbjr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2bqgfprqb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2mhybaxdl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2atrggjiq.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2sqvqxhtc.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hdqefudf.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2xcgusppj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2mvgoyptx.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2uhoiumnq.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt2abkzeoey.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt2ayygkdbp.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2obvtfhag.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt2kaketdse.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2sttkdmsa.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2oblbqqwb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt2ofdyejae.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2nfihdlkl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlugoytk.html

[O04] 定义异步函数并等待
来源：http://www.ydjk.org.cn/Article/details/gt2mndbmuma.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt2hkwrfqcy.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt2jaruylcn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2zirhuzdq.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt2undfbppg.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.52xcode.cn/Article/details/gt2adpbeezp.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt2qhlrszrt.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt2hyjlyqtk.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt2uoqlzepy.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt2bkesgnee.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2rhvctkmz.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt2uauahlpn.html

JS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt2vioovqpd.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt2apgboanf.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.52xcode.cn/Article/details/gt2vaqlurbx.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt2wpfjtnpu.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2mllyrprl.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt2loqkgddd.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt2ofblsgqp.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt2rilankxd.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt2zinpiugl.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt2xuldvlxr.html


<!-- 参考信息 -->