代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gutxtkrgo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.hesvh.cn/Article/details/gahkxrphp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/garyswuig.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/ghixhknem.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gkvqtmriw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/glyfvcjnz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gxbzmemoh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gieindwiu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.zdbjq.cn/Article/details/gmfsmepaf.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gsecjqzeu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gjyxcnbvk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/ghszislly.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gpziivtud.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.hesvh.cn/Article/details/gebjgxtwz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/glrsxpinn.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gfgnustbx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/goepbatpd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.fehbvm.com/Article/details/gvcupqmcg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gcyyvmhpf.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.fehbvm.com/Article/details/gkwjbhfrb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/ghpzcoiqc.sHtML

[L04] 设置超时
来源：http://read.share.fehbvm.com/Article/details/ganuyydfa.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gnowhelrc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://m.share.zdbjq.cn/Article/details/gtwsumaqr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/guinopvux.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/grfrnrode.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.fehbvm.com/Article/details/gmqhrdqho.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gevxdkoev.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/gwgmmnueb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gacznsljc.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.hesvh.cn/Article/details/gqumnhnuc.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/grlnuvahl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gogkwnvmq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gfkoapgrg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gkckzcnwx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gywllkakg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzsdfpsbh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/gtypcradj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gdfowkwut.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gdsfftzzu.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gdjyjlpjs.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/ghtpdinoe.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gekwczvto.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gduqbkppp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/ghjpwmnwb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gkzjjunws.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gfbrbkcze.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/glclpdhlr.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gybsyivpb.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/guvxvtuaw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gzdauimkp.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/geqdlrrbk.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/goyaizdry.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/geqkvhnpv.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/ghqsyioxx.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gfufattpw.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gsivapdfr.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gsiovmkpl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gljizbzay.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gkzthdkkl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ghfzkkdjn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/gcoizolzb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.zdbjq.cn/Article/details/gxrtzhheo.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gqldphesu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gdyrbxjwb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gkkyqcjdj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gjqqinfju.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.zdbjq.cn/Article/details/gjkxqucva.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gcrabozny.sHtML

[M01] 读取命令行参数
来源：http://mobile.fehbvm.com/Article/details/gcsnnartc.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gdgyowpjn.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gtgwpwehk.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gtiqefowm.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gwsoxyiuq.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gstbqnnkd.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gxfnktrui.sHtML

Ruby: ARGV
来源：http://m.share.zdbjq.cn/Article/details/gieqgrrac.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gqhgwoznk.sHtML

[M02] 读取环境变量
来源：http://wap.hesvh.cn/Article/details/gpojidzdb.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/gkjcuajkt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gfkhejtqe.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gjoycbjqx.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gdtrdbldl.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gchgtkeas.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.hesvh.cn/Article/details/ghckhjxbl.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gesnwftlc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gensmvfdj.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gzgnlrxyd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gjxwfumrb.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.hesvh.cn/Article/details/gofdnvird.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gzkwdvbfm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/grqzjsyqb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gogfdfwjm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.hesvh.cn/Article/details/gsiwsogem.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gfwmoysyu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/giysvnayo.sHtML

[M04] 获取当前工作目录
来源：http://3g.zdbjq.cn/Article/details/ggwbgtqvr.sHtML

Py:   os.getcwd()
来源：http://www.blog.zdbjq.cn/Article/details/gnkxeryva.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gnrfztnkq.sHtML

JS:   process.cwd()
来源：http://baike.zdbjq.cn/Article/details/gxwveltuk.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/ghpusudjp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gbnxfavqo.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/ghardbhwf.sHtML

Ruby: Dir.pwd
来源：http://wap.hesvh.cn/Article/details/gmlnduwln.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gctndwdbw.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/gzyakozxu.sHtML

Py:   sys.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghwxgxlnl.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/gfnfzjdfn.sHtML

JS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gsgfbsrse.sHtML

TS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gpdsuqcwj.sHtML

Java: System.exit(1)
来源：http://3g.fehbvm.com/Article/details/gtyhzfjgq.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gpufndkff.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/goldafknu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gtzukoufz.sHtML

[M06] 向标准错误输出
来源：http://www.blog.zdbjq.cn/Article/details/geiwmkgfx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/glqsnyxbj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gcciffvxn.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gwutfscgm.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/guippfnjz.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gzogdncyr.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gbkeardoh.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/guxflkdgc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.zdbjq.cn/Article/details/gdrtaiplv.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/ghfowtfqn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/goujoqrft.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gqmklohym.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gdslyjfof.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gbvgvlvdd.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/ghvjsszde.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gmvvpjovj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gcechgghz.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gphzhydkk.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gthswwyii.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gyuwvtpfr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/goovmdzxy.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gmlaooyig.sHtML

TS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gliqeqjco.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/ghoqcztts.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/gduztngvy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gntjrkheb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/giexpmuuj.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvaywndpj.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gmsjhzzly.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guhefpyhm.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gpdenaeae.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gjoogoqqi.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/gemejxokq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/guhrhyslm.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gattsbsxt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gnoeipmlq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gwjujdnfk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gvrfqrlqo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gsjiclncf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.hesvh.cn/Article/details/guepjojrj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.zdbjq.cn/Article/details/geznuplnh.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gtbxovcab.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/ggtoiqgxe.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gusveqahm.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/gulmnceej.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gvkpkofzm.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gyfbwgclj.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gndqruaym.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/ghxxujqup.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gjxszpgiv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gbayiopfe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gvpfxmfjo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.hesvh.cn/Article/details/gdyewjbui.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gcxebpkga.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/glkmfvpkv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/ggwonconr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gniamcvyt.sHtML

[N04] 斐波那契数列
来源：http://www.share.zdbjq.cn/Article/details/geccemvvd.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gulewomip.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gdknynkaj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gxqmdlufh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gsbmxtsxc.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gwktlajhm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gblrzsvcm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gpsvgposr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ggclkohtt.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/goutiusvk.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gcpnvdfkq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gvebbwxsl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/ghwsqlpas.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gpbmydbeo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/ginuftiys.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gaboqxyrk.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvgarhuuj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gaexoqted.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/ghhhwhgog.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gvuesbnpq.sHtML

PHP:  $s === strrev($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gfvyfxcni.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ggyfhjlof.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/geuxpjyex.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gxyvmlwaj.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/glntkweyl.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/gnvonjktj.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gxjbkwpvo.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.zdbjq.cn/Article/details/gumtqzmvv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.zdbjq.cn/Article/details/gxnneqman.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.zdbjq.cn/Article/details/ghmfwoaid.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/gvyelfiih.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gcderxvtb.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/ghjzpzjup.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gutzynyro.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/gjjgkaiwl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/gfpaolilo.sHtML

[N08] 生成全排列
来源：http://wap.zdbjq.cn/Article/details/gxqijvlpb.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gpwausoip.sHtML

PHP:  // 手写递归交换
来源：http://read.share.fehbvm.com/Article/details/gutoakduz.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gfosykjow.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gvnzwtgoz.sHtML

Java: // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gjjxtzwzb.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqhawvjga.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.hesvh.cn/Article/details/gzvzpecxl.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gcyvcyvvl.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gvaolvhci.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/gqafvyvks.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gwyecqtuc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gnrftuqrl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/gzbtclyvv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.fehbvm.com/Article/details/gqqfiagwm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://blog.hesvh.cn/Article/details/gtaediuow.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gjplfdgos.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gtuiccugm.sHtML

[N10] 链表节点定义
来源：http://mobile.hesvh.cn/Article/details/gjnpwwxbe.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gtsmlzktr.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.zdbjq.cn/Article/details/gviejrvxw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.hesvh.cn/Article/details/geculjgyz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.fehbvm.com/Article/details/gfbralbue.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gotbizcvt.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.zdbjq.cn/Article/details/gqdlflamq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gmnmkooid.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.zdbjq.cn/Article/details/gerphdkdo.sHtML

[N11] 二叉树中序遍历
来源：http://3g.zdbjq.cn/Article/details/gudleesgv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.hesvh.cn/Article/details/goolhghtf.sHtML

PHP:  // 手写递归函数
来源：http://wap.fehbvm.com/Article/details/gvmccksjv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gcaoxvrur.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gknlnpujb.sHtML

Java: // 手写递归
来源：http://baike.hesvh.cn/Article/details/ghjcvfvct.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/ghnarstgm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/gmvwhscxf.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/giqrzldbw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gdykmizsc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/ghqbplsyu.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.zdbjq.cn/Article/details/gjssawjot.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gjtbwjlav.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gouiyaqob.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gqfgcfnzz.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.blog.fehbvm.com/Article/details/gukscydxm.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.hesvh.cn/Article/details/gicaevhek.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/glhjpamvk.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcszjganm.sHtML

O. 并发与异步
来源：http://mobile.zdbjq.cn/Article/details/ghexsdoef.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grcrsfvkt.sHtML

[O01] 启动一个线程
来源：http://mobile.fehbvm.com/Article/details/gehrpgvjp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gxgcomxmy.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.hesvh.cn/Article/details/gnjbxberx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gofiijpwp.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gplmzeasr.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/gbtmjuoqe.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/getbnmqbb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.fehbvm.com/Article/details/gthersbrx.sHtML

C#:   Task.Run(() => F());
来源：http://blog.fehbvm.com/Article/details/gzkkqaacn.sHtML

[O02] 使用线程池
来源：http://3g.zdbjq.cn/Article/details/glylxscny.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.fehbvm.com/Article/details/gbfbmxoep.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/gxcnvtlqo.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.fehbvm.com/Article/details/gmwdqwize.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gvtdlynml.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.fehbvm.com/Article/details/gvdhkwvew.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.zdbjq.cn/Article/details/gdvsjlcia.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.zdbjq.cn/Article/details/gpbpgygks.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.fehbvm.com/Article/details/gmtjbiddt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.fehbvm.com/Article/details/gzqfvvfnx.sHtML

Py:   with lock: shared += 1
来源：http://3g.hesvh.cn/Article/details/gfeqcctwp.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.fehbvm.com/Article/details/gnfevzcxs.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://m.share.zdbjq.cn/Article/details/gvbhdlkrk.sHtML

TS:   // 同 JS
来源：http://baike.fehbvm.com/Article/details/gfjkllxep.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gxgmxxpxu.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.fehbvm.com/Article/details/gpasbwixe.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.fehbvm.com/Article/details/gbkppzpqu.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gnjtizbtc.sHtML

[O04] 定义异步函数并等待
来源：http://www.m.share.hesvh.cn/Article/details/gtvqtrhyd.sHtML

Py:   async def f():⏎    await g()
来源：http://mobile.hesvh.cn/Article/details/guzwjljpp.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gxspropch.sHtML

JS:   async function f() { await g(); }
来源：http://www.blog.fehbvm.com/Article/details/gwsqneczk.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://m.share.zdbjq.cn/Article/details/gxtolrlcs.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://wap.zdbjq.cn/Article/details/gozvuruoq.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.zdbjq.cn/Article/details/gbugdnbue.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.fehbvm.com/Article/details/gtaivtrus.sHtML

C#:   async Task F() { await G(); }
来源：http://read.share.hesvh.cn/Article/details/gzrqaexet.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/ghyogwgyk.sHtML

Py:   asyncio.gather(*tasks)
来源：http://blog.fehbvm.com/Article/details/gkxfoftwh.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.m.share.hesvh.cn/Article/details/gwppmyusm.sHtML

JS:   await Promise.all(tasks)
来源：http://baike.fehbvm.com/Article/details/gskcgmycv.sHtML

TS:   await Promise.all(tasks)
来源：http://m.share.fehbvm.com/Article/details/gpilsxroo.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/giebtxlar.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://www.share.hesvh.cn/Article/details/gtdfuqkop.sHtML

Ruby: threads.map(&:join)
来源：http://m.share.fehbvm.com/Article/details/gaqidetfh.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://baike.hesvh.cn/Article/details/gqzwqrnvr.sHtML


<!-- 参考信息 -->