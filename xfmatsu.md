代发 wailian999

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gnxajewae.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gfbhlendd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gqckmoarp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/groapulub.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/ggxlfbmqi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.zdbjq.cn/Article/details/gbixspqfp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.hesvh.cn/Article/details/gzodwsyfy.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.fehbvm.com/Article/details/gezizleot.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gppgqatdc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/ggqufuamp.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gqfrpvrit.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gpkvjamlj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gfwwgdjcp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gxqcbuhfh.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gouocbhoj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gslvbhxih.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gwzoopdho.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gahyqnjqa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/glhjdjyzw.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/gbhyvdeko.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/ggzrmqdeo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gvusclsab.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/gwwlkqcgt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gxdcgwhow.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/ghowyyfte.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/gvznrfvdl.sHtML

[L05] 上传文件（multipart）
来源：http://3g.zdbjq.cn/Article/details/gftxwjgyr.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/giwiytwka.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gytbgsyor.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/guydvppkk.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gdootoica.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gmlusmrmi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gnlmqxnnh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gkpyxwrgi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gzcmtouuz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gldwarood.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/glsudrcgi.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gayxhldvl.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/giogkhvdy.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gdnwaoijo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gaobtxkoh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gqtacwmiq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gywnomyfy.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.hesvh.cn/Article/details/gofpkwqll.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/ggxsrirdq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gektfcaaz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gqofdknsi.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gczhrqamh.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gaskrbcvn.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/glqhffyzi.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gxhgtoljf.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/grtxokytp.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gqxjrysjh.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gxspdsjjw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gmucoyaxl.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.fehbvm.com/Article/details/goywajeev.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gcacqbbja.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gsimbawql.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.hesvh.cn/Article/details/glarryslu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.zdbjq.cn/Article/details/ggtndalep.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gdnhpjdsv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.hesvh.cn/Article/details/gwuzigwtw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gytjckgdl.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gugipqxfw.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gfjgdiouq.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/grhqxtahw.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gvbpcfyfs.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/ghuwgscnk.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/goxptftel.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/ghjqlljpp.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/giwxldrcv.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gbqglttgz.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gwvkgyimk.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gcbwlxomo.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/guaybtvuv.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gvhxyvgws.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gcavmaxju.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gngqguylg.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gywkwhwqb.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/gkaaksrju.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/ghktigjoj.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/gkmtatqrl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gtzdtmzyj.sHtML

[M03] 执行外部命令
来源：http://blog.fehbvm.com/Article/details/gcshadpqj.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.fehbvm.com/Article/details/gtejhsmfq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.zdbjq.cn/Article/details/gqalqbole.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/ginyvwiju.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gymzwynom.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gppsmcqfe.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.hesvh.cn/Article/details/gmbeugwia.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.hesvh.cn/Article/details/ghqeemhyi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/glkgiecxk.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gkzwjsdms.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/grtigsone.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gvrjnpyso.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gmthmrqyp.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gryghnfcn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gsthyfrfb.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/grokwcmse.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/golwdbxsa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gpkfaioce.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gzfrzopeb.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gjevmlzoy.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/gccapcyvk.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gtlpextbw.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gmzrvgioz.sHtML

Java: System.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gezpgyeju.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbiagsldp.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gtzyyoayq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gverqeaur.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/guozxubqm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/ggucksapl.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/ggkmxqobd.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gynzpzidl.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gcwbvnjbe.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gcqvuwnnt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gcewgalem.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gpzkpfezg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/grpsxvbvh.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gidqqzskj.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.hesvh.cn/Article/details/gomzweywc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.hesvh.cn/Article/details/goyuazuak.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gsggmfcab.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gcdaegzgs.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gcnjpttff.sHtML

Go:   func main()
来源：http://baike.hesvh.cn/Article/details/gbzoulukr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.hesvh.cn/Article/details/gipxpanzn.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gerwgvjgy.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gnxzfosyu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gyseyladd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gqaqqglsl.sHtML

JS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gzxrgrucj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gdeccldlk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.zdbjq.cn/Article/details/gcoffposw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.zdbjq.cn/Article/details/gvwbdnucb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gksezunnm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.hesvh.cn/Article/details/gwzdoycfx.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzceciizk.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gzsxjuqaw.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gpowmicci.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.hesvh.cn/Article/details/grmyjtrlo.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gllyucgze.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gxinthvjc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gqzolwcvf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ggqovvhrf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gbvecabbo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gtroqmltz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gkvpjxqqn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gczskgiwu.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.fehbvm.com/Article/details/gjmcopnok.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gcsasehqz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/ghpsarfqg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gxtzucwue.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gntrywfbi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gokoofffo.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gacbcmigp.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gnwmtabts.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gygwhyuem.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.hesvh.cn/Article/details/goaqckeng.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gfusakzoh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.hesvh.cn/Article/details/grwiiknhi.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gbuidmurs.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gkardpbuh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.hesvh.cn/Article/details/gusmqjqqi.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gwirmnhzi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/gsrjmbaao.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/gfrnltvhd.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gsfwkkpml.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gsrsfsgfo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.hesvh.cn/Article/details/grsjoadoi.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/ghxljgack.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ghldlbdei.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.hesvh.cn/Article/details/gizquekgr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.hesvh.cn/Article/details/gzahompcn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gfwqdskgl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gcoxjlnoi.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gdkdpjeib.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gcubqkpoh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.hesvh.cn/Article/details/ggheaihyd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gvsdehzmm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/goelonbze.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gcsfhluov.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.fehbvm.com/Article/details/gyuroqarx.sHtML

Ruby: a.gcd(b)
来源：http://blog.zdbjq.cn/Article/details/gxiavwhre.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gvdcbomxr.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gfbmnwrxq.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gwuplnukv.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gqpmzznfz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gixaroesu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gknwxsbdf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.zdbjq.cn/Article/details/govelflgv.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gcxcctcfd.sHtML

Ruby: s == s.reverse
来源：http://mobile.fehbvm.com/Article/details/gkjdgapni.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gpgrurvbh.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gzcvfnjkj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gdovhoqqk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gsccdlwqz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gcmtobqja.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gfepqmdbt.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gamblxrlz.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gororwahm.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gzjfpvima.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.zdbjq.cn/Article/details/ggalcgnyc.sHtML

[N08] 生成全排列
来源：http://www.m.share.hesvh.cn/Article/details/gpbghinrk.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gqgiljnxw.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/ghzbhoznz.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gfxfnhhzl.sHtML

TS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gduicjzye.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gznwakdpd.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/geqsxnmdu.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gjygbokhz.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gptvttovt.sHtML

[N09] 栈与队列
来源：http://blog.hesvh.cn/Article/details/gfivfetuo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/grjcoowvo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/glpnlmhgp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gnuznkbqk.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gvrqddpwx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gtffzpgdq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gwtgpxmjq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/graqijmyv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gjevwgttt.sHtML

[N10] 链表节点定义
来源：http://read.share.zdbjq.cn/Article/details/gkxszbeud.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gnytqdsfk.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gwfcrzymf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gonqaiwuc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/ghbcffcor.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.zdbjq.cn/Article/details/gmdhzfwnp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gqjpsxlku.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gudnyjcly.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.zdbjq.cn/Article/details/gayftxyta.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/gfbvrpxwl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.hesvh.cn/Article/details/gdgtsiund.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/gbzcgijql.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gpyfjnigr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fehbvm.com/Article/details/gmurgqxbf.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/gwpwkwjpj.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gnylosmnv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gyrwpcwdq.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/grcfmytbv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/grlychomt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gbxuyizjl.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/gcnefxqgn.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gyipqqurr.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.zdbjq.cn/Article/details/gimiyaemz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/grdykhyck.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/gewzjcggv.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.hesvh.cn/Article/details/gbcpvkzpw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/ghhptojtg.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gusfcauzz.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gdqnniotn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gncpwtuza.sHtML

[O01] 启动一个线程
来源：http://wap.zdbjq.cn/Article/details/gjdisfzjn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.hesvh.cn/Article/details/gdsjxhdvy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gymzudivu.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.zdbjq.cn/Article/details/gfpnuqmta.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/goztvnbbm.sHtML

Java: new Thread(() -> f()).start()
来源：http://baike.hesvh.cn/Article/details/gwsabodis.sHtML

Go:   go f()
来源：http://www.share.zdbjq.cn/Article/details/gkuitgxqw.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gosoavpqz.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gojhcrmlv.sHtML

[O02] 使用线程池
来源：http://wap.fehbvm.com/Article/details/gamfxrvac.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gsuxkcllg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.zdbjq.cn/Article/details/ghnhuyhif.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gchnwjphg.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gxbsslqyw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.fehbvm.com/Article/details/gkzshgixv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.zdbjq.cn/Article/details/gaemyjkun.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/ghzxgwrwa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.zdbjq.cn/Article/details/gpsfltqvd.sHtML

[O03] 加锁保护共享数据
来源：http://baike.hesvh.cn/Article/details/gantldmah.sHtML

Py:   with lock: shared += 1
来源：http://m.share.zdbjq.cn/Article/details/gywwewnzz.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.fehbvm.com/Article/details/gmqmxacda.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gxmbhahmy.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/givjzjxil.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.fehbvm.com/Article/details/gldjsvzyf.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.zdbjq.cn/Article/details/genjnmcas.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://3g.zdbjq.cn/Article/details/gkcyidurn.sHtML

C#:   lock (gate) { shared++; }
来源：http://wap.zdbjq.cn/Article/details/gqduioofq.sHtML

[O04] 定义异步函数并等待
来源：http://blog.fehbvm.com/Article/details/gqeunjtvf.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.zdbjq.cn/Article/details/gzuaybnmp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/grmcuodlu.sHtML

JS:   async function f() { await g(); }
来源：http://www.share.fehbvm.com/Article/details/gwbajinum.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/guvdchkdg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://baike.fehbvm.com/Article/details/gygoyifuo.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/gmmgwizry.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/gwerqiwxg.sHtML

C#:   async Task F() { await G(); }
来源：http://www.m.share.zdbjq.cn/Article/details/gisrrreci.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.zdbjq.cn/Article/details/gzsjungmm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/geilmnwqs.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://mobile.hesvh.cn/Article/details/ghhuuhhgv.sHtML

JS:   await Promise.all(tasks)
来源：http://3g.zdbjq.cn/Article/details/gfdpklujg.sHtML

TS:   await Promise.all(tasks)
来源：http://www.blog.hesvh.cn/Article/details/gnfgrpycm.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://wap.hesvh.cn/Article/details/gvafvuslo.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://blog.zdbjq.cn/Article/details/gcqzfdzry.sHtML

Ruby: threads.map(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gdbrommkf.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.m.share.hesvh.cn/Article/details/gvpnlrekq.sHtML

[O06] 使用进程池
来源：http://3g.zdbjq.cn/Article/details/gpgcagbek.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://3g.hesvh.cn/Article/details/gmjoayzhd.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://m.share.zdbjq.cn/Article/details/grvlavium.sHtML

JS:   // child_process / cluster 模块
来源：http://blog.hesvh.cn/Article/details/gxeqevzuf.sHtML


<!-- 参考信息 -->