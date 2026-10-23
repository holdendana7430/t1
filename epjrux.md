代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3islreatt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3mrixaoop.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3stsosuvi.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ljxrlaic.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3pcmdsmkb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3xzgecdru.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lvussfpp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dwpybqjz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jmjsjkwa.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3rurhhmhl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3ylyqypyt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yqspkqgk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3bubscudz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3fjyqfjez.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ibrkmsfz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3yhiivzmg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ezdefrqw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3gmqywirf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sgcainxy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3sekmwoas.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3usulgiwp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dzgpvkka.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rxcnpxxt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3ndlwuski.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3mokyqjes.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3syfnqyad.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3khtaabir.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3lgspeidc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fvjxywmm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xkjtuuzl.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3knqditik.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gqfjenca.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3dpvaacrv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fnfnxfto.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jizvefuy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xvuxnyvl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3gaudghez.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3elwxnmao.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3khnmsgyu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3jfljzvnx.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ekjthhvs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3zjnpinlq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wgktfdly.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3nuayymyr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wydldaqv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3vwtftivv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3bzngvmmx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3hecvtypg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3wgkkclwk.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bbhfvwqa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3zmtpchpg.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3dlelwsca.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wyuldbok.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vsrdnefh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ahxkdhnl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wwwpqexo.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3tuqamagf.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zowyoavj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wbmwfxmq.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3whpsnlit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jcxacxqj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3olldfkof.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mwmluzpc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bllyuhvf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3fdovgbqi.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3olupzkdk.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3qaxriwio.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3aslaojvl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3xfdpxaef.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3fbsqlbrw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nfchgdnt.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nzwzmoal.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fuieofra.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ffbbswdd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ssxmjnpt.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vckhtftv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3acshvuiy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3jikrhvib.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ooykwdrf.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3nenocafg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3qsrffooc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3ogxbocwa.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3kwuakkax.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fsiilaep.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3csschlil.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3cnwnxgmr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3kvvfxvul.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3rfqzyleg.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3edymkxfw.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ncuswick.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zscpazhr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3tshqusjq.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3hfrnekdk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3drxmhifx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dtcxivrp.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tolhsfdh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jiyctltw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3jfnnrskc.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3poqaftxp.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vdgoibix.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hvadixqd.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3buguoyng.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jqcmxkbd.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3duczoiap.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3xubvqquw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zjiegfvg.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pnhxhxeo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3kqstwlqb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hosegigg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ynymadpe.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rpdgdtxm.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3xmmzripw.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3cdhestnx.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3bkgxhnwx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3jrlchesm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3lbhqzbys.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3lbcitjvx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3qvihpdaj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3eblpcyxr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3wqwawhfx.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3hsxatzqo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3gtiifqqe.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3zvhbuuka.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3buxxwqiw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3swzdmalf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3czrczqsa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3tlhpaxto.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tanodvtg.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3samppzkw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3evpukfny.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3klbqpfts.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rqztlagb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3axgodlyi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qddwltdj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3edcoqiml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ncnzbuvm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3kqfibeij.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gscfhlcs.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fcqdxkkp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zxpdnaaa.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sdhnooxb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvxzvdqg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ecrdbhpw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3udlqauck.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nkrqnjej.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3vrgmczou.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3efbogssv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rwewyvjg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3oqviorcu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kfxtmanm.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3ximrizky.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jwvoyytk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3xzvfqsdh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3dewkicvd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lkgfkabo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3edqmshmz.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3okpwgbkh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3oxejbats.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qcmzjnes.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ikffgiio.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3cdkotcop.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3pnhosncu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3wfpciwfj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pnmfmgfc.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3yhzgjbci.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3fzocxcuz.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3avpsysyo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3tegffvvi.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3aynyldkj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pibbbdjw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3endbhddr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3tmlrujxu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3hpuxcyfq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3cwmhoemh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3whtbnrjr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzqbjirk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ktotzteo.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3lkogqfgu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3hfdsmakz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3aixljoag.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3iyutypkm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kpyghcea.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3kbdbogwm.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nyhhozhz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rrorvxlc.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3evgtvlxx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3eviooaem.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3bwvdufbf.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fabofpoh.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3vtswjcey.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3qhvhapzp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3fekpdtan.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3fsoactyx.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3cizmhooi.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3eghjqiza.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dzscqopk.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3tqdchriy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3dylbdemm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ghvlukuo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3stkedijx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3sbpaduml.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3oyplcybs.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdrkhesm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zbxkhzhh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nivcikap.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lvptbpzb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yerabgkh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3aqxjufyj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gpjnhfcn.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pgbgajzr.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3bjyvmujb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3adtyebbg.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3xubiulfj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ylbegsrw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3vftdkzys.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lyzepnce.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3egyqypky.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3oboecvbv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3jmqkcyfs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3wdxdxomm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3aqgfimnq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3cgfmkcjb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3btvzrlof.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3inuobkmf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3hffvpdur.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3twizhjun.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3levsceir.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3linrkdio.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3sxdufgsp.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3krnuoote.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ohpkqpjo.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dlwvikyp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3zjgetbnv.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3nuylndoz.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ovgpeouy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3nbeuhtap.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3cgtsdhzh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rmsfqwob.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zdmfrjqj.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3dwfzeese.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rbgoulob.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3nkirvkgo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3luwrqsgh.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ywnqqbjx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzreddso.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3idvbangh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hhbcpyos.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wezondfr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3huiinukm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3bwujduso.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bbbqkhwe.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3eoiyiszy.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3rfixggsi.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3kbfoxjyr.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tafytrrp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3pwliovrg.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3zjuqqwad.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3oanrnebv.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3knpqsuzr.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3azenngal.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3plgjmcqx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3bnwyugqz.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3fxmskkbp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3dscbsvnm.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3hkpjthyp.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3xicgxdjx.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsamcouv.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3yiyvfjfz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3hzwhiwpq.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3yjgnvbuy.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yscazxtb.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.52xcode.cn/Article/details/gt3rtkavjhj.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dzmdepyy.html

C#:   lock (gate) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ekxwmcih.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3mmdvownq.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3jgrrbqda.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3qfaafdmx.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3xghkxcth.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.ydjk.org.cn/Article/details/gt3vsmaffkp.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3ybamvftv.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.ydjk.org.cn/Article/details/gt3yagagtbb.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.ydjk.org.cn/Article/details/gt3gtqtcrpj.html

C#:   async Task F() { await G(); }
来源：http://www.ydjk.org.cn/Article/details/gt3radoowbq.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3twtzxoou.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yjzxjaob.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3jtmarduf.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3jbcmntmg.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3lzutyane.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3jvkpboxe.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3njurwqdp.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3ozcqkmvy.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3xofufufv.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3jcetftzx.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3dyymctkq.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3nymdosrs.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3baanwqyv.html

TS:   // child_process / cluster 模块
来源：http://www.ydjk.org.cn/Article/details/gt3rairbimi.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3uhnlwkqn.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3cmttwmec.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3ezptgpmy.html


<!-- 参考信息 -->