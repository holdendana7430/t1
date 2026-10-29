代发 wailian999

L. 网络请求
来源：http://baike.zdbjq.cn/Article/details/gcejywczu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkhgtrobd.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gqzlczfni.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/gwtxpnslk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.hesvh.cn/Article/details/gbrpmbeaz.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gmzfklvep.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gedurzehx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.fehbvm.com/Article/details/gvuxhgakv.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/ggfmtsldw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/guedmgrbu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.fehbvm.com/Article/details/ghzegburi.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gamocdjaq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/gjvdnmexr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gzmvjmbns.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gnmiehitc.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/gitywoxui.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gqoeyxpas.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gyttihrec.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.hesvh.cn/Article/details/gqfiegnyd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gkuwqdvjb.sHtML

[L03] 设置自定义请求头
来源：http://read.share.fehbvm.com/Article/details/gypurgayd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/ganipfwar.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.hesvh.cn/Article/details/gvorjlekr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/ghccjpghz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gmytuvwhh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gpgaklsmc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/geeykhrus.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gvatiufzq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gpkzywcpe.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gqnvtavbc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gjuttfena.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.fehbvm.com/Article/details/gtqovxsap.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/gqjklcoor.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gsopfojev.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.zdbjq.cn/Article/details/gwrmkxakm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.hesvh.cn/Article/details/gqazamjeh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.hesvh.cn/Article/details/gslpygnuz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/ggapdputp.sHtML

[L05] 上传文件（multipart）
来源：http://wap.hesvh.cn/Article/details/gdhamrcog.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gbijegfjr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gpoajhyfj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/grqxpycqj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gvkhynynv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gvsvonurm.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gnhxhnygo.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gkjhqvvub.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gdgyknmxk.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gfzsuugvs.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/guggnmzzy.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.hesvh.cn/Article/details/gyfnjtcax.sHtML

JS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gcgxgbmcy.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gefsvqphf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/glznsgcns.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gfuhiofip.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gkqlhcmwi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gartmvebw.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gnvyaukpl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.zdbjq.cn/Article/details/goisggwgk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gvufhqlvg.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.hesvh.cn/Article/details/gyjoeomio.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gaevtligq.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gjwplutro.sHtML

Go:   resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gatrhgxbq.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gjqejojvj.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gsrxrdtci.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gzhlwqwji.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gtiuxwozy.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gvojdcecb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gqtpfceoc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.fehbvm.com/Article/details/gclmwtaif.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.zdbjq.cn/Article/details/gbetspiks.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gyurrkzel.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.zdbjq.cn/Article/details/gjpyixemc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.hesvh.cn/Article/details/gvurkqrrn.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghugdlzno.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/galoorouy.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guenuqxgk.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gfysgvkfx.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gcgyablee.sHtML

PHP:  $argv;  $argc;
来源：http://baike.fehbvm.com/Article/details/gdrwxydnt.sHtML

JS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gktjsvaex.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gdvfokuiw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/guszrqzxj.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gpbdnvubw.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gftmroyrs.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gnjcarrjo.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gcrloqxsh.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gwbirwwnx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gsanlfqtc.sHtML

JS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gmxjtjuni.sHtML

TS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/glzzbuucq.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/ghrffdmul.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/guvbhzzgi.sHtML

Ruby: ENV["HOME"]
来源：http://baike.fehbvm.com/Article/details/gbtsvbeid.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gsfeuwrhs.sHtML

[M03] 执行外部命令
来源：http://wap.zdbjq.cn/Article/details/gtibvvegi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/glccxevcw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gmedqsamu.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gehtifbeb.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/ghozlwxvy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.fehbvm.com/Article/details/gswyjdyeb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.fehbvm.com/Article/details/gmxaypabw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gqoykmrfp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gvwhnybdz.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gucwefjps.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gckdkkojk.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/ghrdqhedz.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gtsbrfkdc.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gprewmnqd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.fehbvm.com/Article/details/gvjtwirlr.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gkegtmirx.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gidqeqzxg.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/goejofifi.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gkcuxxpff.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gknapldiq.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gtmfhyqkt.sHtML

JS:   process.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gcuryuyzr.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gstithbhw.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/glcjvnuer.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/gsprbeynf.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gjlnkqfic.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gcpmjzvrb.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/ghjywjyhw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gdnhytfrw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gspzobazi.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxoalxbrw.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gvykcorzp.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gomefomka.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/gdlzqiyrn.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gpulwcahx.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.zdbjq.cn/Article/details/gjmwikcku.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gakbhdfsb.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.hesvh.cn/Article/details/grocmitvd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/graovjaoa.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/grnsmifqw.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gmccxeevs.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gdlopqfdh.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gpqwpdrnm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/grmnxjdvy.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gnudybekf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.zdbjq.cn/Article/details/gpnrbyuxe.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gylxvszxu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gepdecujq.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gtrbdbses.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmdaxrcut.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.fehbvm.com/Article/details/gtugtjtyy.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gwyfdhrmz.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/gaxzpkzea.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gqypttiqj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gevfgbnqm.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gryegzifh.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpjjsmufb.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gvypkljdv.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gmubstouf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjpnxdwel.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/guykapypz.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gqjogqczs.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gwpvvunhk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/grwdmyxyn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gqslinsxb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gposmdvfh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gbfmgvsjg.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/grkqcosfv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/ghqkajqna.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gnjnrdtxj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/giebqovum.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gscmtnccc.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gsclenelh.sHtML

Ruby: arr.sort
来源：http://www.m.share.hesvh.cn/Article/details/gpxibhana.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.hesvh.cn/Article/details/gujdiawxn.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gxjigyolt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/glmppzzgq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/gufxhixft.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/ghajdvvns.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gzetatpur.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gracicgtd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.zdbjq.cn/Article/details/glsosugzr.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.fehbvm.com/Article/details/gcruaecsy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gnuktdcww.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/gchcfftmp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gvxjjlbgl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gzvgeqcai.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gmounizwc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gcsjrscgf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gpzmjyizb.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/ghmqpzpqf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gpkhdmuai.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gkbbijoos.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gumcifjvk.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/glnnwmrqb.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gfljfciyg.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gvyfhlpau.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmswwknak.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gqpffewra.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gtbbomvqj.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gdszazmyy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/grmkhapby.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gynfrpnvx.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gypesubja.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/gqnyvrcph.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gnpmjzlno.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gdwcewmwh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gbihxzbos.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gpkteisap.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gnncstmqe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gmkwdsddf.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gtdjioumy.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.fehbvm.com/Article/details/gxfcivpql.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gpctxuomz.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/gemyfqpzl.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/geiokwked.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gmmnwqvxh.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gsepswgjy.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/grsvmmpby.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gmjocubfm.sHtML

[N08] 生成全排列
来源：http://mobile.zdbjq.cn/Article/details/gmrfxdptp.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/giagboeru.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/gglmizivr.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gqcgxbcnw.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gbsxddkuu.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/ghlfhzsex.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/griobspqt.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gfbgindcs.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gfozkrwmd.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gbznuhphd.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/gchchsgpb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.hesvh.cn/Article/details/geaflecjv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gvmnyfmnl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.fehbvm.com/Article/details/gluzkjacl.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.hesvh.cn/Article/details/gaedycfaf.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gpwtxicdy.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/godpuffce.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/glgfomztt.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/ghiiosvpg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.hesvh.cn/Article/details/gvjxdcuwp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gyuztuxkh.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gzetshwee.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/gtdzeyrzn.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.zdbjq.cn/Article/details/ggttpzzas.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gryulqxpj.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://mobile.hesvh.cn/Article/details/gxjrdwjuz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.hesvh.cn/Article/details/gaysvcyuk.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gksdosoxc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gbtnquuqv.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/guvafgwlp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/gxfdbqpnj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/goiufveil.sHtML

Java: // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gdpbovpvn.sHtML

Go:   // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gehmwtoqg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gruzivgpj.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/grevavpwn.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gfayfqdgt.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gxisfjrgy.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.zdbjq.cn/Article/details/gspkwubdg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.hesvh.cn/Article/details/gecoisplw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/ggbqygenx.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gazhmkiwk.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.fehbvm.com/Article/details/gbpbxisau.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.hesvh.cn/Article/details/ghkrcppsg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.fehbvm.com/Article/details/gywewykhc.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxffdknco.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gvobgyrzc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gdprievqs.sHtML

[O01] 启动一个线程
来源：http://3g.fehbvm.com/Article/details/gsnjcjiyf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.hesvh.cn/Article/details/gzcpbngzu.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://m.share.zdbjq.cn/Article/details/glnwhzskw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gttpnivbc.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gtrnimjyx.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.hesvh.cn/Article/details/grbkyokfs.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gkmhoivck.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.fehbvm.com/Article/details/gvqjxhcdr.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/gbntdgwnm.sHtML

[O02] 使用线程池
来源：http://read.share.fehbvm.com/Article/details/gmumxobgo.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gwdriizfq.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/glavdqqwy.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gauyconld.sHtML

TS:   // worker_threads 线程池
来源：http://mobile.hesvh.cn/Article/details/gmsyujmum.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.zdbjq.cn/Article/details/gfplizket.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gsybhdohn.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gqgsbekyf.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.fehbvm.com/Article/details/gelfsnzkt.sHtML

[O03] 加锁保护共享数据
来源：http://www.m.share.hesvh.cn/Article/details/gizxogjyk.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.fehbvm.com/Article/details/gqxiuitov.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.blog.fehbvm.com/Article/details/gyqoclydg.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.blog.fehbvm.com/Article/details/gbzihbhga.sHtML

TS:   // 同 JS
来源：http://www.share.hesvh.cn/Article/details/gqpvxuxle.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqisanqlc.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.blog.zdbjq.cn/Article/details/gmltxshcz.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://wap.hesvh.cn/Article/details/gmuxaqiqx.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.hesvh.cn/Article/details/gsprynytu.sHtML

[O04] 定义异步函数并等待
来源：http://wap.hesvh.cn/Article/details/gvkkezasu.sHtML

Py:   async def f():⏎    await g()
来源：http://www.blog.hesvh.cn/Article/details/grjjpcusx.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://read.share.zdbjq.cn/Article/details/ggpyzwhfc.sHtML

JS:   async function f() { await g(); }
来源：http://wap.zdbjq.cn/Article/details/gtbndykmn.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.fehbvm.com/Article/details/gqipywbcx.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://read.share.zdbjq.cn/Article/details/gbzlymzqz.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://mobile.zdbjq.cn/Article/details/gcxnhyuyi.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://baike.hesvh.cn/Article/details/gbgbwqjlm.sHtML

C#:   async Task F() { await G(); }
来源：http://blog.hesvh.cn/Article/details/gpomthczm.sHtML

[O05] 并发执行并等待全部完成
来源：http://wap.hesvh.cn/Article/details/gfbylxkvh.sHtML


<!-- 参考信息 -->