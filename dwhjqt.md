代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3pxgbxcwx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bwblvumh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zqdhzoqf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3abztneav.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pixeyrii.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ovodbyjs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ywbqfltv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jkeysnxl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bippsxgu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3hdebogno.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3mxgygflw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3dyvamvbv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gbssvanu.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3nahaodlx.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3lhpnthnk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yvetzllv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3npmxiwfw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dkhqsgmj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3fuuqgtwb.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3agxlakju.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3viuvpuql.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3bpvkcltq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3uvaazczc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3czvahkzp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3wikqglkn.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dlpcaxqn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dwdxjrts.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zdcpomme.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmptnfin.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3upvqhqnj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zyvqmqpo.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3prpnrvpq.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dhxlibti.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3rxdqnkiv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uitnbpoo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hspmcvqb.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3nejklani.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fslmgwug.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3blytdoud.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3owpbjlzc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3clenfbzl.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uhdagqed.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3hehpbpmu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dmvqwter.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3otcivjzn.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cfaybblj.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mhancnak.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cvlnemkr.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cafkrnua.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3rrqnotpe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3krckobyd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3fwlemfgv.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vatibbnj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3xvwptozt.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3erbifzva.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3yrevsnoc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3oebbttio.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tcsesdqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3naothhmc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zqgfpiva.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hlxzlogx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3lesoxjzn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ochkwpal.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jqousybi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wmfpbhdu.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3puqllhxl.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3oqusakvv.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hhjzusev.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3jdyjtibi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hywhkkyh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gbapkxht.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3puagggdu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qdnwpujr.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ujtdpkhi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vsitkjxe.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pexqhxev.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xhokvgcr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3xeamqwcv.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3alyzshtk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3sxpinurk.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3zyerfupa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mqyfxhdi.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3xqjroagp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3wrkhoubq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3hbwojlza.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3kottzhjw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3lewqwyuk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3egwpdlls.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3fmyloxfv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3jlnkpung.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3ycqrdiwl.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3onjykwxq.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oojsgvll.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xdlyrlth.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bomumwzj.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3lpmkmftb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cspmnogs.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3csyzsozm.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghfutkcv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ayjnirfw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mfxqilrn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3pgxatojn.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3flqmlpxv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3boqwoukd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vmhchbgs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3qydjxxgv.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3sgcbawjm.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3kybarfkm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3sywgpqyz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3pxsqatur.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fmjzlsye.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3yqdjqpng.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3putsxlzf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3fqikedkh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3auhfymam.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3khdbulxd.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3lkywbkhs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3huwvhonz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3upgfruhs.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3tdjbfnvw.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3axxvlwdj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3jayqkhvu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ziqureum.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3nwvjsxch.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3frplwomm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3yjsedzit.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3nfwlerhs.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3gtmtusbt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ixmhojgi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3lytloxti.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3himhygip.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3fjwgarxs.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3rgycpqqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rdmztvgx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xvqkzcay.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ccuhisdy.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3dttlijbs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sovvtlzr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vybrcytj.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jsnxspwp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3munaysnf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wcpubrfr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bncsrckn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3zotrxakh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iotmlbks.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3tqifderx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3elyctvuk.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pxhycrxc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wibecngk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dmilmuao.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3edovffbi.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3taowwcst.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3anwaesnu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3covdflrv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3rghvmicg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3nupjbwbw.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3qlnfcmtz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fvpowwpa.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mhcdelwq.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mnxcsjuu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3dqsploqa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3csxwpdhp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3osrkxbjw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ntusodxm.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3czkbrckk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3lsacyezp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3igzjpggx.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bexmrzmf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cekkuepr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3eqxmrktm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3oxojaqiz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xgmlcgcm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fhvhjzjv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ozmozpxz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3qkbeezct.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3rowfxmir.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3phxgzsjm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3yqopvamp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3iqktpumn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3minqlnmc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3cnxvijbt.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gnmluvhw.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3goyksjfw.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qlqqjvtb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vxskqlpe.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mqxevsvz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3nloumwfv.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3bvsqeeih.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qzbdrcam.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dbziedyd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3vtjdcgjw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3abprpplw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3tmifrvig.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3emvvazcx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3xfndoyft.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3cputvhkq.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3liexhklp.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3btmaqwrn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3etyokhre.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3liygarya.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zhkaowwk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3cfffvwld.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3cqntaqbn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qiuktfeg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3yatmlyxi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vwzkcreu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3fvmuonlm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eyraqkww.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zujnghdz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mfayhjbn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3ieyftsbh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3hpksntaw.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3gcxqpnay.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dmkkbqco.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uhqtiarc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nogxflpl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3hejcjwfv.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yuuyacvb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3vxgvifjw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3dnmvlngn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aroepyaj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pdvsyidp.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3giuqivsa.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gznnxlmu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hnwgdwvd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3oknfmukw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3yoeupocc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3kavlglhm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ebtxtdaf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3uzlxktir.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3hycbeoxp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wfcrroek.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ncfpszsy.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ywiaisfr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3pwfvwdsk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3oejcckdy.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fizdyexc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ccbtwaoq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3cbjrvsgq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3hmylnrkh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xwmkrxpw.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3mpjrntpa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xcuatxpq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tbtsytvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bmuhfioj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3twnradsj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hucivvdo.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3vwcffsuv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zxtbskkf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fvulijcd.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3lfbieukm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3tiszjosz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qnwzdipg.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3ipikxbge.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qlkyijju.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ruefborp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3otieirhr.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3epltuyyz.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3fxyfuacf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3tuaftxsr.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3xlvkrdbx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ayjpriae.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3ficvqhli.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3doveyxpa.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3vehtlqga.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3iwvftxkl.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3oprsecni.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3pkveksfw.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3wprxcpwo.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3omyfpicm.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3lgbrdkhh.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3kszxjkrp.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3fdggsngh.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3fjiqehxd.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3rbznlrva.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3xfkaerpi.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3xocetwei.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3wrzgnhsb.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3zynuiqtc.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3tchsulnh.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3skqzsyue.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3ouzgnbpe.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3fffrvpda.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3acjjijrs.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3vlcgrljh.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3hjipfhaw.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3thkoliyh.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3uwmccpsh.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3dwowlqen.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mztowzkg.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3anwhxygr.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3jasdtjvu.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3nnzpuauf.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3mgfgysxm.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3pfbnpelq.html

JS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3hcyewtxc.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3nhixiwcg.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3fckerobw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3qjyxhgis.html

Ruby: // fork 块
来源：http://www.ydjk.org.cn/Article/details/gt3rtsyjenl.html


<!-- 参考信息 -->