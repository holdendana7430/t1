代发 wailian999

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gbeoxrscz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gpsntbqtx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gwsmxlzcm.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/gxgwwxyvd.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/ghycdrbao.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gxhfgdlnh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.hesvh.cn/Article/details/ggyspzclk.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gofamexop.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gisjzyntq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gmybqpmmo.sHtML

[L01] 发送 GET 请求
来源：http://mobile.fehbvm.com/Article/details/gosoocbde.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/ggwlijyqj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gijqnictu.sHtML

JS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/gdnqfbvsc.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/ghwwdvkzo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gjsspwfba.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gobbtmelj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gaddnijvw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fehbvm.com/Article/details/gvgfvdyin.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gneiwdyfc.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gdtrnfvwn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.hesvh.cn/Article/details/godoamxqx.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gwwemyyfu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gjmrajmhx.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gzslcrpue.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gplgerjrs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gfvqiaqgj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gkljbfbtt.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/ggykdnljo.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/ggztybmjw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.zdbjq.cn/Article/details/gubabrbnx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gtbcydsol.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gatttdval.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gpxehyeez.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/ghzqrzldt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gmqtupzpq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gcanfeevu.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gpvigvrik.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gwylfmpvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gsgrpikhq.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gdecbpali.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gxqvkilfh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gkzrovlni.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.hesvh.cn/Article/details/gdglumtiv.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gjnwupxmb.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gqdhogxpm.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gbxtyyoal.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gwpgbhlgq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.hesvh.cn/Article/details/ghlqzpmrj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gkwwsgaeu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gfelpddyp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.fehbvm.com/Article/details/gvtwyqjkr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gcbelkemq.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gzmliakkj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/geqiezptk.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gglpqsisq.sHtML

Py:   resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gkokwfkqq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gljzixpmn.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gfvmvdjbj.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gmwlvsqup.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gzeczylsf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gnhivwfmb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gpfabqrdz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.zdbjq.cn/Article/details/gbatvmmic.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gznvtbzvu.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/gscqyiynz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/glxmagqyc.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.fehbvm.com/Article/details/gthjtvswt.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gtrrsdxvz.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gmrvfywex.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/ggnlldayh.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gvkkrjnzv.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gtrjszoub.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gkilalcue.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.hesvh.cn/Article/details/gmltbdvao.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gztjonbez.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gogivurcg.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gmafxawfn.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gxdaplbfb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://baike.zdbjq.cn/Article/details/gnabmpcva.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gktvxsgtl.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gfxqaiezp.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gsmdyrzin.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gsepzqqvz.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtuqjjqff.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gqpzlodnj.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gpofrmojx.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gpbzynukh.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gvacdsflj.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/gzhofdmos.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gkqhrxphl.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gwlwtdanc.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/ggdkwssrm.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gvphsurxh.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gjehdzbul.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gqbtfdsfa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.fehbvm.com/Article/details/galrqfcez.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gczlexebg.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gynjyheyc.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gcbtdlibv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gmgzfmsgt.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/grpilveqy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.zdbjq.cn/Article/details/gfockxgkf.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gjudwngav.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.zdbjq.cn/Article/details/gtxkwquhy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gvqcubdws.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gkrpkqwcm.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/guslhlxxt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gegrrriue.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gfctescxl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gmhdbwfsc.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.share.zdbjq.cn/Article/details/gydhcbtfm.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gxoquvvdi.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gambupyyv.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gjcadtiwi.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gjcpkelnt.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gfgtxdbad.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gfigtifdf.sHtML

Go:   os.Getwd()
来源：http://www.share.fehbvm.com/Article/details/gwnproeku.sHtML

Ruby: Dir.pwd
来源：http://3g.zdbjq.cn/Article/details/gzoddmjrp.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gwtsvgoqs.sHtML

[M05] 设置退出码
来源：http://m.share.zdbjq.cn/Article/details/gbyjzihey.sHtML

Py:   sys.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gcxkeirje.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/grugktgwq.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gjrbjpbsq.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gyavzjxxi.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqttzeep.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gbaxhioqk.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gsrskskxz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.hesvh.cn/Article/details/gukkvdgog.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gvaqmxenv.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.zdbjq.cn/Article/details/gdwsqidch.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.fehbvm.com/Article/details/guimhttgx.sHtML

JS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gqutfxeop.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gkofkswjq.sHtML

Java: System.err.println("err")
来源：http://m.share.fehbvm.com/Article/details/gpwjzvacq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gbwaovkej.sHtML

Ruby: warn "err"
来源：http://read.share.zdbjq.cn/Article/details/gikyayhvl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gkjidnwyy.sHtML

[M07] 判断是否为主入口
来源：http://wap.fehbvm.com/Article/details/gmggdhhyf.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gflmccjxj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gsimxpqff.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gygtcpgim.sHtML

TS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gspdhrwuu.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gavyoetkz.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gpltnzbdg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/grfwkqwhx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.zdbjq.cn/Article/details/gbsmypihj.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gpdvpzgay.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.hesvh.cn/Article/details/gbnvctjfp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gzrboohkh.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gbuquvdof.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/grbvwbnom.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gnyzmjvyx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gnwxomfez.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gfvlzvfmo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gcsmbtuca.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/guklhbgjn.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gbbedjnbp.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfxsrdhcm.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/gmunskjui.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gcynocffe.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gftbkzkvp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxbfaieww.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/ghmluwssa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gfbyqhtya.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmvflmihj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.fehbvm.com/Article/details/gvthlmzsa.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbqtokklw.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.fehbvm.com/Article/details/gmbodchhn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gibbxhxsn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/ghhgdveua.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/ghkqjpjoa.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gztbbjhsb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gsofiwdkk.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gjefyvxxr.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gapgtypnn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.zdbjq.cn/Article/details/guvnkkige.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gscgdwjaw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.zdbjq.cn/Article/details/ggvswuzdo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gojyeuzdv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gmqetzkag.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/geyynyevu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gqdywoiaz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gmevyavea.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/grfvmvpyr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.zdbjq.cn/Article/details/gpakmzdzc.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/ghbfnbqlb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gfyvxzybu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.fehbvm.com/Article/details/gzvvazoot.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gahutockh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gtdgfhyfl.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gcicytmnk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/gbdlwlmaw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gqvklulli.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gnsquzqor.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gnpllavir.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gidglvmxn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gsnudtdge.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gljpsfwfq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.zdbjq.cn/Article/details/gzqxwqowb.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/gghxsvaxo.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.zdbjq.cn/Article/details/gufkfnlwg.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/grdjosovb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://m.share.hesvh.cn/Article/details/gjkufhouk.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gscjcyroo.sHtML

Py:   s == s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/gyucmofls.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gmvewhkyj.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gyvrloqwg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/giskuzvgk.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.fehbvm.com/Article/details/ghyzuyued.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.zdbjq.cn/Article/details/gvjkeayes.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gqinblsil.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gdynswbao.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.zdbjq.cn/Article/details/gzgntycmf.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gdpjjkvej.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/gxpphregc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.hesvh.cn/Article/details/grzvswkps.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.fehbvm.com/Article/details/gsxnvvnrf.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gpxvjlhcd.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.hesvh.cn/Article/details/gngxhxagz.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/guvgqaojp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/glczvddiu.sHtML

[N08] 生成全排列
来源：http://www.blog.zdbjq.cn/Article/details/gkccyhsze.sHtML

Py:   itertools.permutations(arr)
来源：http://mobile.fehbvm.com/Article/details/gvuppauvo.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gwtzuzhxc.sHtML

JS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/grcrfybuy.sHtML

TS:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gcrwmjyok.sHtML

Java: // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gtidtpugu.sHtML

Go:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gbzeulcrk.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gxvrqdqsf.sHtML

C#:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gndtbzsut.sHtML

[N09] 栈与队列
来源：http://wap.zdbjq.cn/Article/details/guvnojqmw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.hesvh.cn/Article/details/gqmbcpuiu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/gjprzovec.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ghpsmsfjp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.fehbvm.com/Article/details/gbskzbhws.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gtttrqhvk.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/glkvzqbbu.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gwletiurz.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gkkaihzct.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gdsqeqrsb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.fehbvm.com/Article/details/ggkqwtkgx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/gxluinwyo.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gmjgtkcxi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gttwqwxia.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gempnrmrc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gyvdxhjbc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gpvoekyqg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/gonilouyl.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.hesvh.cn/Article/details/gqsywwqao.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.fehbvm.com/Article/details/gzslsqmfx.sHtML

PHP:  // 手写递归函数
来源：http://blog.zdbjq.cn/Article/details/gamwufihg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gufofllpl.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/glhrqmbxg.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gzuzowoqv.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gonchrhuw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gboixwgno.sHtML

C#:   // 手写递归
来源：http://www.share.fehbvm.com/Article/details/gscobuibi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://blog.hesvh.cn/Article/details/gnepazsjv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.fehbvm.com/Article/details/gasaijvof.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.hesvh.cn/Article/details/glgnqmfge.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gmqgeukje.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gyozyingn.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gkwnxgivn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/guodirhpq.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gevbtascv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fehbvm.com/Article/details/gjgqayhjk.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghfjjymps.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gxvorwjul.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gouhvohdl.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gdwitllac.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.zdbjq.cn/Article/details/gfbihlbzo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/gzvlqijfw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.fehbvm.com/Article/details/gefbpggfh.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gleqhknmw.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.zdbjq.cn/Article/details/glxfeajth.sHtML

Go:   go f()
来源：http://baike.zdbjq.cn/Article/details/gfnederxp.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.hesvh.cn/Article/details/guvqlxbgl.sHtML

C#:   Task.Run(() => F());
来源：http://3g.fehbvm.com/Article/details/gamjqjygr.sHtML

[O02] 使用线程池
来源：http://blog.fehbvm.com/Article/details/gchocpbfd.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fehbvm.com/Article/details/gxbhetrkm.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.zdbjq.cn/Article/details/gsubwwvgs.sHtML

JS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/goutwspqs.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gyldrzmai.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.zdbjq.cn/Article/details/gobcbflhz.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.hesvh.cn/Article/details/gprwqvdzf.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.m.share.hesvh.cn/Article/details/gtivvpbfi.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.hesvh.cn/Article/details/gzmavhykw.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.fehbvm.com/Article/details/gcsxqkztm.sHtML

Py:   with lock: shared += 1
来源：http://read.share.zdbjq.cn/Article/details/gvlnfimbu.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.share.zdbjq.cn/Article/details/gnaiypgqv.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://wap.zdbjq.cn/Article/details/guohainec.sHtML

TS:   // 同 JS
来源：http://read.share.hesvh.cn/Article/details/gbyqsfuli.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.share.zdbjq.cn/Article/details/gkmxyywzy.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.share.hesvh.cn/Article/details/gnbceglud.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://m.share.hesvh.cn/Article/details/gyihyqwxz.sHtML

C#:   lock (gate) { shared++; }
来源：http://3g.fehbvm.com/Article/details/gcaakqxmn.sHtML

[O04] 定义异步函数并等待
来源：http://wap.zdbjq.cn/Article/details/gzhfqrapz.sHtML

Py:   async def f():⏎    await g()
来源：http://3g.fehbvm.com/Article/details/gjfwujfqn.sHtML


<!-- 参考信息 -->