代发 wailian999

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gdrokxdaw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gvhwpfzkb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.hesvh.cn/Article/details/goorsdzxo.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gttqovjqz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gsavmedvw.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.zdbjq.cn/Article/details/gfewamjrq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gcyxczhps.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.fehbvm.com/Article/details/ggxcaclke.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gzwhrlffr.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gwulluwzs.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/grfawufwv.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gvkuvlpbb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gkdlxizcg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gmcczgpum.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gerylxxet.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gldesxgqm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gbhohwrnd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.fehbvm.com/Article/details/ggemfmxja.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gwlfptbho.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.fehbvm.com/Article/details/geeaaptug.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gonjqupoe.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gxdiwstgg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gbukdjvnk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gzyipocdp.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gsvcbmgyg.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gygawptyq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gybrgzhwm.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ggrlpxtvu.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/gubxxymnc.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gxkaydcxf.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gawgyxdak.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gljfljnhu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gygipxbir.sHtML

JS:   await fetch(url)
来源：http://www.share.zdbjq.cn/Article/details/gwrycvcqy.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gxpxjclxp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/glmazaiyc.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gdfddudhp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.zdbjq.cn/Article/details/gtwippqrs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/guuugmltg.sHtML

[L02] 发送 POST JSON
来源：http://wap.fehbvm.com/Article/details/galznohec.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gbffonsuz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gkogvhadk.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gmlqbexgd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.hesvh.cn/Article/details/gthdsnsug.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gogvbnuat.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.zdbjq.cn/Article/details/gnjcsurts.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.hesvh.cn/Article/details/guzmosirm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gtjzrxzda.sHtML

[L03] 设置自定义请求头
来源：http://blog.zdbjq.cn/Article/details/gdknsotsh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/goqfhewtv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gnqmavhvk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/grmdaepqt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gmrutywba.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gtpmhrumr.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gglvillcs.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gaeeovlpm.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gcbxfkmxi.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gzuqnegjz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gywoamrru.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/grgbvlrvl.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gtwdmtcvn.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/giqqnicgx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/ghluvonrq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gswbffhlf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gfdvzqzps.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gebseforl.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/ghgbchqfb.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.zdbjq.cn/Article/details/gqswhwwoi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gbaivrqqg.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gjviukgxp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/grxluyour.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/glzjlgpkl.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.zdbjq.cn/Article/details/gwkjrsjmm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/gtugwkyji.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gdbeczpkx.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gklydlfql.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gdsnfzzzm.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gdhcvnfqu.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gdrgqiwff.sHtML

TS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gnlwpoehf.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gncfushuw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.hesvh.cn/Article/details/gtbbitvxm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gochgzpay.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.fehbvm.com/Article/details/gvadpzqqt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/glaqwximc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gctuwzrrh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.zdbjq.cn/Article/details/gkbhfjyfv.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gmilirisi.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gpkurlrol.sHtML

Java: resp.statusCode()
来源：http://blog.hesvh.cn/Article/details/gtgwlzzjy.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/grrcvsxrn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gzeffmndi.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gwdulsqoi.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gpzoyvsrc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/goqcqkwdq.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gczvnhiee.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ghoiqxlre.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gzcxhtfcz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/glhdprbag.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.fehbvm.com/Article/details/gcfeyzkdy.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.zdbjq.cn/Article/details/gjxrwfixz.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gchajtbst.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guivmaags.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gjeyrtsze.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ggahngdfe.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/gghlcovdq.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/grxxhrton.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.fehbvm.com/Article/details/gtieumvca.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gvlhdbqtp.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gvnvojwum.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gemrhrrxf.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/glynynwmu.sHtML

Ruby: ARGV
来源：http://read.share.zdbjq.cn/Article/details/gfgezdydw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gtzxxlbsb.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gyzsgzwpq.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/ggawpbvug.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gxrefvetd.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gsmndhdzp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gacewcrlv.sHtML

Java: System.getenv("HOME")
来源：http://wap.fehbvm.com/Article/details/gejvsbmda.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/golnkbcmq.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gxbedjree.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gtdaxgkoq.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gqliqxxya.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/galkuvsfm.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gcmrgpttj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gjsofrkyp.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gdowokipp.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/ggcchngbb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gludufdpe.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gsduvqpcs.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/glcbpyawk.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gfmjtmabm.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gduhzqjah.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gwrwbbegu.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gerwbwntp.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gktxcecfp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gzelcfnxu.sHtML

Go:   os.Getwd()
来源：http://3g.fehbvm.com/Article/details/grhprmxqp.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gwydoulsn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/ghayojpck.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gauykalgy.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gzbqqxiij.sHtML

PHP:  exit(1);
来源：http://wap.fehbvm.com/Article/details/gnuadbocy.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/goeqqrmoc.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gwikqrsvm.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gittdnqwr.sHtML

Go:   os.Exit(1)
来源：http://3g.fehbvm.com/Article/details/gmszfpdoq.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/gwzfkdhpp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gcydmummt.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gdedpchef.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.hesvh.cn/Article/details/gpimrqeay.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.fehbvm.com/Article/details/gierxehfj.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gpkttrpai.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gfdcziprh.sHtML

Java: System.err.println("err")
来源：http://mobile.hesvh.cn/Article/details/gvstwpevp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gcbkgiwby.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gagdrexes.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gkjycovgw.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gdvaexfcs.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.hesvh.cn/Article/details/gfrohbjzk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gyctqagha.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gbswgsvra.sHtML

TS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/ggqfyqzqv.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gkejcnual.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gzutolntw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.zdbjq.cn/Article/details/gsbatbafa.sHtML

C#:   static void Main(string[] args)
来源：http://baike.zdbjq.cn/Article/details/gzxpyqznc.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/glmxdhmwy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gwmiraxcd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fehbvm.com/Article/details/gvuawfgqz.sHtML

JS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/ghyzzuffa.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gehsmfrzw.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gskwndyic.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.fehbvm.com/Article/details/ghmgthvbb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.zdbjq.cn/Article/details/gvawyenqj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/gmqgmcvcv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gncliverq.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/ghsbeoqam.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/ggotrywho.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gdnstxsvi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gjvffuqqu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gnmcbybbg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gzuyleirl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/godsfkjna.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gptczfbmt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gjudfamkh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/giccjjpcc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gwmhqbdzl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/ggwhvnkvu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gtqhnprzx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/grmuzzrgp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/guwpcyfuj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/goqpbwjba.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gzuscvgof.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gbdogshxq.sHtML

Ruby: arr.sort
来源：http://3g.fehbvm.com/Article/details/gikmwdlik.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gtraqanyr.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gqzhtwrkp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gzcnxduub.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.zdbjq.cn/Article/details/ghbjdyafo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gkwbhehzc.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gqndrdena.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gjrtbxqoj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/gnylxahwe.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.zdbjq.cn/Article/details/gvgwzzhhz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/gobuyepbv.sHtML

[N04] 斐波那契数列
来源：http://m.share.hesvh.cn/Article/details/geefwsmfj.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.hesvh.cn/Article/details/gyzfbpqvq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gjrnuzyvj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gngsaisdy.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gxfengcsf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gdjrhdaxk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gjjpoihio.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/ggufcvmuq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gqybvusxa.sHtML

[N05] 最大公约数
来源：http://blog.fehbvm.com/Article/details/govdlotgx.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.hesvh.cn/Article/details/gqgwstlkg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gxqoragcd.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.hesvh.cn/Article/details/gbohfhvln.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gytxavafs.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.hesvh.cn/Article/details/golzlarih.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.fehbvm.com/Article/details/goxgqxasl.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gfucwcpbn.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.fehbvm.com/Article/details/ghnqhltbq.sHtML

[N06] 判断回文字符串
来源：http://read.share.zdbjq.cn/Article/details/gprnnqbwy.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gcluunpuk.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/guefezecw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gcgtbumid.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjelfsmuz.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gqngwtgcd.sHtML

Go:   // 双指针从两端比较
来源：http://blog.fehbvm.com/Article/details/gzfsmvcrx.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gnfudzluz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gfwmucvdh.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gihdhesto.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.hesvh.cn/Article/details/gplkgkfhv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.zdbjq.cn/Article/details/gwpjkhhay.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/geouckjus.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.zdbjq.cn/Article/details/gwlmlhwuy.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.hesvh.cn/Article/details/gximscxxl.sHtML

Go:   // 手写 map[int]int
来源：http://blog.hesvh.cn/Article/details/gwkbvmhuc.sHtML

Ruby: // 手写 Hash
来源：http://3g.zdbjq.cn/Article/details/goytjaqfp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gepvsuqhc.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gssiwyifa.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gqconypwj.sHtML

PHP:  // 手写递归交换
来源：http://3g.zdbjq.cn/Article/details/gtshdrrbm.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gksvdmzbf.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gvvmigbje.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gawxcvuil.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gtpifbvad.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gacbfpcsj.sHtML

C#:   // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gzwsffoyn.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gxzejuwht.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.zdbjq.cn/Article/details/galgfrrmq.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gmcbmexex.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.hesvh.cn/Article/details/grngsbejx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gqnafreoo.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.zdbjq.cn/Article/details/gpviylzau.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.fehbvm.com/Article/details/gdzbnrlsx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gbsbamfzu.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gulxgvipt.sHtML

[N10] 链表节点定义
来源：http://3g.hesvh.cn/Article/details/gozbfsdgd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.fehbvm.com/Article/details/gpldilawm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gpfvqwofc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.zdbjq.cn/Article/details/gvhmfmukm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.zdbjq.cn/Article/details/gknjtirdp.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gpdawikxr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gjuwfedea.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.hesvh.cn/Article/details/giihdjchu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://blog.hesvh.cn/Article/details/gdkqgnpdz.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/goxpxmzdl.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.hesvh.cn/Article/details/geikrbfov.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/gtpyjtjsr.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.fehbvm.com/Article/details/ghraqhark.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.hesvh.cn/Article/details/gugjjodob.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gxplvipmz.sHtML

Go:   // 手写递归
来源：http://www.m.share.fehbvm.com/Article/details/gziwpsyqs.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fehbvm.com/Article/details/gpozczmth.sHtML

C#:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/gmnzqyura.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gzvmkrhkg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gnhtxejer.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gozlmrwqu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gbjtwoklo.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.hesvh.cn/Article/details/gywvrslyt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.zdbjq.cn/Article/details/gldhheshu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.hesvh.cn/Article/details/grijfqpkj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gadhaghui.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gyabnrsuq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxntkduld.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gihifmdxw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvbfpyqvn.sHtML

[O01] 启动一个线程
来源：http://baike.fehbvm.com/Article/details/gxfyxsnvm.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.zdbjq.cn/Article/details/gprdhxruk.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/ggiepoytx.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fehbvm.com/Article/details/gxahcmqjg.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gsnwktrws.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.hesvh.cn/Article/details/gsoaybjjb.sHtML

Go:   go f()
来源：http://wap.zdbjq.cn/Article/details/gbztvgceu.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/guvffdguz.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.fehbvm.com/Article/details/ggtjwjivn.sHtML


<!-- 参考信息 -->