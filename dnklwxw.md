代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gaydlifid.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gorwzdhad.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gqhpqgfrx.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gmwjrpnks.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gnrihovyl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gutgydtrp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gboypsxeh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gbcmgojbw.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gfpeqrodb.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/giodbylat.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gnilgrbbq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnjiniufz.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gajhkfwhs.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwzkaqvjd.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gllqbwbbv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/galuhznmv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/grntxjxqo.sHtML

JS:   await fetch(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gtsgumllg.sHtML

TS:   await fetch(url)
来源：http://www.share.fehbvm.com/Article/details/gzbnpkcfy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/gqwuqtfup.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gmdaztpee.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gguqqjybm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gyqzojbgp.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gtxpsnmyn.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gijsairhm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gywerwrac.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gvgacaawi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/girvmgpwc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/goefkwqbp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.zdbjq.cn/Article/details/gillbmpuz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/geertmmzb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/grajenrxd.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gkzzgapfm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.hesvh.cn/Article/details/gqvhknogf.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gtrgyyouc.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gqoczxozs.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gczxiolwz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gkwbuldzt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/ggktfuofb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gjdozxejj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gvnalqigk.sHtML

[L04] 设置超时
来源：http://m.share.fehbvm.com/Article/details/gfgzliqor.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gefbvqpfd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gflmrifdm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/ghwqegajz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/ghthozqyd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.hesvh.cn/Article/details/gqfrrsadc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gclximybm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fehbvm.com/Article/details/gpbaeplmx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gkejzahwh.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gsbdzyigo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/govmfsrgv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gdefjuame.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gnvseyzuz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gcfggyqfi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gohyzegpk.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gkcgqhkgj.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fehbvm.com/Article/details/gxtrxldxw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gyztmziik.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/ghtcafkyz.sHtML

Py:   resp.json()
来源：http://wap.fehbvm.com/Article/details/gycidyktb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/gydpuytfk.sHtML

JS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/grqnysudm.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gtpwvnhje.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gtadovfby.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gwgyjhlka.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gxkqgitqb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gwhwivrqe.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gbrdwswjn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.fehbvm.com/Article/details/glbnbraau.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.zdbjq.cn/Article/details/gswkhoqni.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fehbvm.com/Article/details/gvsmufrkj.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.fehbvm.com/Article/details/gmwxrcnph.sHtML

Java: resp.statusCode()
来源：http://baike.fehbvm.com/Article/details/gocvjdqne.sHtML

Go:   resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/golzcchoe.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/grfjawmuk.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gcntkkrxu.sHtML

[L08] 并发请求多个地址
来源：http://read.share.fehbvm.com/Article/details/gkalsoger.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/grcxcbgge.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gubdhqdup.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gkhsigbti.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gczvnlwyz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gxpdnafbq.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gwhamknzg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.hesvh.cn/Article/details/gjumxwuuc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gzkfrtqta.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gzfidtbpf.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.zdbjq.cn/Article/details/gzjhkgrnl.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gsjugvllo.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/gizwuqqkk.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gefysdtcp.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gtsnkmrlz.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gxbodyswd.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gzpmqhcqz.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gnoogxfaw.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gribsoehg.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gqjxutfrw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gqvyrdizn.sHtML

[M02] 读取环境变量
来源：http://www.share.hesvh.cn/Article/details/gnwxzsbfe.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/glcdqnppj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gfuhrcowa.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gzxopffun.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ghkctkrkf.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gmowtvsfy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gwflwbgug.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.fehbvm.com/Article/details/gazogltrc.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gthsptveb.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gbiezhwjy.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/goxctmvgl.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gzxrgwlcp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/grnovkbzo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gomeirfcg.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/ggbocuuez.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gpkebypwe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/gbromnjmo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gidzqqlvq.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gvfvvxehg.sHtML

Py:   os.getcwd()
来源：http://m.share.hesvh.cn/Article/details/gabegkapp.sHtML

PHP:  getcwd();
来源：http://www.m.share.hesvh.cn/Article/details/gpgccssia.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gbfvoolll.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/ggihqjsrr.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gswhtwhfn.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gwsxvaofb.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gtuymtxtw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gzfdzccge.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gltzcttgh.sHtML

Py:   sys.exit(1)
来源：http://mobile.hesvh.cn/Article/details/grpowdmbq.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gdqwbehsz.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gmkowjptk.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnlitzvwu.sHtML

Java: System.exit(1)
来源：http://3g.hesvh.cn/Article/details/gyjsaccmc.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gahjceibp.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gkgzisvtl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.fehbvm.com/Article/details/gpotxaseb.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gkppfaekk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gkouvhudi.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gniuxvyzg.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gwxzmteja.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gucfhjpgh.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gouhztumb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/grqtosefn.sHtML

Ruby: warn "err"
来源：http://m.share.hesvh.cn/Article/details/gcpgcohbp.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.zdbjq.cn/Article/details/gsoubsfms.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gkkrbbyxr.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gbtpnfakf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gvzxnezzv.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gbidfohzq.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/grjmpkvty.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gdmsdipjp.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gokvsfitx.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gbbstdgyc.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gbsjtebzi.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gwckptfwd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/glgzhkged.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/gtauenmba.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/glijdtwcd.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gsohgmhpa.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.zdbjq.cn/Article/details/gepvachcq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gzruscoxc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gvsrzkqzz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.fehbvm.com/Article/details/gqcimoqcu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpzipcjvm.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/ggbpysomb.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/goytakhhn.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gdgqkcjeu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqkxqgsil.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gdayaymbe.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gudhqphhu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gkynujdzl.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gofnbanjb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkoklmpeh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gpxgtembe.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gzpdtocqm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.fehbvm.com/Article/details/gbznvbihj.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.zdbjq.cn/Article/details/goztlchfi.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gutequuig.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/giqckvsux.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gfufhpjdo.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gphxcxkgf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.fehbvm.com/Article/details/gwundzzzu.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/gnrfajtql.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.zdbjq.cn/Article/details/ghkoxohzz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.hesvh.cn/Article/details/gqvgardkk.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.hesvh.cn/Article/details/gbreqnaxw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.hesvh.cn/Article/details/gmpbwskvm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gglvooqpt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gblnpwbzm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/gbkcoyyav.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gpszliuwl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gazgqugey.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gfqqudbor.sHtML

[N04] 斐波那契数列
来源：http://www.blog.hesvh.cn/Article/details/ggovwybzo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gwemmitno.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/glpyraljv.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gcujhbrss.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/grsbqhhdo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gygymqffx.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/gxpkfpfvn.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gdfcfxwfg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gqpoupfsc.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gaempuwhh.sHtML

Py:   math.gcd(a, b)
来源：http://blog.zdbjq.cn/Article/details/gqdyjdsmr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/grccgzivi.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/glvfkjjqw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gizwyljqa.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.zdbjq.cn/Article/details/godnbymif.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gxralofmx.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/glhxgtopc.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gyviezfsm.sHtML

[N06] 判断回文字符串
来源：http://3g.hesvh.cn/Article/details/ggvdejipz.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/ganpwmxzo.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gajukoowt.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ggvuegfwf.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/ggzlfunyy.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.zdbjq.cn/Article/details/gzsnffzqg.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/ghopqpuel.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.hesvh.cn/Article/details/gzoufatoy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gvlgdaccj.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gdtyejkxl.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gnxlectaz.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.zdbjq.cn/Article/details/ghybswabg.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.zdbjq.cn/Article/details/gobyrlyde.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gsznqkwuq.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fehbvm.com/Article/details/gkojivmtl.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.fehbvm.com/Article/details/ggttnqejv.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gaqpjjgbw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gcbreflix.sHtML

[N08] 生成全排列
来源：http://baike.fehbvm.com/Article/details/gmjpagfuz.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gkqkwkzig.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/glwkldpsz.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsylmvnum.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gxghdimym.sHtML

Java: // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/gamsmlkya.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gklsvywxo.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.zdbjq.cn/Article/details/gmehkgtbm.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gearlxueo.sHtML

[N09] 栈与队列
来源：http://wap.fehbvm.com/Article/details/geommmgkq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gqxtzsvbu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.hesvh.cn/Article/details/gjojpkqld.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gziiouojb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gphdzyvro.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.fehbvm.com/Article/details/gtaguieyt.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.hesvh.cn/Article/details/guyoueyck.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gutgtgrii.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gfkzsqhhc.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/ghxbngdfm.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/gsvyonetg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.fehbvm.com/Article/details/gbnrmumvd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.zdbjq.cn/Article/details/gbahoaqrs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gnukcqqyw.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.fehbvm.com/Article/details/gllytsihz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://m.share.zdbjq.cn/Article/details/gbjntekrz.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gmrwujmfg.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.hesvh.cn/Article/details/ghrvpldlb.sHtML

[N11] 二叉树中序遍历
来源：http://read.share.zdbjq.cn/Article/details/grjjsfreo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gsypfnbaz.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gyvkjggss.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/glfaasssb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gauvpzfiv.sHtML

Java: // 手写递归
来源：http://www.blog.zdbjq.cn/Article/details/gvzywaubg.sHtML

Go:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/gmhmwbknw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/gbsbprojq.sHtML

C#:   // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gklfwlytl.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gtycdozmk.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.zdbjq.cn/Article/details/getvhkrge.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gtflkhnyi.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.zdbjq.cn/Article/details/gdeqxzsbj.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gsqcfjdly.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gcwufpjqh.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.zdbjq.cn/Article/details/gndrwzink.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://wap.hesvh.cn/Article/details/gdzngjqkg.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gmvthlhlf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gclkpyile.sHtML

O. 并发与异步
来源：http://3g.hesvh.cn/Article/details/gjqwwhhxi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gnwlvliqh.sHtML

[O01] 启动一个线程
来源：http://read.share.zdbjq.cn/Article/details/glxsqxbln.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcxwrbv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gcbropiou.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gjkhshsdi.sHtML

TS:   // 同 JS
来源：http://blog.hesvh.cn/Article/details/gbxjobqgh.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.hesvh.cn/Article/details/gnetdxwmy.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/gkuyidsug.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/grtuqbbtm.sHtML

C#:   Task.Run(() => F());
来源：http://3g.hesvh.cn/Article/details/guiawrnkf.sHtML

[O02] 使用线程池
来源：http://baike.hesvh.cn/Article/details/gnbcmtaez.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.fehbvm.com/Article/details/giwqktlyx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://baike.fehbvm.com/Article/details/gsmecymof.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.hesvh.cn/Article/details/gxpeleklp.sHtML

TS:   // worker_threads 线程池
来源：http://baike.hesvh.cn/Article/details/gsnnxkxoz.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gkcfkyyur.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://m.share.hesvh.cn/Article/details/gjhmefjws.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.fehbvm.com/Article/details/gossuvhsk.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.share.hesvh.cn/Article/details/gvuyniamf.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.hesvh.cn/Article/details/gyscjczbt.sHtML

Py:   with lock: shared += 1
来源：http://read.share.fehbvm.com/Article/details/gljjttvns.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://m.share.fehbvm.com/Article/details/gqjililif.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://mobile.fehbvm.com/Article/details/gaqcfpcnv.sHtML

TS:   // 同 JS
来源：http://www.blog.hesvh.cn/Article/details/gnbcxuuas.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.zdbjq.cn/Article/details/gavwuwfkk.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://3g.fehbvm.com/Article/details/gxfdlqscd.sHtML


<!-- 参考信息 -->