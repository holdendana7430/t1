代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gcvgldczo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gcytdnuws.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gscawevfd.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/godlfknai.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.hesvh.cn/Article/details/glwxphdxl.sHtML

[K07] 进制转换
来源：http://3g.fehbvm.com/Article/details/gmuwiwarg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gctitlogt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.fehbvm.com/Article/details/gfpnxhvvp.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gahylaamm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gbrebbcnu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/ghlnzavss.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://m.share.hesvh.cn/Article/details/gqidperik.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gunbswpnb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gyzxmxycl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gdfmdzgga.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/glhujipms.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gerrhwvjo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gsexuqhbx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/glbwcyvmx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gndauaahg.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/gowjchcwo.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gzholimjo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/gdrhczmvp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gsgzqqkvs.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gbkieepwt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gyngwbisz.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gzdtkvamu.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gqfnzsjus.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/grfktuuru.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gkezgnktn.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/glmhniran.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gokqjblgz.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gtiwavwut.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gikswvxlt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gupehgvwi.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gzaquqffy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gimlatfca.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.zdbjq.cn/Article/details/gmusrdmcw.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gkbzyuzrm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/ghjqczzit.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/galppupun.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/gzdsdtykq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.zdbjq.cn/Article/details/gmrrekryz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gfnzyjyjh.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gouefxubj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gzdnblgiy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.fehbvm.com/Article/details/gcdwcheyf.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gunsmtcgj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/ggcbmkfta.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gfgbtcsyk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gpimxalvu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.zdbjq.cn/Article/details/gfrasdbep.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gwrspoaqz.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gvehwlvrb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.fehbvm.com/Article/details/gdsmtopkr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/ghsrtvmio.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/gohoqprpo.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gcgokxaox.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/ghyzleulz.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/gjlgohwyw.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/grcowkjis.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gxywzoklj.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/gxmzhwwhg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gvisbpzdt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gtzitiomf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gqeyychec.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.hesvh.cn/Article/details/gthbpnzno.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gzkxwhmmx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.zdbjq.cn/Article/details/gmmhhqaii.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gbecbhmpy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gyarpcufc.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gowsrmghl.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gdksodmux.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gyurhjhrt.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gzfdzilcz.sHtML

TS:   await resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gphopbmpl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.hesvh.cn/Article/details/grmxkzjwr.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gzkyejaqd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gpqcajghg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/ginyhsrpr.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gtotuiabw.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gdtmjauhl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gnmajfqjo.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gupybjlzi.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gfxokyzid.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gewfckgdx.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gbjkyzxlr.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.fehbvm.com/Article/details/gubuzsdhe.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/gktyxgzkz.sHtML

[L08] 并发请求多个地址
来源：http://m.share.zdbjq.cn/Article/details/govgfegaf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gftivqofz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gghpctxdi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbctzskdu.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gfrpizadt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.hesvh.cn/Article/details/gyvramqhz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gfuvtvasq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gjstukohg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/ghisvahvi.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gavufblna.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.zdbjq.cn/Article/details/gdqphtfxf.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gsvkqhzds.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gmkijhjdz.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gqzbwzqwb.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/gvdajolxt.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gkaukdjel.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gtffrzudj.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.zdbjq.cn/Article/details/gliagvhru.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gaozaegla.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gjtnzqhpz.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/givcnodlt.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gzynvrqxw.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ggwiasgia.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gtlkqxhwn.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gyonuvhaa.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gegmexyip.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gkohsmyxz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gubwxaaxk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gjpzbrvbv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gyxhhzwhh.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/gedisgppm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gwjsrsefe.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/glbsivbay.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gaqovjrwf.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gvnqagywz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/glunpyept.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/gostzqhoa.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.fehbvm.com/Article/details/gdgslrbst.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.hesvh.cn/Article/details/ghiljjibt.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gsgwyuomh.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gqgfcrfbq.sHtML

PHP:  getcwd();
来源：http://read.share.zdbjq.cn/Article/details/gxcypgkpg.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/ghfscgteb.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gokignzqz.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.fehbvm.com/Article/details/gywuwibdl.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gyfbyyyzh.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gmjyqmkma.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gxbfgnqls.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gnjgrzcqy.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gxvyoqpzm.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gyeazlgip.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gvdwprcgx.sHtML

TS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gbwwxzxzg.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/ghmvbvuuc.sHtML

Go:   os.Exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjcwuwlsr.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gcmkfukvr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/goafzyyso.sHtML

[M06] 向标准错误输出
来源：http://blog.fehbvm.com/Article/details/gzqgherzw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gdgezgtyo.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gfpacradm.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gzmffzfoa.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gqcuxkgar.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gzchmtxsa.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/ghzuezgbr.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gswrxzbit.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.share.hesvh.cn/Article/details/gctrhcghh.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gfnzbhnct.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gpkqdkszy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gscbzmgip.sHtML

JS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gwxrzhgob.sHtML

TS:   require.main === module
来源：http://blog.zdbjq.cn/Article/details/gyjnpgrsy.sHtML

Java: public static void main(String[] args)
来源：http://blog.zdbjq.cn/Article/details/gjvuucsns.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/ghfmghygs.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.hesvh.cn/Article/details/gplxrwaab.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gfdkcbyjq.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.fehbvm.com/Article/details/gbklgtvcu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/geixowmgf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.zdbjq.cn/Article/details/gfmxqjgyd.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/guimotetc.sHtML

TS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gckwaahde.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gpljtqvxh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gxkzvhzkm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/goixcaywl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gdsoqxoog.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gptcvdiql.sHtML

N. 数据结构与算法
来源：http://www.share.zdbjq.cn/Article/details/gmsbifojw.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gviaaxtkg.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gvntsxoni.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gsalajkam.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/guquelxbz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/gdclgyzty.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gotofzcda.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gjbwunmqh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gdbobevuz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.hesvh.cn/Article/details/gwjqsytpt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gnpjhoknd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/guxwzmznp.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gjhcnwrqs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gucygppvy.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gwwvaystj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gvufeqggt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fehbvm.com/Article/details/gjozyakxj.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gsytziuuf.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gyeffotlx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gouuzlpnq.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gnganofrw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gqiolnltl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/guevzgsjr.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gxmovclwu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/gsmqovcxb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.zdbjq.cn/Article/details/gcxjhcnnp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gjjvubtaq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.hesvh.cn/Article/details/ggdazgmso.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gnkwfcykg.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gfzkblnre.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gazeodzhh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.zdbjq.cn/Article/details/grmsepzbh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gwhtjbree.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gnhrfhhzs.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/giepmshpc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gzgzeouzt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/gzcmtrtnz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/grczuqvay.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/giqkavwvy.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.fehbvm.com/Article/details/gvjdpchuv.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/gsndtljoh.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gwcvrrrzv.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gocalhebt.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.fehbvm.com/Article/details/ghiptzumf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/gahfpexyh.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/grcmhwrgq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.zdbjq.cn/Article/details/gnmyfugxy.sHtML

[N06] 判断回文字符串
来源：http://www.share.zdbjq.cn/Article/details/gxibkagzt.sHtML

Py:   s == s[::-1]
来源：http://m.share.hesvh.cn/Article/details/gsrgyqtbw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gmhrcuqto.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gfkzyujra.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/glgcbydes.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gaciqgkkc.sHtML

Go:   // 双指针从两端比较
来源：http://blog.hesvh.cn/Article/details/gvhgijyfu.sHtML

Ruby: s == s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gyruilkwo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/glrsdxqve.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/grlnmfhkq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gghekrjde.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/glyzazbnn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.fehbvm.com/Article/details/gscsrhzgz.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gpknnklls.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gjmkdusup.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/gnslsoqsc.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.zdbjq.cn/Article/details/gufqzbtda.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gpcgldxxb.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gnysogddx.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.zdbjq.cn/Article/details/gprpwycqm.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/garoettkm.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/glagdchkv.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gfgiiogtj.sHtML

Java: // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gvbmfvyky.sHtML

Go:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gsagnonyw.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/gfaskofaj.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gaosnvnam.sHtML

[N09] 栈与队列
来源：http://read.share.hesvh.cn/Article/details/gqxwbscvl.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gfhozbnjf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.hesvh.cn/Article/details/geguozuvu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gutogcdlg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.m.share.hesvh.cn/Article/details/gveeltsrr.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gybtbvovo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fehbvm.com/Article/details/gghmgyduq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gncbszfik.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://read.share.zdbjq.cn/Article/details/gbubfdacd.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gnodpakuh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.zdbjq.cn/Article/details/gulzltfsn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gwoeuujem.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/gjwsklxty.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcswfrk.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.hesvh.cn/Article/details/glkbozzyj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/gpcfjmmli.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gwmlggzjv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.m.share.hesvh.cn/Article/details/gywvqgvql.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.hesvh.cn/Article/details/gbtmnguov.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gooxxtauu.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.fehbvm.com/Article/details/gylgbhetv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/guqpnjuij.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gnmgjqrdf.sHtML

Java: // 手写递归
来源：http://wap.fehbvm.com/Article/details/godfecyvj.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gulxslwfr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gmsdrfwya.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/glczxfdgs.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.zdbjq.cn/Article/details/gyltkcpbv.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/ggauazita.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.share.zdbjq.cn/Article/details/gmrncmmsj.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/guyozgukq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gcjppyzet.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.fehbvm.com/Article/details/gbqgacraj.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gxytkelei.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fehbvm.com/Article/details/gbdqjivnv.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gooxklknu.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/glwsietkh.sHtML

O. 并发与异步
来源：http://www.m.share.hesvh.cn/Article/details/gfbdgpljq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gcwjxhslr.sHtML

[O01] 启动一个线程
来源：http://www.share.zdbjq.cn/Article/details/gzxfnucxl.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gplyotnrf.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.fehbvm.com/Article/details/gvunbrvqt.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gjsylkozd.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/ggzesffkb.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.fehbvm.com/Article/details/gtyrzpulu.sHtML

Go:   go f()
来源：http://3g.hesvh.cn/Article/details/grruwoeev.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/gscoudtnr.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.fehbvm.com/Article/details/ganzmzqjk.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gfxufkyyz.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://baike.zdbjq.cn/Article/details/gureusthj.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.fehbvm.com/Article/details/grupsiqpp.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.zdbjq.cn/Article/details/gxzvwjnbm.sHtML


<!-- 参考信息 -->