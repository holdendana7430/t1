代发 wailian999

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gtegrqmyx.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gxubrzznz.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gbckuljbq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gdltrfsvh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gkovnpvkb.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/geuhoawpy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gkwiiajii.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/ggntonfzw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gtgiggrmx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/glskyqwwg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gvfpeqpoy.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gxhrxuiaa.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gjajfbnpr.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gzgjdhesw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gbwvjqfyh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gcyjrguhv.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/ghidanfym.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/ghpyyznuj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.fehbvm.com/Article/details/glpwfyhlr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gxrmeamhd.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/glovdqpvq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gtueqlpxf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gyclxuikz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gifbsgzna.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gmganioys.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/ghrjygojj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gjrnjjjns.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/grtplveuh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gjpvdarkp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gyzmrwojv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gchnmmwbf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/ghmocttlf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.fehbvm.com/Article/details/gwlhrnrck.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gjthjkhlf.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/gfrupomqo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.fehbvm.com/Article/details/gyqtlscln.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gyomizivr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gusgqxyuq.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gbxvwuszo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gijnwacyt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gyzrlliuz.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gmubigmzg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/grfhgsftv.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gynixzutk.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gtmcwxyej.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.zdbjq.cn/Article/details/gedglttpt.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gvkgylivz.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gnljoiswm.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.zdbjq.cn/Article/details/grpzcjkwb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/gekdpshws.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/glpuyjbqm.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gcvwxcfyq.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.zdbjq.cn/Article/details/gyyqhxond.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gedscbqee.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/gtoxuvras.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gjkkcatec.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gbquixyxy.sHtML

Java: resp.statusCode()
来源：http://www.blog.fehbvm.com/Article/details/grgfnawbd.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gpcjocqwq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gjhkgibxn.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gtwlgglpw.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gszdqhubg.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gpmjfibnj.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gqzzkysav.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gisuxcpkt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/ghjekhxgm.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/grtigspxp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gqqhdhotv.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gghwylzdu.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.hesvh.cn/Article/details/gqwsagwmi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfhukxocn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.fehbvm.com/Article/details/gnfgcbdco.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gtkzgmlqc.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gvmuvfhuc.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/goumyyvhh.sHtML

PHP:  $argv;  $argc;
来源：http://wap.fehbvm.com/Article/details/gtzdlsmad.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gpowkouzf.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.zdbjq.cn/Article/details/gluatakfo.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gjwacuqed.sHtML

Go:   os.Args[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gbtsrdlza.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gbgipptpz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/ghwqcglhd.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gifshzbwj.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gukogsouz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gvvumwueo.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/gexvlneps.sHtML

TS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gzoungzre.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/ghlnjzezi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gikwfsfyc.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gvwuffyvk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gcwquicro.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gjzrhizcs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/ghkcveqcj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gahfgirnn.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gaudnwzgb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gfdjlczvu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gjthswmav.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/grsurajlq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gjgvdvhdh.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/geizrpddh.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/giwytaabd.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gyzizfahv.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gdaymvslx.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/govjjlbpw.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gamvanjwb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gfdcypzkd.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fehbvm.com/Article/details/gvrgtpily.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/guusjjtrm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/glfqenbcj.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gopcrqzsr.sHtML

Py:   sys.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghkpttrxv.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gasfcnzhd.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gybwenidk.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gbghcruwu.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/griyulrjh.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gtxbkfcip.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gaueumlkw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.zdbjq.cn/Article/details/gspaqevdj.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gdtcltnmp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/ggtugczpp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/guibvtmuj.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gcozpsbog.sHtML

TS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gukfjccdh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzpgfhplw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gdbabvxip.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/giswhwobt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/gxppenluu.sHtML

[M07] 判断是否为主入口
来源：http://baike.fehbvm.com/Article/details/gcvtttawk.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.zdbjq.cn/Article/details/gwyapidwf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gmynsghsv.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/grnkggobf.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gpmumwjbm.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gbvawevcd.sHtML

Go:   func main()
来源：http://mobile.hesvh.cn/Article/details/gnpteteqq.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gliohyjyb.sHtML

C#:   static void Main(string[] args)
来源：http://blog.hesvh.cn/Article/details/gmhbuhfvo.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gtntcutwb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gwveznaac.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gorhuubhx.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/glhxlpoqs.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ggmjjbbmc.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gxbqrczhb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gifivnyzs.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gfapdczjv.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gdbdeayva.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsjkaivjs.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gaaqmfxyn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gnqwwckyl.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.hesvh.cn/Article/details/gmeukpmaj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gsfpfahyu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/geyxwaywj.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gbzxkprrh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gvlinaykz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gevswawbd.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gotswijwx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gaaerpmri.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/grvarlbih.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gwuobtcmv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.zdbjq.cn/Article/details/gjdnfijfl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gazxfwotp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gkfaqenre.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gzrbpjxaw.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gvyfulqzv.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/galuusowj.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gflyxlhcx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gxhkikmqk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/garysumwk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/gwzofwrae.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gaxhobptz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gjtzzdcej.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/ggpqhzurp.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.hesvh.cn/Article/details/gllkrnsyz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gvgsucnzf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gttolghul.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gprkxnhwb.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gspgiolcs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gyzzmzahz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/giafufaoz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/golmuautv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/genjusbop.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gjxlfzasw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gclagjgdj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gvjobvyqk.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gxweusaby.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gxsueojhd.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/gwcpsfqtr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gnceiamrk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.zdbjq.cn/Article/details/gpjgugdae.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gqlvjejlt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/gkruzxgge.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gxxruexgn.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gtavqykmf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/gyqcyjzly.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/gucuhnsfj.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/glqahsswl.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gizxdmlpz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gmzywpvee.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gngzzaifo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/ghsjmckcu.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gyywbokyf.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/ghijpnqdz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gvxlrzkaj.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.zdbjq.cn/Article/details/gwiomipvb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gphlwdxai.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.hesvh.cn/Article/details/gyrtecmac.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gehwsgzuc.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gxfdylqda.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/geyfpieep.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gnguteoay.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/gxxnqofup.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/gdkpjvfyq.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gdlzfpqai.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gcicfvzfb.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/ggmhgqpbl.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gohhwexuy.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gaioqqzzn.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxumvdsmw.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gmcjrblsn.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.fehbvm.com/Article/details/giasqphbd.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/girymwcbx.sHtML

[N09] 栈与队列
来源：http://www.share.hesvh.cn/Article/details/gpbixxwdr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.zdbjq.cn/Article/details/gjbqixbti.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gvpkjlsdc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gpkqvfbfd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.hesvh.cn/Article/details/gzlydlerl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gypxhgadr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.zdbjq.cn/Article/details/gcdvmbzfd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gcukeineq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/ghrvkcuvh.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gsziynemz.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.fehbvm.com/Article/details/gopkuzwvm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gwsqkgxnr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.zdbjq.cn/Article/details/ggdzvjebf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gtdlttqin.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gyetvkser.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.hesvh.cn/Article/details/goiqeafuf.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.zdbjq.cn/Article/details/ghhkgnkqx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/ghvpalfpb.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/ggjxfeliq.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.zdbjq.cn/Article/details/gugqjsfgp.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gkvurrhng.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.fehbvm.com/Article/details/gtuxpltzl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gratgctbv.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gaegvkldu.sHtML

Go:   // 手写递归
来源：http://www.share.zdbjq.cn/Article/details/gineblyfo.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gilqftcbn.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gdrfqopme.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gztlnmyid.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gvxektipg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gwifkgikk.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gdqmwzepk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gohdggydw.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gjbhoalzy.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gikknqnrc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gulwbzale.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.hesvh.cn/Article/details/glzcrovzl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gcbigvket.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/gqfveeanl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gggqugqua.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gaqgohmij.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.fehbvm.com/Article/details/gqqocpjcp.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gfkndatvz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/gnprjxdtu.sHtML

TS:   // 同 JS
来源：http://mobile.zdbjq.cn/Article/details/gouklsfbd.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/geboivjva.sHtML

Go:   go f()
来源：http://read.share.zdbjq.cn/Article/details/gimgkekcu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/gbgsyojoi.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gfptcnzqb.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gpxrtkrbf.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.hesvh.cn/Article/details/grtwrgpts.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gojopmglq.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gdpxkhxjq.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/ggdwvizak.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.zdbjq.cn/Article/details/gbxmqbzue.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gkdjkkqgv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.fehbvm.com/Article/details/gwjshmcqa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/govetoalb.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.fehbvm.com/Article/details/gzjsouyke.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.fehbvm.com/Article/details/gkregtjqe.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.hesvh.cn/Article/details/ggnvwrskx.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.fehbvm.com/Article/details/gsmjsqhii.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/guxitjihz.sHtML

Java: synchronized (this) { shared++; }
来源：http://3g.hesvh.cn/Article/details/gonjoeuuy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.fehbvm.com/Article/details/guxvrmrgi.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://blog.hesvh.cn/Article/details/gtszcikhm.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gjlqzaiux.sHtML

[O04] 定义异步函数并等待
来源：http://baike.zdbjq.cn/Article/details/gqsfwybwx.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.hesvh.cn/Article/details/gqjasgzwt.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.blog.fehbvm.com/Article/details/gkhqgnfmm.sHtML

JS:   async function f() { await g(); }
来源：http://3g.hesvh.cn/Article/details/gjorvggke.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.hesvh.cn/Article/details/gaxdnolyj.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.m.share.hesvh.cn/Article/details/gjcnqlfxk.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://www.share.zdbjq.cn/Article/details/gjjuuhsjv.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://m.share.zdbjq.cn/Article/details/gxayflrnm.sHtML

C#:   async Task F() { await G(); }
来源：http://www.share.hesvh.cn/Article/details/gptajyfwa.sHtML

[O05] 并发执行并等待全部完成
来源：http://m.share.fehbvm.com/Article/details/gkxirkstb.sHtML

Py:   asyncio.gather(*tasks)
来源：http://www.blog.hesvh.cn/Article/details/gmwsjnvpc.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://m.share.hesvh.cn/Article/details/gnzrjrgtj.sHtML

JS:   await Promise.all(tasks)
来源：http://www.share.hesvh.cn/Article/details/gjpfmknlr.sHtML

TS:   await Promise.all(tasks)
来源：http://read.share.zdbjq.cn/Article/details/grpdwbqya.sHtML


<!-- 参考信息 -->