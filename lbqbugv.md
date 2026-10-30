代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gjudbnyco.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ghglektpl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gkdhtdfrf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gjsgrzqak.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gtugqqrkj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gookjclgc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.hesvh.cn/Article/details/grlcnczit.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gxejmrfhg.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gnynxdedx.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gkbqfblav.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gmgybwdqa.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gzyilytiv.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gbqfdzevf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghgvyobnd.sHtML

[L01] 发送 GET 请求
来源：http://read.share.hesvh.cn/Article/details/gqsylnhzf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gtsyjogfm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://m.share.fehbvm.com/Article/details/guqeddeut.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gwyxyiagz.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gkwkxkvtg.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.fehbvm.com/Article/details/ghblhsyij.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.hesvh.cn/Article/details/gnkzboexs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gqndpgrck.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gxgwgyxxb.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gxfenuzoh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gszfayteo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gvpldxess.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gvgdetlmk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gxgetllsl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gtreogolt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/grnrrchtj.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gguggfbnc.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.fehbvm.com/Article/details/gjslmtzcf.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/glljohray.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gncvjiowe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/ghimubfre.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gnrbofhit.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gjbzhalfi.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/gezzmcqax.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/grhvusfpq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.hesvh.cn/Article/details/gkrajrdju.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gvnmijfvt.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gbffjvzst.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gapwhxfru.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gphefipco.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ggdzwdslt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gxypwkdjx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/guiapjjsu.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/gujjosumb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.hesvh.cn/Article/details/gckqgzbzg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gaqhysuao.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gtllzvnui.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gmpujlqpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.fehbvm.com/Article/details/gmavgnevb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gsacslrtc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gapoerosz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gendmzmao.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gzrcvgxaa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gjaotbimj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/glexqaaxt.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gshgnahfr.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gkxaxffsy.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gweeeqxwi.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/glneuoucw.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gptotwtpd.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/govtcvons.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/gpayyhjvu.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.hesvh.cn/Article/details/gtnfgotvx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.fehbvm.com/Article/details/gzsmltsnp.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gykqntmrf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/ghurcuowa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gnjbwnonb.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/giewfhope.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gwusswpfe.sHtML

Java: resp.statusCode()
来源：http://mobile.fehbvm.com/Article/details/gdmmzhoix.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gbtivmium.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gduybbyuz.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gwkkntrdq.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.fehbvm.com/Article/details/gokqwzrib.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/gadrfawxc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.fehbvm.com/Article/details/gwdhpluyn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gomjvoaaj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gqvptlnqy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.hesvh.cn/Article/details/ggxjkzaac.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.hesvh.cn/Article/details/gzdktsayp.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gdoadqevh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fehbvm.com/Article/details/gbcteebkj.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gojudfrqc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/gkoyjxmnc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gzwzxbyhs.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/ghmyovcoa.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gvamhqatr.sHtML

PHP:  $argv;  $argc;
来源：http://baike.zdbjq.cn/Article/details/gpglyajbj.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gazjxzvod.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gydoeyygh.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/ghjmbbnue.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gohjcvoha.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gmmvcbdhp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/ghoolxxiw.sHtML

[M02] 读取环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gwhegvltt.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.fehbvm.com/Article/details/gdydarqod.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gnxjbkwhj.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gfbwgjwtj.sHtML

TS:   process.env.HOME
来源：http://www.blog.zdbjq.cn/Article/details/gzygteqfj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gqqyszkob.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gszhvdgbe.sHtML

Ruby: ENV["HOME"]
来源：http://baike.hesvh.cn/Article/details/ggclrlniy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gzyxpmmaw.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gxnybpvnv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gnchlkvdn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gzkkjuels.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gqtbpeoyq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gxebpmekk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.fehbvm.com/Article/details/gyatgrpov.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gqnywhocb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/guyfhuuxe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/gnjkgtaok.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.zdbjq.cn/Article/details/gfkyrxpcc.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gcbdrxmxh.sHtML

PHP:  getcwd();
来源：http://blog.hesvh.cn/Article/details/ghbryjlva.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gcnlpwhlu.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gmxomhlbp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gxvcsjguo.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gkrghakyv.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.fehbvm.com/Article/details/gbklnmrej.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/glgzixvdq.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gfoxasuor.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gnmtdkqhq.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gkzjyhafz.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gsexgwuyt.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gmntbpohw.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwdjhphdv.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gyqnocdbb.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gegdmrecr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gajqazken.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gaacpquxp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gxhtjocvj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/ggrisbrzx.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gjdpankei.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gplqfonvl.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/gpzzqnvjd.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gsgcsxwcr.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gcukfboae.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gqbuvwzzq.sHtML

[M07] 判断是否为主入口
来源：http://baike.zdbjq.cn/Article/details/gvvlqlgzp.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/givznyrtm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gfplgnyea.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/ghxilewvq.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gtnpcamla.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gouhodrcj.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gbqtqrzee.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gvdmgrtpr.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/glzfftbtw.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/ggxsrhccq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.hesvh.cn/Article/details/gepcpbxna.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.fehbvm.com/Article/details/gckfirxbe.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/ghzybrfup.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gcbcdotxs.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gbgqagtba.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gvslkmqvi.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gxizkgbay.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gvexnimnt.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gszhlrajc.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gavvnfrkp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxqhiwbhb.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.hesvh.cn/Article/details/gswbdggsx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gpeladpkg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gtofvdwyv.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/gyfzgqbtc.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/ggivrqguv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gkvtexhcs.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjzitgycx.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gwbaeqamg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gywdfhbbg.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.hesvh.cn/Article/details/gwbusyvyw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.hesvh.cn/Article/details/grtdhfeuy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gytdiiwnz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.hesvh.cn/Article/details/gqusewrzf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gbrhvvlcg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gaqqnxwed.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gaekpdlnw.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gpeeupcnu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.zdbjq.cn/Article/details/gfpmotcar.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gtalfzjzu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gkbszjulh.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gnrdnoart.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gafqfrtqu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.hesvh.cn/Article/details/guvyoinxa.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/gfisbyljl.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.zdbjq.cn/Article/details/gzfqwrrxu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/gxlkulodj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/grtmpvxrn.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.fehbvm.com/Article/details/gieaejeda.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gwyemraiq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gmnptkrtz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/griumhofx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gycuqdtpd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gvejhohuv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gjptbtvab.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gnalcizlh.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gfbgwzsbr.sHtML

[N05] 最大公约数
来源：http://mobile.fehbvm.com/Article/details/goxjkigzu.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.hesvh.cn/Article/details/gldghyjyl.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gwtpkxlme.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/genpuhsdh.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gsxwtrfhu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.fehbvm.com/Article/details/gxnseovgj.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gkamwgyxt.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/gtbmuxwks.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.fehbvm.com/Article/details/gggtruhxx.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gnqmycwap.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gbroolvfi.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fehbvm.com/Article/details/ggsamwxlx.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ghyxzlpvx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gkptgimxe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.fehbvm.com/Article/details/gcuzxnxot.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.zdbjq.cn/Article/details/gsrzbuzot.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/gqfhlzuhr.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gqmtwbdnq.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gzuxscehx.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/grwryttgs.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fehbvm.com/Article/details/gpbkdhsgl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.fehbvm.com/Article/details/gcgydksvs.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.zdbjq.cn/Article/details/ggghokzmz.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/ghwsgplzl.sHtML

Go:   // 手写 map[int]int
来源：http://wap.hesvh.cn/Article/details/gaashrafa.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/guqggqlqh.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.zdbjq.cn/Article/details/gwgucxptn.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/glouasteq.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gaigzknjm.sHtML

PHP:  // 手写递归交换
来源：http://read.share.zdbjq.cn/Article/details/gfqnxcuvc.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gobuauhsq.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gggcrytml.sHtML

Java: // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gpwmnozib.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/geptsnovy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.hesvh.cn/Article/details/gkehinnli.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gfiubchmx.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gfxjvndrg.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.hesvh.cn/Article/details/gppveomim.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.fehbvm.com/Article/details/grqrfwlcl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gxfhtwtkz.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/glgrkjccz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gnrrcvafw.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.fehbvm.com/Article/details/grdxgwlkz.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gdjmirunm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gdhuprfej.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gyuvvphuv.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.hesvh.cn/Article/details/gqfslznwg.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gcryrlzpf.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.blog.fehbvm.com/Article/details/grkcopkzt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gpnrerued.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.zdbjq.cn/Article/details/gsunbwvie.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.zdbjq.cn/Article/details/gfiuizwkh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.zdbjq.cn/Article/details/gwgclkqpf.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.fehbvm.com/Article/details/gpbneqvas.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.hesvh.cn/Article/details/ghvpkgfqj.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.zdbjq.cn/Article/details/gbzwrhwhk.sHtML

PHP:  // 手写递归函数
来源：http://baike.zdbjq.cn/Article/details/gnuafuyrg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gzuzjkerv.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gqpyxxumz.sHtML

Java: // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gfhqmvemm.sHtML

Go:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gyqutajyy.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.hesvh.cn/Article/details/glzwczcjp.sHtML

C#:   // 手写递归
来源：http://blog.fehbvm.com/Article/details/glrojobev.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.hesvh.cn/Article/details/gqneouchi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/gnyjoatcw.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://m.share.hesvh.cn/Article/details/grtfwjecx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gfkertcnl.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gyatmkmwm.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/grrbhvbma.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gctvgchbl.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gmfbgznbe.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gyqrdwjct.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvaxobome.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/gwjotybqi.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gemagjddw.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/ggnfdnrue.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.zdbjq.cn/Article/details/gtbpmtkqs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gsqnsoyjz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.hesvh.cn/Article/details/gbzdpnfew.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/ghqianwlo.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/gwqobapav.sHtML

Go:   go f()
来源：http://www.blog.hesvh.cn/Article/details/grskrzvnc.sHtML

Ruby: Thread.new { f }
来源：http://www.share.hesvh.cn/Article/details/gjcklaagl.sHtML

C#:   Task.Run(() => F());
来源：http://wap.hesvh.cn/Article/details/gcacqcaeh.sHtML

[O02] 使用线程池
来源：http://mobile.zdbjq.cn/Article/details/ghlncbyrs.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.zdbjq.cn/Article/details/gfrufaqay.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.fehbvm.com/Article/details/gwebhwufv.sHtML

JS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/gghqzqhru.sHtML

TS:   // worker_threads 线程池
来源：http://blog.zdbjq.cn/Article/details/glxpxmrfh.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.m.share.fehbvm.com/Article/details/gpcbbbfsj.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://mobile.hesvh.cn/Article/details/goasllkfg.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.share.fehbvm.com/Article/details/glikgzgtb.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://m.share.hesvh.cn/Article/details/gfbszaype.sHtML

[O03] 加锁保护共享数据
来源：http://mobile.zdbjq.cn/Article/details/gvtneeeax.sHtML

Py:   with lock: shared += 1
来源：http://wap.fehbvm.com/Article/details/gofwaznzr.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://mobile.zdbjq.cn/Article/details/gpyosccxq.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://blog.zdbjq.cn/Article/details/gwuykvrrh.sHtML

TS:   // 同 JS
来源：http://baike.zdbjq.cn/Article/details/gnoednyfu.sHtML

Java: synchronized (this) { shared++; }
来源：http://www.m.share.fehbvm.com/Article/details/gqhuqhwei.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://wap.hesvh.cn/Article/details/girjorrkv.sHtML


<!-- 参考信息 -->