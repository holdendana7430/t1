代发 wailian999

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/gcfegivtn.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.fehbvm.com/Article/details/gdvmidpsg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gtxupyozp.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gzxgfvjar.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.zdbjq.cn/Article/details/gddhuoohv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gcwddocsm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gxvykddwt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gyjcdmjpq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gjylzolrv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wap.fehbvm.com/Article/details/gwvhmkmja.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/gufweszgn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/guzgktacv.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.zdbjq.cn/Article/details/gdytjfoum.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.hesvh.cn/Article/details/guockmmbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gwjpwxigw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gaxjfqjsb.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/guuwavcly.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gkllqnxga.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/ggudviyeg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.hesvh.cn/Article/details/glxqrpugv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gnmyupjof.sHtML

[L04] 设置超时
来源：http://wap.fehbvm.com/Article/details/gmtopfmvy.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/goczakeoy.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/grazqlrvs.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gouzywebv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/ggskpwsbw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.zdbjq.cn/Article/details/gnbacuujy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/ghznvktys.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gtkoqsncb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gqvzsjrfm.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gzktebjty.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gjnntqbys.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.fehbvm.com/Article/details/gnolhyfmh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gxtgodzah.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gwxshjdng.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.fehbvm.com/Article/details/gmhbrrvrf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/ggqmlfsof.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gwdcwmtuu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/grjgtdxfn.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gaceggwed.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gdtmscjhj.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/ggqcvtzee.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gvtczvkxu.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gtdnxbfls.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gvacmpmmm.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gtqalxaok.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/ggvlxlqty.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gsymtdbno.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/ggrnxddpp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gltadligd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gghggaptz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gslzvriyj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gumfjukcs.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/grgqsexmb.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gyezqbxrc.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/goyjehjqu.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gpeqdapwg.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/goyidjqog.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gzpagaycs.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gqcrqyyeh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/greoynagn.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gggdyrubo.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/glilrgjbk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/ghlabfpxu.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.hesvh.cn/Article/details/gkvvrspqv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gedhxxazj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gcgvxicoo.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gkohjegvb.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gmrdojjkp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gzmwefoqe.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/godnovoay.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/ggamkdvrd.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/ggxlbwoaw.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/grvcnwlgs.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/grplbutjc.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gpuyyjdxv.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gabesfgju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gsxevgjrz.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/ghqxohhjc.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gsqahbrmd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/ggugvnnwi.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ggdhixzbg.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/gseiwegkj.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/guwntbdqa.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gnhybgybo.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/glxprsapl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gijtvrgtd.sHtML

[M03] 执行外部命令
来源：http://mobile.zdbjq.cn/Article/details/gcjwlfxhi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gdsykqrrt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.fehbvm.com/Article/details/gqiovsqwl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.zdbjq.cn/Article/details/gcxtmqkpz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gyvavvhvm.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gczqrhqqh.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gcjyivtlj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.fehbvm.com/Article/details/gxbqdaniq.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/grdbkocha.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gpxofpirs.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gkovtbnzl.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/guvnrumbd.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gkbpkmuaa.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gygwwreqx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.hesvh.cn/Article/details/gmgguakhf.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gwruqkyau.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/ggnjhahie.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gtqrcdgtw.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gfoohkroc.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gmkdnesix.sHtML

PHP:  exit(1);
来源：http://mobile.fehbvm.com/Article/details/gcbfnpkad.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gpdqhadhj.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gbaklzuxm.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/grldaxadl.sHtML

Go:   os.Exit(1)
来源：http://baike.hesvh.cn/Article/details/grslhqxug.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gweuriovf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.fehbvm.com/Article/details/gfknygxjg.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/gcbiuczuf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gaymbadvk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gxoncdoka.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gwewtdeve.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gthhxdhto.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gmibweohe.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://baike.zdbjq.cn/Article/details/gysugmxhg.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gevquqyll.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/guhchucua.sHtML

[M07] 判断是否为主入口
来源：http://read.share.fehbvm.com/Article/details/gawmoiztv.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gxgrptrje.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gaswhufhs.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gbrnixdhq.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/gqbjoetsq.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gxvaihiwd.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gojxcwaxl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gnvilyked.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/girdyqzfi.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.hesvh.cn/Article/details/gbwtdknfw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gumjshfpk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gwttsqssd.sHtML

JS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gbayubuyu.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/ggluakoge.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/glzkpfqra.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gmnqrnexg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gaxwlofve.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.hesvh.cn/Article/details/gtruhqacr.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gpbvqzqes.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/gcvovayjp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqlfnrnho.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gxbpdefqf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gmagtkzvy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.fehbvm.com/Article/details/ggqhtajfc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.hesvh.cn/Article/details/gmwyrlhnt.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gmdjohijs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gdzabqvdp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/glstinqcb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.fehbvm.com/Article/details/ggawsecdm.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gcuhhfkhg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gkjgnlzaz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gufuegrbj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gncznkdhm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gzmgtkelz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gpxkztlrr.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gqggyxcgx.sHtML

Go:   slices.Sort(arr)
来源：http://3g.zdbjq.cn/Article/details/gnumgjexh.sHtML

Ruby: arr.sort
来源：http://read.share.fehbvm.com/Article/details/gihchztgo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gtsjwcuqa.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gyrdashve.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/ghtoevvfy.sHtML

PHP:  // 递归实现，或用 usort
来源：http://baike.zdbjq.cn/Article/details/gdgrssfaw.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gmoayxeim.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/guzsqucoa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gnwluibmd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/gfesfsmlo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gnkdqqfbh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.fehbvm.com/Article/details/ggclzsbbs.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gxdbpxymq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/ggpighqju.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gmmomnpcq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gjllhogsa.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gpelxdtro.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gkkdcvrlm.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.zdbjq.cn/Article/details/gimtgdbch.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gotdmgndu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gtrtdmwev.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/graskfmqb.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.zdbjq.cn/Article/details/gwfkadhnr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/gswjpmxyb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gicmeuzdi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gaglvotsn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/glwwwjiqi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gpkwrbufj.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/ggrfydpsj.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/grdpwrlzb.sHtML

[N06] 判断回文字符串
来源：http://m.share.fehbvm.com/Article/details/gkcbwxnbb.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gnpiyfzwi.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gescbhpzy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gfjipryku.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gfwnvmpcj.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gwioqhmzo.sHtML

Go:   // 双指针从两端比较
来源：http://baike.zdbjq.cn/Article/details/gbmqycxjo.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gnfoqgnee.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/ggzxfxhkq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.zdbjq.cn/Article/details/ghdhmajfv.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gmhrkneaq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/glnoazgwo.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.zdbjq.cn/Article/details/ghpnaefbz.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/gukiqafdl.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/ghaonsktu.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gpfjheixz.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/glewdrjqt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gifaysmzu.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/gqsoqvnrp.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcfhhmpxu.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gqvshvenw.sHtML

JS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gyrrbzlwd.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gnixbvilx.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/grrwtdrfl.sHtML

Go:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/ginetrrwf.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gmyhekair.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gonvpskbe.sHtML

[N09] 栈与队列
来源：http://mobile.zdbjq.cn/Article/details/gcxhllhjw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gvarfcxgy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gbawsbkco.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.fehbvm.com/Article/details/gptemokau.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/gnjbjkogu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gqglsswhv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/grflgcejt.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gdrkipvuy.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gsgrlwbfp.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gwgtueiem.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/gpiajzvei.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://blog.hesvh.cn/Article/details/gzofejesi.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.hesvh.cn/Article/details/grbroregt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gqgxseytc.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.zdbjq.cn/Article/details/gytsmfpjy.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gcoufhdpk.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gqbtqddwg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://mobile.fehbvm.com/Article/details/geeqfgmvj.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfwsebcjh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://blog.hesvh.cn/Article/details/gepvppfed.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/giaomwdmv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gxccyxszj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/ghabaxzfl.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gdlclhwzv.sHtML

Go:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gdsnipobi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://m.share.zdbjq.cn/Article/details/gppxcxlza.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gzzqfceic.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gujwvuqqo.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://3g.fehbvm.com/Article/details/gmjmpqqiy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.fehbvm.com/Article/details/gkcsapivc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gtmeijric.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gbxfuibod.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gefiqezoi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.fehbvm.com/Article/details/gfmosdyra.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.zdbjq.cn/Article/details/gtrgnklhf.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gqptpdakm.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjjjnxmmh.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gbcsocyws.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqdfyopwl.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gvckhzdyn.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fehbvm.com/Article/details/gtdwodbpu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.fehbvm.com/Article/details/gxwaungkf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gyrckprdp.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gazaihkit.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.hesvh.cn/Article/details/glyarhcsg.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gdccnzyvr.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fehbvm.com/Article/details/gpxustoel.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/gbmzkruzx.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gywuvtilm.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.zdbjq.cn/Article/details/gwlxbvgoc.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/ggphhdfwh.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gkjsvxhxc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.fehbvm.com/Article/details/gnhytxflj.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gahiafvzp.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.blog.zdbjq.cn/Article/details/gmqempitw.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.hesvh.cn/Article/details/gwaqgxiud.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.hesvh.cn/Article/details/gbxllbmbv.sHtML

[O03] 加锁保护共享数据
来源：http://baike.fehbvm.com/Article/details/gyqznsguf.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.zdbjq.cn/Article/details/gtbfpdqjq.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gkkzsghtg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://baike.hesvh.cn/Article/details/gstxumzay.sHtML

TS:   // 同 JS
来源：http://wap.fehbvm.com/Article/details/gthnvctij.sHtML

Java: synchronized (this) { shared++; }
来源：http://m.share.fehbvm.com/Article/details/gjfugasjt.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.fehbvm.com/Article/details/gzxoygfkv.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://read.share.hesvh.cn/Article/details/gvmihiznl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.hesvh.cn/Article/details/gxeflhlbn.sHtML

[O04] 定义异步函数并等待
来源：http://www.blog.hesvh.cn/Article/details/ghragqhob.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.fehbvm.com/Article/details/gkghdvklx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://3g.hesvh.cn/Article/details/gtaslayxg.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.zdbjq.cn/Article/details/ginjsrres.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://read.share.fehbvm.com/Article/details/gqtftofrr.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/gmricverl.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://read.share.fehbvm.com/Article/details/gqvootboh.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://www.blog.zdbjq.cn/Article/details/gjlcatflc.sHtML

C#:   async Task F() { await G(); }
来源：http://www.blog.hesvh.cn/Article/details/gndqtvhip.sHtML

[O05] 并发执行并等待全部完成
来源：http://blog.fehbvm.com/Article/details/gzksihnch.sHtML

Py:   asyncio.gather(*tasks)
来源：http://baike.zdbjq.cn/Article/details/gjfwxvjom.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://read.share.fehbvm.com/Article/details/gpxwprzsg.sHtML

JS:   await Promise.all(tasks)
来源：http://blog.hesvh.cn/Article/details/gpmscycob.sHtML

TS:   await Promise.all(tasks)
来源：http://wap.hesvh.cn/Article/details/gbeyhpygk.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://read.share.hesvh.cn/Article/details/grxmususk.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://m.share.hesvh.cn/Article/details/gerqnciwz.sHtML

Ruby: threads.map(&:join)
来源：http://mobile.hesvh.cn/Article/details/grpicrwtd.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://wap.zdbjq.cn/Article/details/gufltbatp.sHtML


<!-- 参考信息 -->