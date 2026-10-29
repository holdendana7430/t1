代发 wailian999

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/ggiabmmfp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gceroyghw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gwdddxais.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjbbhozml.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gbjrdragu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/guqmopmol.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gcnytabff.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/ggqgnzoso.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gfgiovhch.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gsfduylop.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/grroaqyef.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gojoywpcf.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gpjfhztft.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/ggqpcievb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gxcmpoekh.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/ggyfodfmy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gnqwknqtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.fehbvm.com/Article/details/gupahzots.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/glxrsknqm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gnubqactl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gawafwwzp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gaddksrwq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gxurzjclj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.zdbjq.cn/Article/details/gxrgqxpmm.sHtML

[L03] 设置自定义请求头
来源：http://baike.zdbjq.cn/Article/details/gwjtbrtzn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.fehbvm.com/Article/details/gjghlsywh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.hesvh.cn/Article/details/gwztkakse.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gvqkknsle.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gvozwvtqt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.zdbjq.cn/Article/details/gfitcrxwr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/gstelbgak.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fehbvm.com/Article/details/ggtyvcrul.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gflntyubq.sHtML

[L04] 设置超时
来源：http://read.share.zdbjq.cn/Article/details/gcjperzbd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/giqueefof.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gjezvvkmj.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ghyzyzoar.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/glysatxua.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.zdbjq.cn/Article/details/gbsmqtmnv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/ghvuqwccm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gibqnyits.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gibpjmrlo.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gpnkkxknm.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/ghvniivem.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.hesvh.cn/Article/details/gsimkrvrj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gksmnqguu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gbpqpejrz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gainvaovi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gihxjevwr.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.zdbjq.cn/Article/details/gjwxdzwha.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/grrsjdxsl.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gyjlnbhci.sHtML

Py:   resp.json()
来源：http://www.share.hesvh.cn/Article/details/guezidzah.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.hesvh.cn/Article/details/gzozlkobx.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gaqvkouql.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gvlosuzxl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gwelydsyb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.fehbvm.com/Article/details/gmodssckz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/ghvgqxfsp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gtsrlqlip.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gawzvihsg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.fehbvm.com/Article/details/gtlcsfyik.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.hesvh.cn/Article/details/gpnvbkwcp.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/ggcnsnjxj.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gzuuamsan.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/giuedtory.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/ggxseudcv.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gbrmalrrt.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gnzduclbw.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gjxjioptx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.hesvh.cn/Article/details/gkjvhvfzb.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gonykepwl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gjaumquct.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.zdbjq.cn/Article/details/gjiypdykr.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gmzucbuye.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gqnhiyklo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gbnttnrfv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.hesvh.cn/Article/details/gizbkabgu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzfodxnoa.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gzshyvxac.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gbkyqzkiq.sHtML

[M01] 读取命令行参数
来源：http://m.share.fehbvm.com/Article/details/gxxgqxtwv.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/ghfhegwoo.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gwyimgunj.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gwfutedfi.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gkfpzcwcl.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gsfqtcien.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gdsghexqp.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gtyytwmvz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/geowgxrca.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/guqfynnyn.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gdomjvbkw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gjppyzwxq.sHtML

JS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gfqxhxeya.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gjsqgxzlh.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gjgkeibxo.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gwzysmtwl.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/ggloyroge.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/grtemsacv.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/ghktqbybs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gcpmxatjf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gkkqoovgl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gjqbviqmy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gwlatgqqd.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gumbifmtq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/givycobvz.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gxobljcdo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/glcsarmtb.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gogeufivm.sHtML

Py:   os.getcwd()
来源：http://3g.hesvh.cn/Article/details/gikvrlaeq.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gsvdxexkx.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gwsugxvzl.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/gthcezupy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/grrqozfwl.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gjrnfosak.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/grzthyccd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/gughzjyft.sHtML

[M05] 设置退出码
来源：http://mobile.hesvh.cn/Article/details/gjkxhblrd.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gyyghxbxs.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gygukjgcz.sHtML

JS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gsvvidctf.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gnswxjekl.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/ggwyojotg.sHtML

Go:   os.Exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfsihxkkl.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gmlephmde.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.zdbjq.cn/Article/details/gmiadrvft.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gupqfvgof.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/geooxvabz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gdlawqufv.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gmountyrn.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gwnafmjlp.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/goroyrfcz.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/gscwtwrwq.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gxwrerywc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gxrxfjasw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gzhbujire.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gdrhbeafn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.hesvh.cn/Article/details/gdjshcoxz.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gtehgbjgz.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gvzubkpsv.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gfblvhijo.sHtML

Go:   func main()
来源：http://www.blog.hesvh.cn/Article/details/gjxzvlzlj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.share.fehbvm.com/Article/details/glparuwrg.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gctfzpnik.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/ggxwnlbww.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.zdbjq.cn/Article/details/gaiomnkmk.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gytusgulk.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gkmrlpapv.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gfvfsbiet.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gdcxtonsb.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/goxbjywit.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gakruohph.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gkjbpwoow.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwgrdbrky.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gnxphdfvy.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/giungrxnw.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gkdhdnwzm.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/grkjsodni.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/geaypsxwz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gzvlfdeel.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gtyrwyjmn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ghreesugp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gcakmpyhf.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/glqurcbju.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gyvssondy.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gffxjrpmn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/gtaxffqvo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gfpdpnxdb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gguorihxz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/grxiludpb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gimrujbjs.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gykctlvif.sHtML

Ruby: arr.sort
来源：http://m.share.fehbvm.com/Article/details/gfkxnrupm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/ghkoifssa.sHtML

[N03] 快速排序（分治示例）
来源：http://wap.hesvh.cn/Article/details/glwhtgucy.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.hesvh.cn/Article/details/gbvcydpet.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gspdylukl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gbuhhlqcw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/ggjutknmo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gjmdfxmyl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/ghhzlhomf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gnhuwovsl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.hesvh.cn/Article/details/gwhqbmjcb.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gydrkuleo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/gpvavpazo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gdaqngkxm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gnwovvwbb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gscdeytqd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gbxcdjlqz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/grcouuggy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gljgvqokf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gilmtwmpj.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gnhpjsban.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gltslthzo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gbcokpkdl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gzcastgrb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/grkrdjppr.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gnafmdsln.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gtipjspki.sHtML

Ruby: a.gcd(b)
来源：http://mobile.zdbjq.cn/Article/details/gwtrfcope.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gzkewrgnu.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gisyycmur.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gkchglwym.sHtML

PHP:  $s === strrev($s);
来源：http://www.blog.zdbjq.cn/Article/details/grhqexbnh.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/grhoyaexn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gvckhaswu.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/grvmfuxof.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gmjvqcdjc.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gtrkumvbk.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gljwoaaoe.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gpybpjshr.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.zdbjq.cn/Article/details/gbowclkhd.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gpyeuezgr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gxtyopfis.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gxuiecjsz.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gkmcgdcev.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gavkajsxx.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/goybdknro.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gnuoqtbkk.sHtML

[N08] 生成全排列
来源：http://www.share.zdbjq.cn/Article/details/guayfqtnh.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gjgdjybdp.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gnvabjkqj.sHtML

JS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/glhaijxic.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gwlvwzqqa.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/geyjkgdsy.sHtML

Go:   // 手写回溯递归
来源：http://m.share.hesvh.cn/Article/details/gtiowbgoq.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/guwpeseea.sHtML

C#:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/guzqrhcgk.sHtML

[N09] 栈与队列
来源：http://read.share.fehbvm.com/Article/details/gwcpilyfs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gphupluyg.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmdfcfkzb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gophwxumn.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gpsiibouo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/giuxfdgfq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.hesvh.cn/Article/details/grtoxgaws.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ghatamxdd.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/goojbxprk.sHtML

[N10] 链表节点定义
来源：http://m.share.fehbvm.com/Article/details/gbkdwgegm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gnhxgaegx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.hesvh.cn/Article/details/gmqhcoogv.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gtceakssu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.hesvh.cn/Article/details/gfpzilldf.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gxcqgxsjp.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fehbvm.com/Article/details/gttwqdjil.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/guosadtok.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/gvpekaftm.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/ginqfddhd.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gvextsfao.sHtML

PHP:  // 手写递归函数
来源：http://mobile.zdbjq.cn/Article/details/gsewdpmsc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/goaaguewh.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/ghrbuscnh.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gqoovlaph.sHtML

Go:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gizfyvacq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gcdneyhxw.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gqkjjivwu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.fehbvm.com/Article/details/gvsutcjyr.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gdieiznsk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gcfqfmkkd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gyuxrjaoh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gbtztofsu.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gskehdzuk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.fehbvm.com/Article/details/gwpbzptbr.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gptohjyzs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/gusemlifz.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gctoylihj.sHtML

O. 并发与异步
来源：http://www.share.fehbvm.com/Article/details/genbzhghg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ggoxbfujl.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gqippbatl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.zdbjq.cn/Article/details/glhnafdtk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gfmizyqhb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.fehbvm.com/Article/details/govjidhjx.sHtML

TS:   // 同 JS
来源：http://baike.hesvh.cn/Article/details/gacpvctfn.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.fehbvm.com/Article/details/gqkxyusle.sHtML

Go:   go f()
来源：http://read.share.fehbvm.com/Article/details/gtpnjpeyv.sHtML

Ruby: Thread.new { f }
来源：http://blog.fehbvm.com/Article/details/gnthrltxy.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fehbvm.com/Article/details/gwyitabzv.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/gnewaghjr.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gpnusakzy.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.fehbvm.com/Article/details/glkwajxyr.sHtML

JS:   // worker_threads 线程池
来源：http://3g.hesvh.cn/Article/details/gukkowqcp.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gjeunwarq.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gsmwhjiot.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.fehbvm.com/Article/details/gmkutfvlv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://mobile.zdbjq.cn/Article/details/gpskklgaq.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.zdbjq.cn/Article/details/gyqlythza.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/guhczqmcr.sHtML

Py:   with lock: shared += 1
来源：http://www.share.hesvh.cn/Article/details/gegfzcwbk.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.zdbjq.cn/Article/details/gtpxknlfc.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gnxjnstsl.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/goyolwntd.sHtML

Java: synchronized (this) { shared++; }
来源：http://baike.zdbjq.cn/Article/details/gcdupgyvx.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.zdbjq.cn/Article/details/gymzitpnh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.fehbvm.com/Article/details/gmpkdjypl.sHtML

C#:   lock (gate) { shared++; }
来源：http://www.share.fehbvm.com/Article/details/gfetfezhm.sHtML

[O04] 定义异步函数并等待
来源：http://mobile.fehbvm.com/Article/details/gyahxwmyh.sHtML

Py:   async def f():⏎    await g()
来源：http://www.m.share.hesvh.cn/Article/details/gfjqcbkfb.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://www.share.hesvh.cn/Article/details/gwteesglh.sHtML

JS:   async function f() { await g(); }
来源：http://mobile.hesvh.cn/Article/details/gyyhtokiq.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://blog.zdbjq.cn/Article/details/ghqdzjbpz.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://www.share.hesvh.cn/Article/details/gusjcxhcu.sHtML


<!-- 参考信息 -->