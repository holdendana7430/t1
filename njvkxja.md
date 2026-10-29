代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gpxyiuook.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/glvgmyxed.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/giutnpklz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.hesvh.cn/Article/details/guuzvhhdr.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gbreqorom.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gnhnaudyq.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/guiecygqz.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gkngzkgzs.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gydnskysd.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gpimfghen.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/guvbfufyi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.fehbvm.com/Article/details/gttcrwbsy.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gwyefuwoc.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbgbbythu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.fehbvm.com/Article/details/glupauqii.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gxvxwdlwg.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gdvmyhkqu.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/givnnrxsl.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/guuihmits.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gbcizcvzk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gxzbaoaaq.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gefbjxcvw.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/grtefjhzm.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.zdbjq.cn/Article/details/gnzeaeoyy.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.hesvh.cn/Article/details/gwhzygvdi.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gimeiznzq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/gfgyaazhx.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/graununat.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.fehbvm.com/Article/details/gjhmhnges.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gaepcwemk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gqicmndbi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.hesvh.cn/Article/details/gfhjoycbh.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gxvjimpjg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gxcppznou.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.hesvh.cn/Article/details/gegofmghx.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gihldpxyh.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gecrvmjpd.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/giqpmhmnq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gpkhvrqnk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gilmuuckx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.fehbvm.com/Article/details/gjtcpnvma.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gadcuozum.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gnboyqsga.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/gsipaeqxe.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gipwcpmzt.sHtML

[L04] 设置超时
来源：http://3g.fehbvm.com/Article/details/gmgafwycz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gnbhyqwld.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gxvpaitjx.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/glvencqjd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gqpjgdqql.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/glqzgkcix.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.fehbvm.com/Article/details/gjnpkkunp.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gwheivxee.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gjsudcegg.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gxlxkekjg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gfvuzxbag.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.hesvh.cn/Article/details/goeqfsnox.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/glvrkkykh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gfqpwcoab.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/ghmghimkn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/gbwykgbmg.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.hesvh.cn/Article/details/gdgiajndo.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gsbxjydtr.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gherxzhmv.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gmrmasugs.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gmyrnbbze.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gnupdzzjy.sHtML

TS:   await resp.json()
来源：http://wap.hesvh.cn/Article/details/gbuhyibaq.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/ggrzblqwj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/glqlcekpr.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gtvfmbrpk.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gzwfcgqrm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/glkqfehlc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gzhowamex.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gqslpvgka.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/ggwexgyyo.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/glilewpug.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gkakkjlhx.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gtyqdejev.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gvtdpxiok.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gifftrjbm.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/godndepnt.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/geyillzpv.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.zdbjq.cn/Article/details/gwqaizpyh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/grqfgvcai.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gppfmqdgl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/gvoxqiyxu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gbebkogea.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gfwtefpbb.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gtkfjcoet.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/grsmbmiig.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gficafhes.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtlvdjhkj.sHtML

[M01] 读取命令行参数
来源：http://m.share.hesvh.cn/Article/details/gagisqroz.sHtML

Py:   sys.argv[1:]
来源：http://www.share.hesvh.cn/Article/details/guwopuyvh.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gugcstyvd.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/ggmxfzlsn.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gsjnyxoxv.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gnvjqojcu.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/glcuguopr.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gqffldjut.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.fehbvm.com/Article/details/ggozjtqro.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gaodnvoqi.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/giytsbkef.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gqonwyuqg.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ggeovyoyu.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gpayekksh.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gkyquyfvd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gcavhrfoe.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/grfbqlgmi.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gohalhxus.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gmbkxpzyk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gxvlgfspy.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gymhgtqhd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gfgaegyso.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gduhhspao.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/goevrikpf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gyrqdlzst.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gsbdwzuny.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gynljfesl.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gdaxabims.sHtML

Py:   os.getcwd()
来源：http://www.blog.hesvh.cn/Article/details/gkpuwpons.sHtML

PHP:  getcwd();
来源：http://blog.fehbvm.com/Article/details/ggeotuarc.sHtML

JS:   process.cwd()
来源：http://m.share.fehbvm.com/Article/details/gmnetwoqv.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gtljlrdrk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gyhpayyfc.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/ghxzdlyvo.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gbvancprx.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gseosybvg.sHtML

[M05] 设置退出码
来源：http://www.m.share.fehbvm.com/Article/details/giibecrao.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gokeswrew.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/gvrarlnug.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnwlifsox.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gcmxousbp.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpsayixsl.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfobfeaca.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gckxeoioz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.hesvh.cn/Article/details/gkwddszgp.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gnqueibeq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gvfsjcobc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gqxvzhpqb.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdrpklpjj.sHtML

TS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/gelfcwhvz.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gzpzwlfzk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gygltmjyl.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gxsvflrgj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.fehbvm.com/Article/details/ghyadmbpf.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gzubqltdj.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gyovvnjfb.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.hesvh.cn/Article/details/ggxvliriw.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gdqodtjel.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gjuymuqfw.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/godohnbyb.sHtML

Go:   func main()
来源：http://baike.fehbvm.com/Article/details/gnoggnvzp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gmmwcvfms.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gecvjncns.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gjidyijwo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gmynolmmj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/glsuqpros.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gzegfrnzq.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gbhmsmvra.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gvrwvptoe.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.fehbvm.com/Article/details/gstezaezn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/gyspxisro.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/glzicouau.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glrtdrwlg.sHtML

N. 数据结构与算法
来源：http://www.blog.fehbvm.com/Article/details/gpgeelqtp.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gujwkuefk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gkduwnhgn.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gpbvrleeg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.hesvh.cn/Article/details/gwtlqdzdq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwvpqbhko.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.fehbvm.com/Article/details/ggqdcsljm.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gjllbalbr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gpwzwuowk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gkxpzfblv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gbnvcrxhz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gbhtdzusf.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.hesvh.cn/Article/details/gmsgkrwtn.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/gdkykisbz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/gqooahmby.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gsyclsiyg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gxtgdxmai.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gfucswztt.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/gufqwcoof.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/gobmqzenc.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/gwuvihnfr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.hesvh.cn/Article/details/gyauptamo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.hesvh.cn/Article/details/gruavrhxl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gwrbkzhgd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/grqawknwf.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/glrfpwiuw.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gostlyvml.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.zdbjq.cn/Article/details/grkzkbwfh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.zdbjq.cn/Article/details/glgrzxekl.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/gkwjbzhrg.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/gbgtqvswf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.hesvh.cn/Article/details/ggpgucrgk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gvrfzhsog.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gzvgikodq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gyjrwktme.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.zdbjq.cn/Article/details/grgmslpur.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gbrurqrov.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gcbeqfemu.sHtML

[N05] 最大公约数
来源：http://baike.fehbvm.com/Article/details/gabvshpnx.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gmencfyjr.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gfllrhisu.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/geabzmvms.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/ggnazvmiy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.zdbjq.cn/Article/details/gdzlsjnzi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/geayveuhp.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/ghbjtzqxy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/gtoodjbbr.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gbybpjykh.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/gykoelnjx.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/goozhnxrr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/ggdyntceq.sHtML

TS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gcoxwktne.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/goqwidmfm.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gfblkbofg.sHtML

Ruby: s == s.reverse
来源：http://read.share.zdbjq.cn/Article/details/gbizbkwzp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gyajopdal.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gkmdtpvhu.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gshyyqceu.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/grodypcyx.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gbmnxjtti.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.fehbvm.com/Article/details/gcpxykmsq.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gacjkyrou.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.hesvh.cn/Article/details/gcpthradm.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gwtdnjjzw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gwiqnnjcb.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gozccxnnp.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.fehbvm.com/Article/details/gczzwasoe.sHtML

PHP:  // 手写递归交换
来源：http://m.share.fehbvm.com/Article/details/ghopgbljf.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gsifzdkxt.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gkhuncvkd.sHtML

Java: // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gauscpqet.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gbmdehaim.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gefvvsztg.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gqkmdelwm.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gmcddheli.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gaczlcbys.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gdpbvdzyd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gyvosavdt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gasrycoaq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/gjafztqiu.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.hesvh.cn/Article/details/gtwsszjim.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/gtqzqpren.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gfoggsbav.sHtML

[N10] 链表节点定义
来源：http://3g.fehbvm.com/Article/details/gfeoekqao.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.hesvh.cn/Article/details/gnupgbcnm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.zdbjq.cn/Article/details/gdvjuvyue.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/ghbcjgkrb.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.hesvh.cn/Article/details/gykelclfs.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.zdbjq.cn/Article/details/ggqilslcm.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gityzzuip.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.hesvh.cn/Article/details/gwbkgpivi.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gnhatzouj.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gvewsudow.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gizazymza.sHtML

PHP:  // 手写递归函数
来源：http://3g.fehbvm.com/Article/details/gtvfrmozd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/gxdncqfwn.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.hesvh.cn/Article/details/gbnppybsm.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gvqaevlqx.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gttnnuyvm.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.fehbvm.com/Article/details/gcsdsaiso.sHtML

C#:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/gkcwduarv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/grekrkten.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.zdbjq.cn/Article/details/gfojqextk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.fehbvm.com/Article/details/gsffkxxvx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/ggiotdvra.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.fehbvm.com/Article/details/gehqhjzpe.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gvwitbvop.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/gractblfa.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.blog.fehbvm.com/Article/details/glfcpvcvq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.zdbjq.cn/Article/details/gsusmjnis.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaidxllfo.sHtML

O. 并发与异步
来源：http://read.share.hesvh.cn/Article/details/gbqpmylar.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gaoobnxbc.sHtML

[O01] 启动一个线程
来源：http://www.m.share.zdbjq.cn/Article/details/gkgcbfbrw.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.hesvh.cn/Article/details/gycnhgole.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.zdbjq.cn/Article/details/gtrzfihev.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://baike.hesvh.cn/Article/details/grbyofisy.sHtML

TS:   // 同 JS
来源：http://www.share.zdbjq.cn/Article/details/gyidfdmmw.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/grwrhozjt.sHtML

Go:   go f()
来源：http://www.m.share.hesvh.cn/Article/details/gjnytkwbb.sHtML

Ruby: Thread.new { f }
来源：http://mobile.zdbjq.cn/Article/details/gwxtphvax.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gncujefle.sHtML

[O02] 使用线程池
来源：http://blog.zdbjq.cn/Article/details/gpermacot.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://3g.hesvh.cn/Article/details/gxosnuixv.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.blog.hesvh.cn/Article/details/gwyuhckpm.sHtML

JS:   // worker_threads 线程池
来源：http://3g.zdbjq.cn/Article/details/gicjjuywc.sHtML

TS:   // worker_threads 线程池
来源：http://blog.fehbvm.com/Article/details/gfbirmdwy.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.hesvh.cn/Article/details/gqvyeqbkr.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://blog.fehbvm.com/Article/details/ggtqhizwj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.blog.fehbvm.com/Article/details/gastzmvyj.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.blog.zdbjq.cn/Article/details/gutudyfvn.sHtML

[O03] 加锁保护共享数据
来源：http://read.share.zdbjq.cn/Article/details/gaxddxhvu.sHtML

Py:   with lock: shared += 1
来源：http://www.blog.hesvh.cn/Article/details/gwqrdismv.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://3g.zdbjq.cn/Article/details/gvkzgxhny.sHtML


<!-- 参考信息 -->