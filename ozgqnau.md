代发 wailian999

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gjrvrzuhj.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gnhlpbdyx.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/grdexjlgq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gouipawcr.sHtML

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gykaxcuhi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gedlcneov.sHtML

[L01] 发送 GET 请求
来源：http://www.share.hesvh.cn/Article/details/gdhdeviup.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gjndxiyns.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gjkoehmoh.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gwzkyswbv.sHtML

TS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gwgwgeopn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gqjfzcktv.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/goyuzurzw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gwbsyidjz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gptxfivae.sHtML

[L02] 发送 POST JSON
来源：http://3g.hesvh.cn/Article/details/gwucehdsj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/giifqrkvh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gkoxxkvjl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gxgqwkjon.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gffvcrukg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gjrlonmtc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/guqgptpmm.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.fehbvm.com/Article/details/gdqiypjtw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gzddzngmc.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gbjsuswll.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.fehbvm.com/Article/details/gufyhpyhh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/ghydsefit.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gfgssdzfl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/ggevmmkup.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gyrwidhdu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gbfdcrpan.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gufwrssrg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gqicvzjcz.sHtML

[L04] 设置超时
来源：http://blog.zdbjq.cn/Article/details/gtmhwyisz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.zdbjq.cn/Article/details/glhuutlui.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gdbxzsvjc.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gkolczdwr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/ggbmjdzcc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gifknzodu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gjxcdqnrx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gsctowleq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.hesvh.cn/Article/details/gazfvrrwg.sHtML

[L05] 上传文件（multipart）
来源：http://baike.zdbjq.cn/Article/details/galolnmiv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/guwolccuc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.hesvh.cn/Article/details/ggytvgquk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.hesvh.cn/Article/details/ggnymsszl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gsqamtdfp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.zdbjq.cn/Article/details/gohmfpwjh.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/godfkmofx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gtooofrrq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbuwgeeyb.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gjxvfsvpd.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gdcltpvsh.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.zdbjq.cn/Article/details/gjfdtiqgx.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/ggdcjwvxm.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/guuevtcjl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gkzjfdjyn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/ggsezensi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gkhpfoqtf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gihoxhixe.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gimwyjwke.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gtljxejae.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/grwmdactz.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gfwamqfdn.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gfydwpdxs.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/gaohftiif.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gtputbpdd.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gxwynweth.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gcyzkehjl.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gscrscbcu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/ggunvwhrj.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gkgaeuznx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gjyegtjbt.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gwhoadafi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gcysbnabi.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.fehbvm.com/Article/details/gsabnuuhb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gyotvlalv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gjtbyiqne.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxvcoribp.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gduvjkgec.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gbpkssccg.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/grrxcceqp.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gtmsyjmqn.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gznobiivw.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/ghdmtmlml.sHtML

TS:   process.argv.slice(2)
来源：http://blog.zdbjq.cn/Article/details/gqtcwamwz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gnpgqehde.sHtML

Go:   os.Args[1:]
来源：http://www.share.zdbjq.cn/Article/details/gsdkkznkr.sHtML

Ruby: ARGV
来源：http://3g.hesvh.cn/Article/details/gpoaidwdm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gjrebtcpo.sHtML

[M02] 读取环境变量
来源：http://blog.fehbvm.com/Article/details/glicgortb.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gsbnxpder.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gsbjrzhcg.sHtML

JS:   process.env.HOME
来源：http://baike.zdbjq.cn/Article/details/ggdqyjbkp.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gcfeatasl.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gwivoyfuq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gfbtypphn.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gexlbmmnf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gkxtmtzpp.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gayzhijos.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gnqeedixl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gqyxaujya.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gokthxxgi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gselpoigw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/ggwnsooxa.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gywqgevee.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gkbysnyat.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gqlpsookj.sHtML

[M04] 获取当前工作目录
来源：http://read.share.zdbjq.cn/Article/details/gmuphrnbq.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gbmhzuzof.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/gkxaqevth.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gcpbkrhik.sHtML

TS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gchuvuggp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.hesvh.cn/Article/details/gwkidyeby.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gkhdnmovu.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gmkxnmdis.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/gstrqiygs.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gachijewd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glnmdutkf.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gpamwkmwi.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gikjgwkeb.sHtML

TS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/guywkprxz.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/giojqbbsu.sHtML

Go:   os.Exit(1)
来源：http://read.share.hesvh.cn/Article/details/gjwnzfxgk.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gjnoyxhbl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fehbvm.com/Article/details/guwjlcqvm.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gejuulihm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gzuohowzw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gxfryshyg.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gxtiskxns.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gugxaaisi.sHtML

Java: System.err.println("err")
来源：http://read.share.fehbvm.com/Article/details/gnavrfhiw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gahgikwea.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/ghwdyggbv.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gnrpcvcoo.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/gydfqeezu.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gthaajgtr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/ghvjehidb.sHtML

JS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/graaaengo.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gvihiyqwx.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gcvnqlvvy.sHtML

Go:   func main()
来源：http://www.m.share.hesvh.cn/Article/details/gypaesivp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.zdbjq.cn/Article/details/gksyedhjg.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gesmoxlzs.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gquqfflgx.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gpmytnohf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gydybanca.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gdmfpxyei.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/govuwipoa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gdgjzvxxe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gatecyewm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gqfamjajq.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.hesvh.cn/Article/details/glgobwuyj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gditwuwub.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/ggouunhki.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzkaqdeie.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gihdydqbn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gaqxedbig.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gyjjtdzrc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gdwcauiwy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gdkygftie.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gaoateswt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gunqdzuyk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gjobqppxc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gyczdwbrm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/gzyouxzgq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/glveltxsx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gevrfmhzx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gefwcsohs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gykaisfve.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gxwkuepwx.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.zdbjq.cn/Article/details/gpmoyxhdg.sHtML

Ruby: arr.sort
来源：http://blog.hesvh.cn/Article/details/gqricutcz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/ggikoodmx.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.fehbvm.com/Article/details/gwiblhxev.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gzlbzemrk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/ggstjpciz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/gkwiquqmm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gerjbsbrf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gppnanrfo.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.fehbvm.com/Article/details/gvotwxpnf.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gphrhmkzl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.fehbvm.com/Article/details/gzljejizi.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/glomkazfu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/geitzhgwg.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/ggucnklfr.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkoedpofz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gylopkvys.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/gcybihvbf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/grdbezixb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gbwlitqlm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gshiigbfy.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/gxkiaiwxn.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/govojhdau.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/gemdsnmns.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gknmoggan.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gsydygryd.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.hesvh.cn/Article/details/goobksrvi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gxgfpkgmc.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gkjsrzzyd.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.zdbjq.cn/Article/details/gbfeuseji.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gkoqbyetl.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/glfodwaag.sHtML

PHP:  $s === strrev($s);
来源：http://3g.hesvh.cn/Article/details/gdsbnmyqe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmoxorrey.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gpznshpdp.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gtnknqjsc.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gbfwaqekd.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gkfasvhkv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gcnoxriai.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gcanquvnd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.zdbjq.cn/Article/details/gypzdemac.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gvzddaeqz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.fehbvm.com/Article/details/gfvigksev.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gusiinuzk.sHtML

Java: // 手写 HashMap
来源：http://mobile.hesvh.cn/Article/details/ghmltzsrc.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.fehbvm.com/Article/details/gdhflzrwy.sHtML

Ruby: // 手写 Hash
来源：http://m.share.hesvh.cn/Article/details/gupsturhi.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gkqywrxce.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gbdhthnvm.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/ghpromhtq.sHtML

PHP:  // 手写递归交换
来源：http://wap.hesvh.cn/Article/details/gqhidsdpq.sHtML

JS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gycsugfrq.sHtML

TS:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/grfghbvcz.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gytjslujq.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gqdevjjlz.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.zdbjq.cn/Article/details/gzgesnliw.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gswpkvgwo.sHtML

[N09] 栈与队列
来源：http://wap.hesvh.cn/Article/details/gkgozllqe.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/ghjwjuian.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.zdbjq.cn/Article/details/ggutwokzh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.hesvh.cn/Article/details/goxqrzuor.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gaeapthps.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.hesvh.cn/Article/details/glabwelwb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/gkihxpzxo.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gbvzrxdix.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gmckrfpxz.sHtML

[N10] 链表节点定义
来源：http://www.share.zdbjq.cn/Article/details/ghgmhewyv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gzxxyisjt.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.zdbjq.cn/Article/details/goytdafxc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gacpfhigu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gnatvpqhk.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/gaislbptv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gdcysrlay.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.hesvh.cn/Article/details/gfacgvyrz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gotwkdttu.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.hesvh.cn/Article/details/gabboagid.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/ggkeaqmez.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/ggkgnlwch.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gfhrfivkm.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.zdbjq.cn/Article/details/ggmeivbwe.sHtML

Java: // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gcbfvaone.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gjerlwebs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.zdbjq.cn/Article/details/gtqkolwge.sHtML

C#:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gygqsoovp.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.hesvh.cn/Article/details/guwwlngmx.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://read.share.fehbvm.com/Article/details/gypaoasfj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.hesvh.cn/Article/details/ggvwkupud.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gbvckridx.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gibloxshq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gpqjygmwl.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.zdbjq.cn/Article/details/gignzzmbo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gcjsxvvcs.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.hesvh.cn/Article/details/gkzrxbkmp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gxrfquerj.sHtML

O. 并发与异步
来源：http://www.share.zdbjq.cn/Article/details/gkivfkwpr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gvszblpdx.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/ghwsugfmk.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.hesvh.cn/Article/details/gyvfwctcs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.fehbvm.com/Article/details/geabnklyg.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/gsksehkfc.sHtML

TS:   // 同 JS
来源：http://www.blog.zdbjq.cn/Article/details/ggegpjnvb.sHtML

Java: new Thread(() -> f()).start()
来源：http://wap.zdbjq.cn/Article/details/ghltzavgs.sHtML

Go:   go f()
来源：http://m.share.fehbvm.com/Article/details/goxlvhcrh.sHtML

Ruby: Thread.new { f }
来源：http://wap.hesvh.cn/Article/details/gjoyzaigr.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gqcsifuiz.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/gbefwkpyt.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.hesvh.cn/Article/details/gkofqgecf.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/gjajouqkf.sHtML

JS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gnnzxyvnn.sHtML

TS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/ghkpthpyn.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://blog.hesvh.cn/Article/details/gdvvofhsv.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gtkrkrjan.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gpoxavaxo.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://read.share.hesvh.cn/Article/details/gqdbqmwkb.sHtML

[O03] 加锁保护共享数据
来源：http://wap.fehbvm.com/Article/details/gaebojtta.sHtML

Py:   with lock: shared += 1
来源：http://mobile.zdbjq.cn/Article/details/gbfzamzmy.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://baike.hesvh.cn/Article/details/gkluxjecm.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.fehbvm.com/Article/details/geynwrxhx.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gjveufxll.sHtML

Java: synchronized (this) { shared++; }
来源：http://read.share.fehbvm.com/Article/details/gchljvrxy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.m.share.hesvh.cn/Article/details/gobjiibsh.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://mobile.zdbjq.cn/Article/details/gcqpjabef.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gwtynozls.sHtML

[O04] 定义异步函数并等待
来源：http://blog.zdbjq.cn/Article/details/gydloslnq.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/gvjrsrsuk.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://baike.fehbvm.com/Article/details/guubtmskd.sHtML

JS:   async function f() { await g(); }
来源：http://3g.zdbjq.cn/Article/details/gmmznygko.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://www.blog.zdbjq.cn/Article/details/gkmpvjnvo.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.fehbvm.com/Article/details/galzmifpf.sHtML


<!-- 参考信息 -->