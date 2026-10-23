代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3bhiajeqd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3otwgtuty.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3hloyzmbx.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ortwimxq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3jcpgfnni.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3azvaxnvk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ycjnurvr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3uqgnapon.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3jdwqelqg.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3yalnfwkv.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nlxmzpht.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3jsfpfvhg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3pfgamxci.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3yjmyzfyz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cfiswqpe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ohzvjzrj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3srdqneyl.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3fcuupcfm.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hrvrcjrn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3oqvoxyzr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ofkalinx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hgiuefuc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dalgempz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3wxxxdnkz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3ezxpvsap.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3wkfniggj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3gqtmyzap.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3gxdvobfn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3qyfhijsm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3hrqsttmv.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dssszfrb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3iovoclrx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3tkjkdcbw.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zducoajn.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ykelofih.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ijygxgsb.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fawtkfbi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tndwmnal.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bkgirvej.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yimrryrm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ftkyfhwm.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3juweqtio.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3hzgsqrmd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3czhjidaa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ynprgcaz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3euqumnvb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3bphbiibx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3rxagxgty.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3cwgydnor.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3xvhisccd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3rwmrtayy.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3eywfkhsy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ejxdxgqt.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cwhxblnr.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ekewitsd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3krljwgow.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dnpezuao.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3cgnqwott.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3lzaiiecr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3mtavyvmi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3fqvgphdh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3zjesrfmi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bdvxdxdl.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xwchakzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cjnqmafr.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3drlcqatn.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ejurgjau.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3htnprtkl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dnkdinee.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ogzjzkgf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3gqhruncs.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3amdxplsr.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3qnktirsa.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nwdbhvha.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ifftlaxe.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mmpkegkv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3ghxrviap.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kaogjelf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kjnerxfa.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tsuhglgv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pokuciil.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ifxauuqp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aolmazgi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3rhabvwbl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3vdqhdygb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3cfrktohs.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3akqpnyzl.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rjzufudq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3cqdxnelh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3rznyjptb.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3cfgxxhfl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ugrrpbex.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vpvlygin.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3bhxqavji.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3urwvxffh.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ldingbtx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3wvvzpoif.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sltzlmig.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3zzfemcaq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3akflhmej.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3ukxbpoey.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3kyygvcoe.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pbzdczsv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3izyiwrhm.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3izndniac.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nxahdvnh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovedfsdd.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zznsxuhb.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3uowcdfqu.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3gadjljvt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3olsnkmtj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ygwslmlh.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3nlqvknry.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zzowsryt.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dwqvfqhc.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3qinfmnge.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3zcuympqw.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rmhyzksr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3vjhsxbfi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3howvpgmp.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3muqzoevn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xvkioyzs.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bkpuarqi.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3slvsqbxh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3pimuutmv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3mihvbcpb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3gyiyqaak.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ujehxmiy.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jbzyywez.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lojrhqtx.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3vdcyyjzy.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3acmherdw.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3rzwimjpf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3jvwwpahu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3excmbmfo.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3nmlwksnj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3lavmpeqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3niziznao.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ehqwycfj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zqbtmdhe.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3puscsonu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bdlslsfa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3prexhvwg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3cisrrvxv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3bqwylnmz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cxbejeyg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzgglrak.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3afghgxuc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tjmbplpv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3olpjvlhl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ehxunwyg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3xroygjpa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3tiinsoou.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3dsxoiyhk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3phasrqgp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3antgbszf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rnilfhkz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nlyqnkjg.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mhyzkkuy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3yhgsnteq.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3tnbocpgb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fpmhgynn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jzjsicys.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3nddffzeg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3lwwohpep.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3sfrzunqt.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3gnvjjrls.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nygndocd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3rngwqxsm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vasubkzm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3wzlbdmlt.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oylcluqn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3uteitbim.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3rlebbccl.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3chjuyowl.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3anbqmykd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3wxiewspx.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3lbwgpcmf.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3vpoulcfo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3qortopht.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmvclbud.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3clbdpwxf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mxjicfik.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3pmnzbyef.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3mbuzppnv.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3udeywvdu.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3wspgzkdu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3kgccrltf.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zthvpfhz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rgrdxdsp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3sqtdsumh.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3zhshoxty.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3thefxgob.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lcktzkoe.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3olxvrlyt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3tjryimed.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3pyhrnbir.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ptetwshj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3pzigdgho.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3acyepctt.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3skrfdvus.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gypxukvm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3pbblvjfj.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3gmcaohhj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3dcfcpjkg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3shemuhtl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3gyxxjhei.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tfbbxbng.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nkdnlkph.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3czibdfmq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3habuittw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xooryinr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ejzsdqrc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3qhqiztwi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3pvhnihzi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sbwrmzcy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jcoaafxq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3yymoeldf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3agobveeh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tlmtybes.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zahfhthp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3eevstlzu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3zvwkcpex.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3wqrswigi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3kiyzyfna.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3ouammruy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3aulmxqof.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3btcgzzvc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3dbjolhmq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3dnmmeqep.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lkdrubjp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3kxzbqepk.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3cgbfghts.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3bukwjtpt.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3gpqfyxkt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bftkrvcf.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3igpdtwdw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3pwshlasi.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3lgpqkgiv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3jdhpmdhb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3evzzewxt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3mqxllevy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ylfwqzmw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ntrfufio.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3nlmylxwo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3cdpvufdv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3cbmdbekf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3rgsaecux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3devljxql.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3vluirhee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bdhrmmzb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3aejfanma.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ikuwibfl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fvclqxiv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zagzrdcc.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3qdesjjvh.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cwslqxvq.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3syidbawo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3sygvmhhx.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3mmxmhjva.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3yzsbnura.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ejnypyuw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3cwqgnjna.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3imjovmes.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3hmcmxdth.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3jjexnoar.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3hqzsmgas.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3nmptjqsr.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt3nndqucsa.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3uhpnkyab.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3uwnpcsgt.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3qpnrsfby.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3bkaysyzy.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3rrnnqcvn.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3yefouvmi.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3bbzziknh.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3mzkkzrqk.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3mjrtxuyg.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3xwmiixvi.html

Py:   async def f():⏎    await g()
来源：http://www.52xcode.cn/Article/details/gt3aoutrimk.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.52xcode.cn/Article/details/gt3wpytkslt.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ldxoechr.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3ehzzeiva.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3lmgnjpdf.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3qlvgugeg.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3hitzoats.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3mzxkwrpy.html

[O05] 并发执行并等待全部完成
来源：http://www.52xcode.cn/Article/details/gt3mbmmwfhj.html

Py:   asyncio.gather(*tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yglgahsb.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.52xcode.cn/Article/details/gt3uzkndmcm.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3ynedsqzw.html

TS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3kjibrmsk.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3khwvfsuw.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.ydjk.org.cn/Article/details/gt3mabfpkvh.html

Ruby: threads.map(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3mxjznixg.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.52xcode.cn/Article/details/gt3lsrzuzor.html

[O06] 使用进程池
来源：http://www.ydjk.org.cn/Article/details/gt3eleornnr.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.52xcode.cn/Article/details/gt3vywvfbce.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.ydjk.org.cn/Article/details/gt3uzowddlf.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3jmvlgncv.html


<!-- 参考信息 -->