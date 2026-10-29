代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.zdbjq.cn/Article/details/gakybwenr.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gaqgqfmfp.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gukzyhaaz.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gcoezgxwo.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gigrgpznw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gsdmivuqr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gsrwgpgzs.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gxgslxhna.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/gfwkznuay.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/getfvekvw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gnmwbkwus.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gzihgizci.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gboudxgbc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.zdbjq.cn/Article/details/gxebxckqr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gnkpywzhn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gnxvuudam.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gtezvpsit.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gtlqozqdm.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gaawbfylw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gyuglxwpc.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gifgwzyzl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.zdbjq.cn/Article/details/glitonzje.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gscuyuemr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/grjfpagqh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gmrmnmfys.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/guflpangz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gffrnsulg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gamzjtodl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gfzqiqhut.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gojstpdiy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gkhlrtzce.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gnrqliapu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gtixsfrkb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/geqkovckl.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/ggtukahdp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gzbhwdfnr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/gzjedislv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ghgtzplpi.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gggohlpnr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gbaibmqjd.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gynuoaobn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/gpovnvrkc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gkydfomze.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gygkqtusj.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gniufjguh.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/grspedaiq.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/glqzsuxbo.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gbyfvxoyq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/ggcptgibv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gbhqpirat.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gzaionghk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gpeftqguj.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/guuytlena.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gbykvxpfm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gmvmyatbu.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/ghqecyaul.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/ghyovsrqt.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gosuglbgw.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gpmaswydl.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gujjhjwwu.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gnqhevppj.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gbnyaxtrs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gefufwpua.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.hesvh.cn/Article/details/gncxlbqta.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gsrpsikss.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/ghiagsdie.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gstgxjkst.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/grrggexer.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.zdbjq.cn/Article/details/ghairorvk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.zdbjq.cn/Article/details/gmpedmuhb.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcadcpiyf.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gnloniyzz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gotgqnwya.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gkgubfwpx.sHtML

Py:   sys.argv[1:]
来源：http://read.share.hesvh.cn/Article/details/gtrsnlzsn.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gpdjxsaze.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/ghllqyaqe.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gpvbdlptf.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gubqxkldr.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gkaisvhmr.sHtML

Ruby: ARGV
来源：http://m.share.fehbvm.com/Article/details/gnrjmixfx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gowtnrhsu.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gapnmexch.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmyadywcr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gkmyrivnw.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gwnrqvoyi.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gskiqnfwr.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/goyqpucyq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gujiiuszo.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gcyrkoddo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.fehbvm.com/Article/details/gcyyllmie.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/geouvkixt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/godtecaok.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gtfmgacgx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/ggzbjzpgc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvgfxumqo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gnybdcjrt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/grkbvxmsy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.hesvh.cn/Article/details/gbksdbjfv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gkreaafiw.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/glpmcseme.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gcujugfyu.sHtML

PHP:  getcwd();
来源：http://m.share.hesvh.cn/Article/details/gyrnljauo.sHtML

JS:   process.cwd()
来源：http://3g.hesvh.cn/Article/details/garouwgwe.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gvinaklcb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gihpmgefx.sHtML

Go:   os.Getwd()
来源：http://blog.fehbvm.com/Article/details/grjzcfmsf.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.zdbjq.cn/Article/details/gstvyprwf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/guemmrade.sHtML

[M05] 设置退出码
来源：http://baike.fehbvm.com/Article/details/gerpolgbu.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gyhnobpds.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/gedufllsq.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gvpwgfifj.sHtML

TS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gpktfjtnb.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gnzpclkmu.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gcgwxahdl.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/grayyqvck.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gaepxgbim.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gqqufuuux.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/grreirmsj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gvuleepjx.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gerpoaito.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gnyqtgety.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gyrjahtfk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gmzmvonld.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gmoramqyq.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/ghxrnkxbc.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gdhyayvtp.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gdtzxgosm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gyywmyvvu.sHtML

JS:   require.main === module
来源：http://www.blog.fehbvm.com/Article/details/gblygtcgr.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/ggxjvlizb.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gswlesaok.sHtML

Go:   func main()
来源：http://blog.fehbvm.com/Article/details/gnqxfmfve.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/ghdinpdlp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gaozdbjer.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/gzccrwpbn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.zdbjq.cn/Article/details/gdudioipr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/guchnmctr.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gjlxczhov.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/ghwpaorfi.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gtdudbbbo.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gwirvkzjs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gvylxebyw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gwkbxwooe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gftfyoolw.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gnjfqngmk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gbhcuuwsh.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gynksdmij.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gffyamrtp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/gogxpbpek.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gjzkpujfc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/ghfnoidot.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvvjmxfit.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gdffjnwmd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gseenmdrv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggqcfxasv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/gbdtbkkhq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/gbvpvjizj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gngqyaxux.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gmfyhhwxb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gkctavulz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/grfnkpqvb.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/gkojghibd.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gkyswjwor.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/ghtsuppkb.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gkaiunvmu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.fehbvm.com/Article/details/gasmroinu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gbphgoemt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gshcfoxrl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gxaxqiruc.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/grvoagpro.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gzsmqyfyd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gyxsdrtau.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gdzyxpecp.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gxzqmbgst.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gkdvtsvtm.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gncybrjva.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gqtrqcdwk.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gudadzgbi.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gifsfnbla.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gccnlimvl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ggmrgcelx.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gyxncuika.sHtML

[N05] 最大公约数
来源：http://wap.zdbjq.cn/Article/details/gfbscwxys.sHtML

Py:   math.gcd(a, b)
来源：http://wap.hesvh.cn/Article/details/gqdqbhifz.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gpfbuudjw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gsuyweozk.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/ggrstytwi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/ghgyjbxyi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.hesvh.cn/Article/details/gndtgijru.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gwbhtoccy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gvndplxtf.sHtML

[N06] 判断回文字符串
来源：http://mobile.hesvh.cn/Article/details/gcuhagcgv.sHtML

Py:   s == s[::-1]
来源：http://3g.fehbvm.com/Article/details/gbbveaetu.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gifdbhbfg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzqjzvnic.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gnejxkbsn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gnlnecmfl.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.zdbjq.cn/Article/details/gckhokwcw.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gzmondnpw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gesschqqb.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.zdbjq.cn/Article/details/gusujuqsw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.fehbvm.com/Article/details/gtneuirbs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gpczamnvf.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gjtwzamww.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gsrbzbwew.sHtML

Java: // 手写 HashMap
来源：http://baike.fehbvm.com/Article/details/gdiljjapp.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/ghgopnbce.sHtML

Ruby: // 手写 Hash
来源：http://www.share.fehbvm.com/Article/details/gszlxdgxt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.hesvh.cn/Article/details/gqljzselj.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/ggruvauqs.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gwhqhlkeh.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gualhudym.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gllcsrhjb.sHtML

TS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gqyvqspdw.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gqrexrkzg.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gzjoiuctk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gpvzdheft.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gvnazfhrv.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gxaqpqrlb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gajjddwwe.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gikaenqrh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/gyoybrbqi.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gkhremicu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.hesvh.cn/Article/details/gapfyurpa.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gxcruugoy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gocsvtsra.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gyufaaimf.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/giszznvsw.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.fehbvm.com/Article/details/gdlhbqpua.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/gidwfvgcf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/ggrodvmpc.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gpsjzciwi.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gctmkjzdr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.zdbjq.cn/Article/details/gaqlnegbh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gluqetmxa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gladavpcp.sHtML

[N11] 二叉树中序遍历
来源：http://baike.fehbvm.com/Article/details/gemspnnye.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.fehbvm.com/Article/details/gkuazegtq.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gcsfxlkwb.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gaycxjpgf.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gcvidacvi.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gfplzzbvh.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gvurqimne.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gzqyrjelx.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gajdfuzkq.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gekffdjmc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gbkemhtuj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fehbvm.com/Article/details/godqahkco.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gdvdrlecm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/glsqrxcit.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gprwkhswe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gzjyqnsen.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/goltquahj.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gnafvbbee.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvtpdgjak.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gdpeytczp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyoboetcc.sHtML

[O01] 启动一个线程
来源：http://mobile.hesvh.cn/Article/details/gmbbiqwih.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.hesvh.cn/Article/details/gjsyzlcmd.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://read.share.fehbvm.com/Article/details/giavvxjmi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://m.share.zdbjq.cn/Article/details/giezuxqmy.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gjthwysjo.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.hesvh.cn/Article/details/gixqgmynf.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gdhzlphxm.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gfdrpugqt.sHtML

C#:   Task.Run(() => F());
来源：http://www.blog.hesvh.cn/Article/details/grpusdjsv.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/gzaaqucgn.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gsbdswzdr.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.m.share.zdbjq.cn/Article/details/gicskpxod.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gamxucssv.sHtML

TS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gjrzqqbwd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gxeehlfhu.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.hesvh.cn/Article/details/gkccndwxs.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://read.share.hesvh.cn/Article/details/gdalkyzpk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.m.share.zdbjq.cn/Article/details/ggcjefids.sHtML

[O03] 加锁保护共享数据
来源：http://m.share.fehbvm.com/Article/details/gmwxeusdm.sHtML

Py:   with lock: shared += 1
来源：http://www.share.fehbvm.com/Article/details/gcxhiqvgl.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.hesvh.cn/Article/details/gessaxiyo.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/ghtnafuja.sHtML

TS:   // 同 JS
来源：http://m.share.fehbvm.com/Article/details/gsbjcmswh.sHtML

Java: synchronized (this) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gbiymiixc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/ghlsytkmg.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.zdbjq.cn/Article/details/geuagypyi.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.zdbjq.cn/Article/details/gmcvkipzc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.fehbvm.com/Article/details/gdmusthao.sHtML

Py:   async def f():⏎    await g()
来源：http://read.share.zdbjq.cn/Article/details/gapjptsfx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.hesvh.cn/Article/details/gbidaxkzt.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gukvagjih.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.fehbvm.com/Article/details/gfduqytpg.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/guwnzkdxx.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.blog.zdbjq.cn/Article/details/gsattoqbq.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://blog.hesvh.cn/Article/details/glhftxayz.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/glssfalxi.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/ghshcziwi.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fehbvm.com/Article/details/gqsgxsmgp.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.zdbjq.cn/Article/details/gpfixspvz.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gzlsbmszv.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gbzezyrjv.sHtML


<!-- 参考信息 -->