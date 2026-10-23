代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3altnromw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3dnpuortw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3ibhcdide.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3cqlhdpzt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3wpxycctr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3wsvyzqfv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3jxmquvml.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3oceqgraz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dguxqhaq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3tjoqrtsl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ohzzhphx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vzyktttl.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3bjscymng.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3enqceane.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vzjburfn.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3tzjaxudk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hfqijrgk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yjljyewp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3xiexalfs.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ajwdeshi.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3opaftexi.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qnixvhfy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3lqfnvzdh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3kijcrdyy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3voxigilk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3soskfpsl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3iirbbryn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3bdlbhxcb.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3tunqcnta.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3gpcpceet.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3qiaplpjh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3dtpkphno.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3tktdsfhf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yfmqbqhd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3awbryeyp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3msnstwtq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3vjhvjaba.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fgpicigy.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gzxjpddw.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lvmxbfru.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3umtnwode.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ccbwwtnx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yfmygdrm.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3vetvxghv.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3jlmufcxr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ruywoaos.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3vxorojbr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3swzgeltk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ukvumjix.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uwqkovvb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3kytwhtos.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3owyshxvu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wefejnhw.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3mhioxjqi.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3fwuoiryp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3cehjdmdc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3tyohexcd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3kpqzbcxs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uogsyevt.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3xtdplchx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3izwxlbsa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ywwzpssc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xbrwwnuq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3dcbwimbb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3incujnug.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3hluwecvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kubxqzpi.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mlqykqpm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xepkbhiz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3zvdmfhvm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jaoiwvhf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3ozeyspbb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tkkxwszo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3anevewya.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3olrvjovq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jmkxucuk.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3vcktrgky.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3yfnsavtx.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3iadljdhg.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vkxhvkdi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3spaubaqc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ckvmwdrh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jsiczjye.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fmaqvpxo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fstxyjeu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3nmjgehrh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zsbxzvvo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3vewfkqvt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kgksqcug.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3dgemapuf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3skiqakun.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3paqnvqmx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3jxmoyhpb.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3jeozilpe.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3cihiwgoj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3afwoszce.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3fcmvveic.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3sgpnxvsb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mmtyfbja.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dutibhuj.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wlxjnwps.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kgauoeir.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3afuhtayw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ejwwbado.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3qfihkqts.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3jicdwmnu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wdkvrfut.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3swqamuoj.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ekdnczdh.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ecklbylp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nextmyxi.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kvwslhkx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3bznbkfma.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3tjyieuqv.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mvysdbbx.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3boztrpmz.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3teclenlt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rtuavvpg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wlahzaws.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3baszvlon.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3jiwziirk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3evyccnha.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3rqupbklu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3fmabjgxt.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3jwgiyibo.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3kdcbwihi.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3aaavtrjl.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3gqefdfcy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3rzwifudq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gfdritke.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ndpwjnxy.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ceszuikr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3ityuhnmr.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3afubumoz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3kdpfhlik.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3gtqmkjxl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3zpuoihqp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3hlyalszs.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3iwvmkyaq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3kkvuckyb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lyrrwxue.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hmtmolba.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3udfpluia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wmifeyub.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3pkuehqsx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbugosgy.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eltnhwmd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fqsjxwkb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3iludqngw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3deyexnuu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fgzaihcp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bzmwfgwl.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3suopfqwa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3pgknsqtz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oteuetoa.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kehmgpsd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3nsfkcazg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ychtjjvo.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3yyneyyqa.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ntiayqex.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3szdtgtgz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3lsvnhyuq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3vhnxtguo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3mipdtxoa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3kspkmcof.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3zerjsurg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mucykjht.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3adlpmfqy.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3eazvnpsi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ofkvufza.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3hbjutiug.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3vreznvik.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hapupwud.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3bynrdybr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bbcteihh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mbjshndc.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zscfgedx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3kkoamceh.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3zpdipjmt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ufzdqwjn.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3dpwftwph.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3luywzqcj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3yflmzkwd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pztlwzbg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nbqozxuz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3xoqcsgen.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3aumxvxlq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnyzzib.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbydgnwu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3issjqajj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ykenonie.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3pbvilqti.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wbpwuval.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rqznuozk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3zgwexavk.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3mdvldacn.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xbujthjp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3rahgkzjh.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3zdxxevcq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3ahuyuorz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3lyfffvzc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3fbbpfqla.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3bunrfklb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3rrnpsgbz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3xffahvjo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kmokryim.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3hhxcknki.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ihanbcdi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nsdbhmqw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3ecrpgnqn.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mgooynqq.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uubulnxr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fkkfrgvg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bjesscll.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3dpkqlnbm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hxtvxsmt.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3ufbxjzqi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ucyuzbhg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3luhbrgrw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ejznzzgr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ksfdicfw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ciubtutv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xupqlltr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ccoeeeam.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3rgbcvoeq.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ffvjfsww.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3glhusrvu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3uobiahaf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3royvltmx.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3dufzoslx.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvigxbcm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gqradonm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xmrjbjlb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zrnjvgnd.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aywbqvwo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ugykymph.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3nditurlj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3atoxqmpf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tfeyvfcd.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xcbsvcca.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ionwjewe.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3kmviyrkd.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3iaaarwec.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ezhrwsat.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fpsfhkkp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3canxqzdr.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ovinklnm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ngsmotlf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3botmzweh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3qltihtyv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3htkzeeyx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ugfxopaa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3adbtbpof.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nixtykka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3smfrfnap.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lhhthjmy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3negjqhqw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3aoamaxju.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3fhvfclgf.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3zkrpwjyt.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3ajfnjbrk.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3afcsyzyi.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3cbjkvrdp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3nioaqoic.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3vmuvlkwv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3bwxnglfn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3aowxzjoy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3opbwacsj.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hxoilkph.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3zxcclpyd.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3cydnhyax.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3ormcodyb.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3eqomjwjx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3qxprofak.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt3gkvgpica.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3cssqueiz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3epfglphi.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vnlatsdd.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3sfeyjpim.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3zkgpvvuh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3hmqdunvl.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3kaaukhll.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3jppsmlup.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3nuxmhqlx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3vrpxdrxf.html

JS:   async function f() { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3flggypah.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3gofnuhxj.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3fxssegtz.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3inykdcpu.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3sdznpbow.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3ggzkevtp.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3yqegdyfy.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rhtfemtm.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3vbzuxocm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ytxtqrpj.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3rdgxfwpm.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3kajvbrek.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3dvrejpjv.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3rhenzppt.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3cwnntdam.html


<!-- 参考信息 -->