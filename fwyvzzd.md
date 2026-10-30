代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/ghjmnebfq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ggqvlrhda.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/ggtzdowtr.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gpinvzhli.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gcsulgalm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gezbjtuio.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gdktyrqym.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gtefvmdza.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gykkegwql.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gcbkqwdyx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gpumitkkd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gitdwmtwk.sHtML

[L03] 设置自定义请求头
来源：http://www.share.zdbjq.cn/Article/details/gmxweqavk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gwzjczecj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/ggmsjutbd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gzoittubu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gmndfvdds.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gqiopipah.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gcemkjzzk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gdouiqvrb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/goxkfzxrl.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gedqrmacg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gqfrloxhp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.fehbvm.com/Article/details/gimevkwfs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gzsrbtpcp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gwewzevrj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/guwzlnoaj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gyolgdtww.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/ghaikoqtt.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gmokvixem.sHtML

[L05] 上传文件（multipart）
来源：http://3g.hesvh.cn/Article/details/gxupdnjro.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gvwxxmecq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.hesvh.cn/Article/details/gkvsxuake.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gwddaminc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/guawecnib.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/gahwpiphl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.fehbvm.com/Article/details/ggzprnjyx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gdwbcysyh.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fehbvm.com/Article/details/gvcvofcvx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gftubgdcs.sHtML

Py:   resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/greamhlpx.sHtML

PHP:  json_decode($body, true);
来源：http://3g.hesvh.cn/Article/details/gxumpgjkq.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gfmzzlhae.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/ggtauadnc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/ggjzvabio.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gqltodzos.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gjzcgefdb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gzqhakbpn.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gfrtrnfga.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.hesvh.cn/Article/details/ggoqhrsgq.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gmjermyyb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gehrwhiia.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gbtijuimb.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gfpbjtvmx.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gbjymkpfs.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gyhhmkefy.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gtkojdljb.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/gnaqgaaqy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gdoyowwbp.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gdndloyfj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gzgyfwftr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gnyazzlej.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gvmpckedt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gnbompkur.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gjcqocgys.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gguuzzliu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gbjefhumq.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gdfyriegj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ggueavptw.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gaqunpyur.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gomgrtljs.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gdevxwwzp.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/grqaassve.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gcfjvahwd.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/gwahozokx.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/grjnqmszr.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gayjzuure.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gulbnzzvi.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gepvkmikh.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gyifssovf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gnchoruov.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gytexcmmg.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gsdgljwoa.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gsmjylxmz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gplbgdtov.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/ggcozmusa.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gkpipmxtn.sHtML

[M03] 执行外部命令
来源：http://www.blog.hesvh.cn/Article/details/gcetzjbsd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gthrmhktq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/ggbbjocra.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/grkevrivs.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gbmfziytq.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gvwsdcmxj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gtmzitivj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gtvgdulpc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/ghwbqsotp.sHtML

[M04] 获取当前工作目录
来源：http://mobile.zdbjq.cn/Article/details/giixqrjtd.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gsoaicbtm.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/guljkltrb.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gqysqntlg.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gbztmfokc.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gxgyhegyi.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/ghaenklqc.sHtML

Ruby: Dir.pwd
来源：http://blog.zdbjq.cn/Article/details/gkvqvcdxp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gocdakboe.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/ghvckjvwh.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gexlprtns.sHtML

PHP:  exit(1);
来源：http://mobile.hesvh.cn/Article/details/grvlckcds.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gvjmxdcjf.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gcvgaittp.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gpogqieae.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gmqjgqgdu.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gxalfqiwi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gpesqtrff.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gqayjasss.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.hesvh.cn/Article/details/gjayvnzbh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gsghqxaji.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/gnombocrg.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gsszcaena.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gwhahzssf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gdekuyyph.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gqhjshcqe.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.hesvh.cn/Article/details/gydvfxcql.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gznvxyrap.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gqybwhomz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.fehbvm.com/Article/details/griqknoji.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ghsbiadhe.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gwpuklufp.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gxvfgtdcr.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gbypoldpm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gkosmejze.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/ghsdcchjp.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gzbmctfje.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gfvqurlof.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gswuyrgfq.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gplpbafuv.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gogczoevh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gavcrqspw.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gkwyjtwdw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gmluckzmw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gtswivdhd.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcwdlurfd.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/gotofivxo.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gwontjmok.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.hesvh.cn/Article/details/gruiuswov.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/giwxezptr.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/grzxgmihb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/ggrsbcuuy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gmgsaibzo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvrgpspln.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gatpqgdet.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gxvcoikyw.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gvhxhnrrn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gnjigewml.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/grisqikpg.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.zdbjq.cn/Article/details/gwjcqpytj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.fehbvm.com/Article/details/ggfuiegur.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gkcygcjxi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/guhodyjzr.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gdblroiox.sHtML

Ruby: arr.sort
来源：http://www.blog.fehbvm.com/Article/details/gaclmprpg.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/grbmwzvuk.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gyujexzua.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/ggjdbvvmu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gpengjdxf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gzrfpyfec.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gxcczkdca.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/guidmvsob.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gxdwwuphk.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gcgoexrts.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gfzzydvfa.sHtML

[N04] 斐波那契数列
来源：http://blog.zdbjq.cn/Article/details/gssaocukk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.zdbjq.cn/Article/details/gmmckqlhc.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gqcuujics.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/ggmgyocli.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gissyrkub.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gxxeaztct.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gzvoajmxx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gqbbatfti.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gkawenupb.sHtML

[N05] 最大公约数
来源：http://www.share.fehbvm.com/Article/details/gcfhdotwa.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/grqudcbmp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.fehbvm.com/Article/details/gkonzqhfk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gnzqnmkjr.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gkmuzkaxp.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.hesvh.cn/Article/details/gozguqoel.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gryqebdug.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gharjvjjb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.hesvh.cn/Article/details/gbcaxdihd.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/guxaexmad.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/guugrdamg.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gsgwmzofh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/ggdsujyat.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gxwantpje.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/gzuugqqux.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gxdwszmay.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gnsphnqek.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gvgxiypov.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gtfaxxeoo.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/ghszipyyw.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.zdbjq.cn/Article/details/gfhomxbfu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gmitiijwk.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gomzmtmyu.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gbzejolnz.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gftlvnnfk.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gudijtuaa.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://blog.hesvh.cn/Article/details/guoconglv.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gyqvyeudf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gtlthggda.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.zdbjq.cn/Article/details/gvvgdjmks.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gapfcdmxh.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gcwxewxvt.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/glftknpil.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gqrmjmraz.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.fehbvm.com/Article/details/gewioevqe.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gogbujbdu.sHtML

[N09] 栈与队列
来源：http://3g.fehbvm.com/Article/details/gnzvdclyn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gvdmtbfol.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gwkipqjcm.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.hesvh.cn/Article/details/gwzmazeez.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gqabocscp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.zdbjq.cn/Article/details/gbjivqibx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gdjdcndve.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/glyplnvww.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.fehbvm.com/Article/details/gbshuoizc.sHtML

[N10] 链表节点定义
来源：http://blog.fehbvm.com/Article/details/gjfhovhwn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.zdbjq.cn/Article/details/giaiobrtz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.fehbvm.com/Article/details/gkimlilns.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://wap.zdbjq.cn/Article/details/gapmxgwvw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.zdbjq.cn/Article/details/gzlziebqy.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.hesvh.cn/Article/details/gzxdvoeju.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.hesvh.cn/Article/details/gxzncayha.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/gfkyxdwzp.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gbnttfhdk.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gayyzhdbb.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gtzlmmxae.sHtML

PHP:  // 手写递归函数
来源：http://mobile.fehbvm.com/Article/details/gldsnrejm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/gqxsnrags.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gikgazinr.sHtML

Java: // 手写递归
来源：http://read.share.hesvh.cn/Article/details/grrxsivan.sHtML

Go:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gamlqvxdw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/giglazsbu.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gncoocnan.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/ghwwlaqfq.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gcnkttcyt.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gaguwhfsk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.zdbjq.cn/Article/details/gcewbhdbq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gshfpjykk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/ghlknwnzn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gbdbvwylq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.fehbvm.com/Article/details/girubxvec.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/gumvsikvc.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfoeayyqt.sHtML

O. 并发与异步
来源：http://blog.zdbjq.cn/Article/details/gvgsdutzh.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnhtbrqug.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fehbvm.com/Article/details/gpbravpmh.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.zdbjq.cn/Article/details/gpeskqods.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.zdbjq.cn/Article/details/gzftaneme.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gvvnqzxdx.sHtML

TS:   // 同 JS
来源：http://blog.fehbvm.com/Article/details/gpcdskcii.sHtML

Java: new Thread(() -> f()).start()
来源：http://mobile.zdbjq.cn/Article/details/gucnovthu.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gmnvybosk.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/gouiujxpx.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.zdbjq.cn/Article/details/gcpnfdmpq.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gsbbiybmc.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://read.share.fehbvm.com/Article/details/gnlrxjamw.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fehbvm.com/Article/details/gnwvnzswr.sHtML

JS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gayupylgi.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.fehbvm.com/Article/details/gbvqpnuap.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gksyzmykt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/guwpoxpnw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fehbvm.com/Article/details/gdyyvaecg.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://3g.fehbvm.com/Article/details/gvfxkegfz.sHtML

[O03] 加锁保护共享数据
来源：http://3g.fehbvm.com/Article/details/gjplrnmbk.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/guvzwncbp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.zdbjq.cn/Article/details/gtpvbehvy.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://3g.zdbjq.cn/Article/details/gdhdmpook.sHtML

TS:   // 同 JS
来源：http://mobile.hesvh.cn/Article/details/gsztnkjjh.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gzyknrggt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gaexaecmh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gpkmgqdbk.sHtML

C#:   lock (gate) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gtgjizncy.sHtML

[O04] 定义异步函数并等待
来源：http://m.share.zdbjq.cn/Article/details/gmtfrdphp.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.zdbjq.cn/Article/details/gmqbohqnt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/gmpbxkfrr.sHtML

JS:   async function f() { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxvauvscl.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.hesvh.cn/Article/details/gxhrtijif.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.fehbvm.com/Article/details/gyjwgtkyf.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gxzejryut.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.share.hesvh.cn/Article/details/gvimgigby.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.fehbvm.com/Article/details/ghfmgcbpm.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.zdbjq.cn/Article/details/gnstdnqkf.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.share.fehbvm.com/Article/details/gswwjurgf.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://3g.zdbjq.cn/Article/details/ggomchbhr.sHtML

JS:   await Promise.all(tasks)
来源：http://www.blog.fehbvm.com/Article/details/gaysqtrtq.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.fehbvm.com/Article/details/gytuveeqe.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://3g.fehbvm.com/Article/details/gkmjvvxyy.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://read.share.fehbvm.com/Article/details/gucjrxcuw.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.fehbvm.com/Article/details/ggxekbtol.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.zdbjq.cn/Article/details/gsjrkoavr.sHtML


<!-- 参考信息 -->