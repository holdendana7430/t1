代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3qpwescrq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bvuobceu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3bpyvgdzj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ndesnvmf.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3lehjwdtr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wkvmfpii.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3giywkzck.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bwtomgbt.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ayeadczf.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3bnixibks.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3iwjoghsm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3hevkufjs.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3mrjdzvus.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3qflyqhas.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3vihspniu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3tickhgsd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3znryifdk.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3trknjids.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3kbjdqvng.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3obpyituv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3bqvqkmgb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3jwdpmxdm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3hcmwhrtz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3jlsmsnxv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3rwjimnkz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3kvcspyis.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ssdulgaw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3faqegcgf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzhgzmix.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xtetiryu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dnefnnec.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3mksmxitt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kwzzmkxv.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3justwzzb.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sveqdocx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3gpfhyjbq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3aaqrslii.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ahvhhedn.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rgbhzxaw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3wqulwbii.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bsdfnxep.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3vyxjqdkg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3hbxnirbk.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zkzsihrl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ovnvajll.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3cybgogrb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ndlrgdor.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3wtnbvyzr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3mipmkslk.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ktlizsiy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3ifdyiywy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3tkvapimn.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3umttmimy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qczsrwib.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3irlasksa.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3virnqjdk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3iopdnikp.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3fmihbmif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xxaztuii.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3uhcplyxa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3grkwkuqp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3rimbyckk.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kchfwvyz.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3nmwpttxt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3brszgkwv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dqpgbrze.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3nnvqluxg.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bbvjtsfy.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3fcppknen.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tbtilsyc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3tcvaamej.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qznvlykh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3drrziump.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3vyxzrluo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3yvnowayx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fozkliyy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qevbaesc.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3eyelxqki.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rxjohihc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3bbpsxhpd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3gpwzrhjm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3qyxdqkns.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eysvvyun.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3mgttluxx.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3jwblwciy.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dujisyyh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3arbkgytz.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3ggonloce.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3hltwklyl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3psmmpdrc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3xzgzjres.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zievphmv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3lvobwzkn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3lbpgytjk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oorpcqys.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3sokmxgbp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3eievavcq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3udbvkkmw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ntjrkmlk.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3qmimrsdg.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3sihzuxbv.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3velurtsr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxcvuguv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3enxwnjpb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3munjgcub.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3nbjmkrzf.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3kvrfefym.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3hpuwysaj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3yliajjeb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eljslvsq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wddwmkkk.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3ohqrdgdp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bipaaxlj.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3wflibvld.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3klhparwp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3pdjfhnir.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ymwgnlva.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wpjaxqtk.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3wlxgwsba.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3igsyoxbl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3qeoxrcpl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3osrpmtzc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3diutdmwa.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hidbnwdx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3hsxhxhrz.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3iulozuta.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3halqmskm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ggezeuds.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yogoualh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vvtqkjoq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3wibnnljh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3hdbkjqkl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3guiglxyh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3efxdyglz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3ljdicgto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3knyubfre.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3ibejrwpa.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lijfocea.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3efbdxzye.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3tzrpxajk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uuiwrfod.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ygdgjvyg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3xnjvjwsg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3ghlvmxgh.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cbiogtjt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3adwybuyo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ebeavbhg.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xubadddb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3jzgolskz.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3evqboubt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xivrkqms.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zszkhlnw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3hntldspd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ikkjkfgx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3hrzylkxr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3thhgwfkc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3eofdzgou.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jptmlrup.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3lioybdga.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3qaaklbvv.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pdsibbxo.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3fwjavztq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3scejfubl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3eakpttvv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pryyuneh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3wodidnnn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3iwvvnacp.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3axzpupzz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3pzmzxbzj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3dwpzaybo.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3clukzmci.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cpmxfqdz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3hjysrrqp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3eckbocjx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsjkspij.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ohazzobu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gowxpchl.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rvskvfbj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mqzydlsh.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3awvhljuv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3caukwzji.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3pjqltwdp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3uuvwlilo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3chxwecpa.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3rwhlkdvs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dwktsaxr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dajlhxly.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3izcdiyak.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nfvmcedl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xwlmqure.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rfwjirxh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3cvviejns.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3mfozqycb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ranujyel.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3nejwemss.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3ynlitqoj.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3rqapzkhn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3pmjeavej.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3grvgnvpy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3evedizom.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3oeoypbjr.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3vvilbrub.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3byiunigp.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hxtkwpyr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3ayyvfovv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3sseblejq.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jumwsypg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mbednmky.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3aqcehsro.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3mcdcimko.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3kyocgcuw.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vwkalpqh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ukktofiw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3bxxytyfv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3dpkrlgtg.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3yyahuggc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3fgvzemvb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3kjvodpsp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3npsjrnwp.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3cvrirzuv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ldycsfba.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3zupgajoj.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3xuokomzv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3uzrfabno.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3cwssywsw.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3xgdnavpi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3etuaeryd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3krzdtkzp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3pmbfztjf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3xkqviczh.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qhfsiumb.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3opclwiek.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fswnzuiu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3yeoxswzl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wuyrjllg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hsnbceks.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3qsngcuru.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3rvkzoikl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3kllqsicb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3dscceljj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3tbgwbppe.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3rkmertea.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uemqdpng.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3mlxjwnks.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cpferuwc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ymiaawsp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xggpwfwx.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3szuhzbhq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3gslcyewm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3svsjxnao.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3slfaphto.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3mmnqjrbp.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3eqxmgmat.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3nhnkgdqn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3zkpgevdq.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3xbkzmfgo.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kvwdicax.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qxarxhbs.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3snvmuxez.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iewlzvfo.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zdnamulu.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3pclwnlyg.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3buiuucly.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3grtbpkue.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3kzjskmdr.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt3cwwxchab.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3omslaavo.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt3aligyzuz.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.52xcode.cn/Article/details/gt3lkgpgtsr.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3dnrxrlmu.html

Java: synchronized (this) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3xigqalkk.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3onludiki.html

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.52xcode.cn/Article/details/gt3mpmdvvgf.html

C#:   lock (gate) { shared++; }
来源：http://www.ydjk.org.cn/Article/details/gt3dqsffnur.html

[O04] 定义异步函数并等待
来源：http://www.52xcode.cn/Article/details/gt3wbtclkht.html

Py:   async def f():⏎    await g()
来源：http://www.ydjk.org.cn/Article/details/gt3qughwjzx.html

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.ydjk.org.cn/Article/details/gt3smcthhnn.html

JS:   async function f() { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3vcocgqdj.html

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.52xcode.cn/Article/details/gt3jvsoqeis.html

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.ydjk.org.cn/Article/details/gt3zifqqauo.html

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.52xcode.cn/Article/details/gt3ffdcyrbp.html

Ruby: # 用 Fiber 或 async gem
来源：http://www.52xcode.cn/Article/details/gt3thqxztfl.html

C#:   async Task F() { await G(); }
来源：http://www.52xcode.cn/Article/details/gt3tvhojbxf.html

[O05] 并发执行并等待全部完成
来源：http://www.ydjk.org.cn/Article/details/gt3zqnwmovi.html

Py:   asyncio.gather(*tasks)
来源：http://www.52xcode.cn/Article/details/gt3lhhhvful.html

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.ydjk.org.cn/Article/details/gt3dwdgitrp.html

JS:   await Promise.all(tasks)
来源：http://www.ydjk.org.cn/Article/details/gt3yguhyeku.html

TS:   await Promise.all(tasks)
来源：http://www.52xcode.cn/Article/details/gt3iifaumnb.html

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.ydjk.org.cn/Article/details/gt3fpskwvdr.html

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.52xcode.cn/Article/details/gt3wwxbzmzr.html

Ruby: threads.map(&:join)
来源：http://www.52xcode.cn/Article/details/gt3jbiwhsxw.html

C#:   await Task.WhenAll(t1, t2)
来源：http://www.ydjk.org.cn/Article/details/gt3lzdasyuf.html

[O06] 使用进程池
来源：http://www.52xcode.cn/Article/details/gt3brxcghsl.html

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.ydjk.org.cn/Article/details/gt3uiwctyrw.html

PHP:  // pcntl_fork 或多进程队列
来源：http://www.52xcode.cn/Article/details/gt3fanjbzte.html

JS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3cqrrksop.html

TS:   // child_process / cluster 模块
来源：http://www.52xcode.cn/Article/details/gt3busptcmz.html

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.52xcode.cn/Article/details/gt3gqoitqtw.html

Go:   // goroutine 已占用多核，直接并发即可
来源：http://www.ydjk.org.cn/Article/details/gt3iejswrgk.html

Ruby: // fork 块
来源：http://www.52xcode.cn/Article/details/gt3muzpbzay.html


<!-- 参考信息 -->