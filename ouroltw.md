代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gvfbrevjv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gqyspoyng.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/glglkmeca.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gfvdhkgiu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gczcvauwu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/glgsqgivc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gfgfczzji.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gthhtqfkw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gdvmamylx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gjsyxabhj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gydaljkyu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gzhihnvko.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gwbeabctt.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/glzcwekim.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/guybjbkwd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gbnjdbuhd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gyufzavyh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gspcoyvpz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gyydnctcu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gupoomxid.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gffpbshjh.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/gamcyikeh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gegsmpjpz.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.hesvh.cn/Article/details/gzhrqrrhd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gbrekrwqk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gwdydnwwb.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gmxieaboi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gbqduppno.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gaxeftaib.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/geozxvhse.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gewkpiuaf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/guphsrmfs.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gxiihkbrh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gvrolgzwf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/gpikqqfud.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gcgculdch.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gqyqijtov.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.fehbvm.com/Article/details/gdpqklkpf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gajuecogv.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gjzckeril.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gtvvletcz.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/gimnrimya.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gjxodorhk.sHtML

TS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gkfvmfjrd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gdrncncqc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gkccemonn.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gwntrnzft.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/grirtwyxf.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/glbksbsze.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gbtutqjdu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gmkegpffa.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gdnabcxih.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gejbivqnb.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gjeymotsz.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gmnhgesbx.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gvbxgkras.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/geowomjqk.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gaezmiqet.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gkadvndum.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/gklvmapkp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/glqlxbobi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/glsgsrnbr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.fehbvm.com/Article/details/ggebubohr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gdxtmfkrj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.fehbvm.com/Article/details/gnaszitws.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gjjufuyjk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gyawsmaal.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.fehbvm.com/Article/details/gptmpnwve.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gatnlxfov.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/ggndsoztq.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/gzrcwuinx.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gdgsakapf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gshwissoh.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gnzaybyss.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gdxgvwckg.sHtML

Go:   os.Args[1:]
来源：http://mobile.zdbjq.cn/Article/details/gkjvtkmix.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/ghymsemwq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/gxctfcjos.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gbucpjbim.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gwfcphvud.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/giqzmwfjw.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gjbwlaynt.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gxxhrszfm.sHtML

Java: System.getenv("HOME")
来源：http://baike.hesvh.cn/Article/details/gdsqdktuo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gpliekicq.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gvxodgsoo.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gjjptntvj.sHtML

[M03] 执行外部命令
来源：http://baike.fehbvm.com/Article/details/guahziiej.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gsllsfjuf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.fehbvm.com/Article/details/gwqecgitw.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gxhafdluq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gbkcyqiru.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gwaodvxes.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/glwygtfcy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gkameipbf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gnmyfgmym.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gopqwwrxt.sHtML

Py:   os.getcwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gcpfubise.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/gopjfpssv.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gkigoxdnq.sHtML

TS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/givenmmab.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gezspuslo.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/gpclukdld.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/ghuqncilr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.fehbvm.com/Article/details/gvfdyntwb.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/ggrfmjlot.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gynhattit.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/goszzvxok.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gajffffbn.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gqvanyfdp.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/giqargzra.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gtmpnhuzd.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gwnpdntgt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/grczaglds.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.hesvh.cn/Article/details/grtoyrvpd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.fehbvm.com/Article/details/gepfgssab.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gkfuckark.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gbdtcxted.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gnoaavfip.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gwctshcmi.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fehbvm.com/Article/details/gilcsznxu.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gtkibqygl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gxmwojzbm.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gbrhvrfal.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gdtcywkcm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gcqwojmka.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/giwszankd.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gtiydxnhk.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gcwjdncey.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gpnfymlhh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/glsbcppck.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gmaygtxrn.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gndohwogl.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gpjrkdnje.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gtxhbcjiv.sHtML

JS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/guahhgmgn.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gwvwgyswd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gphupcify.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gsdkkxoak.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gbzwzgzls.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gradorpzy.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvgpuztcs.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gubphprpi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gcidkeamz.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gemabobkb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.hesvh.cn/Article/details/ggzuekuil.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fehbvm.com/Article/details/gjohibpvx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gvtefwhaq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/glyelkngc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gdvobvdeo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/giyucowub.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gomfoeidu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gbeyvhwna.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gplfltjhj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gnfbaiowx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.zdbjq.cn/Article/details/giezmwxfb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gnabohkhz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gpgyeotgk.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gqhmsxowb.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gmxdyodku.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gsozqwiig.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.fehbvm.com/Article/details/gihjahwvi.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gddhjcqsk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gtagovuti.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.fehbvm.com/Article/details/goxqxetpf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/guhddcqie.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gonlkwwut.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/guhvrklvm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gtobdxqjd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gqtwagaos.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/ggewvkeka.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/gqkmfirfn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gawukhhjz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gdlrzdexy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gbfxsargf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gaympopny.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gtrvavaum.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://baike.zdbjq.cn/Article/details/gdvyhqfck.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/guhtmptnb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gcsmuorru.sHtML

[N05] 最大公约数
来源：http://wap.fehbvm.com/Article/details/gycumcvum.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gtzsqclsu.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gffheemux.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gpmpwbizt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gpwhgfqjm.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/gshvoakow.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gcliyuzha.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gkrpctfxc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gpcfrkalf.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/grvebptbt.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/gsdqzquba.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gjcgjpedi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/guezsughg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gbduuitvf.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gzcbrecls.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/ghofssaqw.sHtML

Ruby: s == s.reverse
来源：http://wap.fehbvm.com/Article/details/gzvvxsgph.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gsvvcrrjc.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/grutfqcpy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gnuoqtnon.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gkzpwdvrc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/ggfyutexa.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/gfcktirgu.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.zdbjq.cn/Article/details/gjlftgocm.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.fehbvm.com/Article/details/goyvpcwtw.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gclyuiwug.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gvqzcmvhe.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/gcgvdzofa.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/grbdxjibk.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gchkvuigo.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gfqiiywyy.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gzfxjftvz.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gjzqxocfh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdvvwhamx.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.fehbvm.com/Article/details/garrikgin.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gfljhssde.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gfmpocsae.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gusjlsgyo.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gqmrksgta.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gjacfeidc.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.fehbvm.com/Article/details/gmiwnrhhs.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gpylrlykv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gwcblmqjn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gxxxqadnd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.hesvh.cn/Article/details/gcnhhdfqt.sHtML

[N10] 链表节点定义
来源：http://blog.zdbjq.cn/Article/details/gcfszzwcb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gmkxmoyvt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.fehbvm.com/Article/details/gfxnuqize.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.zdbjq.cn/Article/details/glvhmxenu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gmidixqzk.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/gzrvddifl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/ggfinmlju.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.fehbvm.com/Article/details/gktilgpig.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/ggcqooyei.sHtML

[N11] 二叉树中序遍历
来源：http://blog.fehbvm.com/Article/details/gisllhlhc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/gtvdcxkbx.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gbqccdjah.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gxyvotflc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gcvrsnode.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gaqcomlvj.sHtML

Go:   // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gphhyldfk.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.zdbjq.cn/Article/details/gtfglvxxt.sHtML

C#:   // 手写递归
来源：http://read.share.hesvh.cn/Article/details/gkgkljnlz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gblrgjdkv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/gsxsdcswf.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gowwicxrj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gedzidzkf.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.hesvh.cn/Article/details/gcqdxxbms.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/gohdxzoye.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.hesvh.cn/Article/details/gjzygcaob.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.zdbjq.cn/Article/details/gfpnuesnn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gxsagtnhk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdtslacfz.sHtML

O. 并发与异步
来源：http://wap.fehbvm.com/Article/details/gjzrmmvgf.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gykoztoba.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gyqfzccvv.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/gzwdbdfcv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://blog.fehbvm.com/Article/details/gzegsfhvl.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://3g.fehbvm.com/Article/details/gklrlgupj.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gbnmfxfnz.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gelntcrxt.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gqawjgkao.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gixpzuhzs.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gbjhgddvr.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/grivquvtv.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/gzmaigbzz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.hesvh.cn/Article/details/glblsopmq.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gjaauckjd.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/gdwwayylw.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gzgslbdeh.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gancckigi.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/ggikhvxkn.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gkdwvauzo.sHtML

[O03] 加锁保护共享数据
来源：http://www.share.zdbjq.cn/Article/details/geitfqlau.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gzpghkjtk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://wap.fehbvm.com/Article/details/gsrzdcqkm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/gytbsnfji.sHtML

TS:   // 同 JS
来源：http://read.share.zdbjq.cn/Article/details/gwdytibay.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gibazabbw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.hesvh.cn/Article/details/gpphogpgu.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://baike.hesvh.cn/Article/details/glcbfebei.sHtML

C#:   lock (gate) { shared++; }
来源：http://mobile.zdbjq.cn/Article/details/gwleepsev.sHtML

[O04] 定义异步函数并等待
来源：http://3g.hesvh.cn/Article/details/gnrvalsvc.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gdwjlzdza.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.hesvh.cn/Article/details/giebpuoza.sHtML

JS:   async function f() { await g(); }
来源：http://blog.fehbvm.com/Article/details/gutzdxtdu.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.hesvh.cn/Article/details/gfnknkrxe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.hesvh.cn/Article/details/gnvlzjeyw.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://blog.hesvh.cn/Article/details/grnviowjj.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.hesvh.cn/Article/details/gqqikrmxu.sHtML

C#:   async Task F() { await G(); }
来源：http://wap.hesvh.cn/Article/details/gdvqazkzd.sHtML

[O05] 并发执行并等待全部完成
来源：http://3g.zdbjq.cn/Article/details/gtosdtykm.sHtML

Py:   asyncio.gather(*tasks)
来源：http://wap.fehbvm.com/Article/details/gicvoirqa.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://wap.hesvh.cn/Article/details/gqdwxhdjf.sHtML

JS:   await Promise.all(tasks)
来源：http://read.share.fehbvm.com/Article/details/gvampbohb.sHtML

TS:   await Promise.all(tasks)
来源：http://blog.fehbvm.com/Article/details/gbojhhcnz.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/gawugatcb.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.zdbjq.cn/Article/details/gjdjfdyyq.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.hesvh.cn/Article/details/giqkapjlx.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://read.share.hesvh.cn/Article/details/gbrrlxefw.sHtML


<!-- 参考信息 -->