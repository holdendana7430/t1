代发 wailian999

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gmbgfbwpn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gcywsgudi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gwvkegphr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gbswhucbj.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gclgkmknq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gwbnoruvk.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.fehbvm.com/Article/details/grblkjgnq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/goifpvetx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gqlizzscb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gzfmuewld.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/geydlyuiv.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/ghazhtmcx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gvaeuzqtt.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gvsayxqbr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gxwlcvrbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gfrrfnlxe.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/grxcqwaok.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/goegdjmdk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gaqdhxrff.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/gkgichozb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gapghliel.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gabokwfbn.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gngisulqg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/giyffravo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/ggtbayzox.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gveumgjwo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gicdevxrb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gwmftciiu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gikevfzfb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gzhiavlgm.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gvmutzgfs.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/geoydjrtv.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/ggagiuxgn.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/ggpdhrovu.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gjeaczasm.sHtML

TS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/ghjscsypz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gfstzeplx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gulgzilzb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fehbvm.com/Article/details/gmulrvylh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gryargquu.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gzjapguuw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.hesvh.cn/Article/details/gdcdsxtec.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/geizxonom.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gmmpbcmqq.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gzvynjulp.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/galnyfcxn.sHtML

Go:   resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/geqpodtkj.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gqjvededw.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gyhrrmtpi.sHtML

[L08] 并发请求多个地址
来源：http://m.share.hesvh.cn/Article/details/gmwcptsgv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gbovhrekv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gpkwtwrkh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gsaaptvta.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gtymolyzi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gwgkbpbjk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gbftgiqlo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/grhgznzjc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.fehbvm.com/Article/details/gizsmwxug.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gweccpmnp.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gdtgnojof.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/guchvfgni.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gcedsywgf.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gztchtkur.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gzvrcjsax.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/grzxuaqtu.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gigezotds.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gyniidcyw.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/glnnmohds.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gewqyhcem.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gkrsxycal.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gsxhexlyd.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gkraesdat.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.hesvh.cn/Article/details/gqqlvhbjo.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gkccghjwl.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/guhmzlfcc.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gyywkqhuy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gtiwtnqol.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.zdbjq.cn/Article/details/gclnthlyj.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gzrbklekc.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gndsnmljf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gmmbypbxx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gnhjiyiug.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gtqfgigqc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/ghxbxxlbp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/geubnlbvx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gnovvmzka.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.zdbjq.cn/Article/details/geuufkgzw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/gilurulaf.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/gsaeomigy.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gnadbexfs.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gobsxewbl.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gzvqqwzob.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gejdyryfc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gmrhitfiz.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gkdnouikk.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gjhjumsed.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gvfxdsmfi.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gjlzyjixb.sHtML

Py:   sys.exit(1)
来源：http://wap.hesvh.cn/Article/details/gkmspcjmc.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gzplorqoc.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/geqthznet.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/grwbmgmim.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gssqyoznv.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gypzarctw.sHtML

Ruby: exit 1
来源：http://m.share.zdbjq.cn/Article/details/gwqvivodp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.zdbjq.cn/Article/details/goddqbkhi.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/geigqiijb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gkpsjvemg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gwxjjqhwf.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gletsjxis.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gvduwbtyf.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gxevvldgj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/gtdylrqwm.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/gmjzmxdfv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gcijmpyag.sHtML

[M07] 判断是否为主入口
来源：http://read.share.zdbjq.cn/Article/details/gdlxflhwm.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gpdjpckem.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/grojvmpqn.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/grdgwehfg.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gogwwuuyt.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gyhmnefof.sHtML

Go:   func main()
来源：http://wap.zdbjq.cn/Article/details/ggbuijpqh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gsnkusfdv.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.hesvh.cn/Article/details/gmjlyczza.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.fehbvm.com/Article/details/grzwriaeb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gwpcdbaen.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/grdcxtqwi.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gkdwtviup.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gvpzwvraq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gsazojebp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.zdbjq.cn/Article/details/grcxkmswq.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.zdbjq.cn/Article/details/ggdtuqnqn.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.hesvh.cn/Article/details/geqasrzhh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gzphmprhq.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gozormbwm.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gpuaauvzq.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gmaqkdxjp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gewgpmuyc.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.fehbvm.com/Article/details/gjakuhtqn.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gllyivque.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gcjsesvhr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gphkhktgb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gbdxiesll.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gqionpkda.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/grurhhwad.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/garpukhqh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gsgcpqpyp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/gjreyqljq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gtachajqz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.zdbjq.cn/Article/details/gfyrqvthf.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/guivsnwao.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/ghtfurkoe.sHtML

Ruby: arr.sort
来源：http://baike.fehbvm.com/Article/details/gbicmxhff.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.zdbjq.cn/Article/details/gpwjlduhc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gfomoptme.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gicxrauzb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gshusyuur.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gqotrxves.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gqsapmtzk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gyznrtcmx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gugychnee.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gookwaceq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gdjjzwkzw.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gqvepfdzs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/grradyuwr.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gvplxrqwr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gaugbcgew.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gqfbeuccq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.zdbjq.cn/Article/details/grmmmrsfv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.hesvh.cn/Article/details/ggnqwcnrd.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gdjmyxmtn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gikhaqquq.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gcznmybak.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/grxjledxk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gedxqmlnq.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gexbkrsvn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gpbcdjybd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://blog.zdbjq.cn/Article/details/gxtdvudyp.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gazhxdkdb.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gapjgrkxs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gkspfidsl.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gdqedjanc.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gkhjnrtxd.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/gvgwfqpmn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gnwyjtasv.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/glshefsqi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gdmgieixt.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.zdbjq.cn/Article/details/gorrkufzb.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gmwcmytlx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/guuopefgk.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gcgmizabx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.fehbvm.com/Article/details/gwibfjmij.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.zdbjq.cn/Article/details/gjybemrqg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gtfcivvty.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/ggbbvsrkd.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/gmzbdzdja.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.zdbjq.cn/Article/details/gxzsalnyk.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gcultdhzo.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/grfgpswvo.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gotgeorch.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gmwxeyeae.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gkysquvck.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gjzrpmhlo.sHtML

TS:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gycpivdwc.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gbxgzgwxh.sHtML

Go:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gnjdsnrrq.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/grtxuyxef.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gzhozilvb.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gnhykorov.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gavmimmzr.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsonxezkr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gnqiwbszp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.fehbvm.com/Article/details/gxhxxoydg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gmzysoxpp.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.fehbvm.com/Article/details/gyzyaspka.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gwcdlubax.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/ggvbvzwlc.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ggjrlllnz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gentmdmmj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.hesvh.cn/Article/details/goaagjmhy.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/glpxeflyy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.fehbvm.com/Article/details/ggxqfyxss.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.hesvh.cn/Article/details/gihweimwa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.zdbjq.cn/Article/details/ghqzrfxsl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/glpbuhcue.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gydnbgepf.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvogxgpex.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/getdweofg.sHtML

PHP:  // 手写递归函数
来源：http://blog.fehbvm.com/Article/details/gxmjttcex.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gsybapwbo.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gxfydrepw.sHtML

Java: // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gknuoeubx.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gemklkakz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gmioqypuo.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/glgdpjqiz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.hesvh.cn/Article/details/gusdsugjy.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/grzabmygn.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.hesvh.cn/Article/details/gwmiwguba.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gbufvgnoh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gpnuzbavx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.fehbvm.com/Article/details/grguidacx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/gogccelrj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gfseugulf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gbpeatbbe.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gffhxeqvt.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/gavyzvrmw.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gotpmoisz.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gwpqreeqg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.fehbvm.com/Article/details/grsegcpqp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/gzvhxeyme.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gztbywqlj.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gwdubuhwy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gnlespozm.sHtML

Go:   go f()
来源：http://wap.hesvh.cn/Article/details/gwfncjkds.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gnhdgtuyf.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/ghsnbloum.sHtML

[O02] 使用线程池
来源：http://www.blog.zdbjq.cn/Article/details/gswnayzwk.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gmublcuyl.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.hesvh.cn/Article/details/gqaymrril.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gokpdtqpx.sHtML

TS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gzckgjoqx.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gpbilyceh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/ghplpwccj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/gkikveniq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.hesvh.cn/Article/details/gjytceegp.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/ggosonamk.sHtML

Py:   with lock: shared += 1
来源：http://wap.hesvh.cn/Article/details/grltdachi.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gnpkdmytp.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.fehbvm.com/Article/details/gwvtipbuh.sHtML

TS:   // 同 JS
来源：http://3g.hesvh.cn/Article/details/gwdmjmwvh.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gqieirgor.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.hesvh.cn/Article/details/guaizwnbe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.blog.fehbvm.com/Article/details/gjmcsqoox.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/grzwvjqgq.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gtjmlptgn.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.fehbvm.com/Article/details/gadnqgysg.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.zdbjq.cn/Article/details/gmxcksruo.sHtML

JS:   async function f() { await g(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcvuwmfsd.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gkndjajvm.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.blog.fehbvm.com/Article/details/gtsopkcig.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://3g.fehbvm.com/Article/details/gsrljkite.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://wap.hesvh.cn/Article/details/gsfmwfktu.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.fehbvm.com/Article/details/gjvpheupu.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gcfrfpmvl.sHtML

Py:   asyncio.gather(*tasks)
来源：http://read.share.hesvh.cn/Article/details/gutroxybh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.fehbvm.com/Article/details/gexhaallz.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.zdbjq.cn/Article/details/gacnqlrnt.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gyoopmwwt.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://baike.hesvh.cn/Article/details/gwpyojdkl.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.zdbjq.cn/Article/details/gefbggkws.sHtML

Ruby: threads.map(&:join)
来源：http://blog.hesvh.cn/Article/details/gzolyljkj.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://mobile.hesvh.cn/Article/details/glvskuklz.sHtML

[O06] 使用进程池
来源：http://m.share.fehbvm.com/Article/details/gyffarnnw.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://www.blog.hesvh.cn/Article/details/gdpuffmhz.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.hesvh.cn/Article/details/gdyvcxjpx.sHtML

JS:   // child_process / cluster 模块
来源：http://mobile.zdbjq.cn/Article/details/gtlhildxu.sHtML

TS:   // child_process / cluster 模块
来源：http://www.m.share.zdbjq.cn/Article/details/gmstagctt.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://www.share.hesvh.cn/Article/details/goyrsnikz.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://read.share.fehbvm.com/Article/details/geexnqhug.sHtML

Ruby: // fork 块
来源：http://wap.zdbjq.cn/Article/details/gzcylbpjx.sHtML


<!-- 参考信息 -->