代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.zdbjq.cn/Article/details/gaoptsdsi.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.hesvh.cn/Article/details/gvdnvioqr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.zdbjq.cn/Article/details/gtcvrmumn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/gcxyefkfi.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.zdbjq.cn/Article/details/grzymagvu.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gnozzaouf.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/ghycqwlbk.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/ggztzzhbg.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gnohnpvzy.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gsbqhtcgv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gecbueefw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/getbwlpks.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gmnhjgwjm.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/gazlhyanz.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gkjmiouco.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.hesvh.cn/Article/details/gbyefoptw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gokbxxhgr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gdfldyuib.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gzgqbktwz.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.zdbjq.cn/Article/details/gfhhuapqp.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.zdbjq.cn/Article/details/gtycozoiu.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ghveyxwlc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.hesvh.cn/Article/details/grcizetxm.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gnexqtbsa.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gngqmoiyi.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gqcjqxcuq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gzraqltle.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gufdtipqw.sHtML

Go:   encoding/gob
来源：http://www.m.share.zdbjq.cn/Article/details/gzbzumooq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gksviklzz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gpmprodpn.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gkhfuaqso.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/glizexbmx.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gezubcgtu.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gzpedrreb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/ghpocutjs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gzcbeiipy.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/grwoymmfz.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/gmwcuvxnr.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gfkfcndhn.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gpgsmavez.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.m.share.zdbjq.cn/Article/details/gwnamokas.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/gbwtrnztk.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gdeubrdye.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/glcmcxhia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/geffaxuxr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gonffhjdn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gkfmchdgq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gcellezup.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gpftucntx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gkfhsnatu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.hesvh.cn/Article/details/gvnyczkwm.sHtML

[L03] 设置自定义请求头
来源：http://blog.fehbvm.com/Article/details/gnnohlbgy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/ggpjsfyki.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gdljrelvd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gokbhuifu.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/guadlnzms.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.fehbvm.com/Article/details/gbmdjcybb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.hesvh.cn/Article/details/goheeuymw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gnpcafmof.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gaytqspfs.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gponyojao.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.zdbjq.cn/Article/details/gnjnxkjep.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/glkmdpxre.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gfqapaerr.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gbjxqyrgg.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gfvzhffda.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.fehbvm.com/Article/details/gwryeokpn.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gdxowwoij.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gqoqtvhcm.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/gcmueqxvo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.fehbvm.com/Article/details/giqqvawyp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/girfutklh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gnukmngeb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/gpfsvkywc.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gchismffy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gwybfazgt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.zdbjq.cn/Article/details/gwnqaagwu.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gfahjjrqy.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gzttrygix.sHtML

Py:   resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/geletzaxv.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.fehbvm.com/Article/details/gkholmuqa.sHtML

JS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gmvoegfsx.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gtlkacqes.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gluxqyioi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.fehbvm.com/Article/details/gbxoccdvo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gzzwmdjae.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gkunpqlfh.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gbgtpwnla.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.zdbjq.cn/Article/details/gxxhqfdys.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.fehbvm.com/Article/details/gaobqdnpb.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gwpencrgx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gathchzud.sHtML

Java: resp.statusCode()
来源：http://blog.fehbvm.com/Article/details/gvwguhxnj.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gvfqspjgq.sHtML

Ruby: resp.code.to_i
来源：http://blog.zdbjq.cn/Article/details/gwsslxxip.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gkqlfsgor.sHtML

[L08] 并发请求多个地址
来源：http://www.m.share.zdbjq.cn/Article/details/gqafnxqlr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gsppcdewp.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.fehbvm.com/Article/details/ghgoqrvxo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gglivxtvd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/glvjststs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gmzkngmhl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/gtergkdfb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gnzwxkszo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gbksavyde.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjewwcfwb.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gqckirkts.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/ghespdjus.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gitverena.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.fehbvm.com/Article/details/gcepkiklv.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gidfoxbpv.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gwcwizbus.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gyqzhqirm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gwiaigotu.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gmhndkazq.sHtML

Ruby: ARGV
来源：http://baike.zdbjq.cn/Article/details/gxjoywtmu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gpolqliko.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gcngjyogs.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gcetbbdmz.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.fehbvm.com/Article/details/gmqncjgdb.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gnpnekokj.sHtML

TS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gktkcfxsp.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gabzsrtjk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gkzggcdkg.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.hesvh.cn/Article/details/gglwkhgyy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfdgyljgd.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/geogmefio.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gdmjnejnx.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/gdwblplja.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gqqrnfqol.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gvcxzghmi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/gqvmzbplx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gcjqcughv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/ghboagmdy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/ghezntyqm.sHtML

[M04] 获取当前工作目录
来源：http://blog.hesvh.cn/Article/details/gynkvuksc.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gutosclwm.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gnoqzrrtq.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gnylcbwdd.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/geihiinev.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gjrozesfh.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gqftecjmq.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/goxhqyfas.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gxdpanerp.sHtML

[M05] 设置退出码
来源：http://www.blog.fehbvm.com/Article/details/gcvjltaml.sHtML

Py:   sys.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gexzysyou.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/galjdmeua.sHtML

JS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gbhzjyump.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gmegfjhcq.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gnxfifrbn.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvirlwanj.sHtML

Ruby: exit 1
来源：http://read.share.zdbjq.cn/Article/details/gnckauyvm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.zdbjq.cn/Article/details/gkwexwwcn.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gljriwvqj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.fehbvm.com/Article/details/giafcyvjq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gwzbubrra.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gdpiirsrf.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gucswuusc.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gtjjqhqsh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gogjqnbte.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gfqcugarf.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/ghwyzspmf.sHtML

[M07] 判断是否为主入口
来源：http://read.share.hesvh.cn/Article/details/gjubggcpd.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.zdbjq.cn/Article/details/gwqsaytwn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.hesvh.cn/Article/details/gldikjmqx.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gcbzvhewq.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gadevbddn.sHtML

Java: public static void main(String[] args)
来源：http://m.share.hesvh.cn/Article/details/gwgffgzie.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/gnklpmrax.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/ghxgjnwlf.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.fehbvm.com/Article/details/gxjtenosa.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gxzhhpetk.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gufgyooag.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gkjqsrmtu.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gvkqukfna.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/geongeqrv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gcgazkjih.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gxalygxtd.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gzvvlqbtk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gcaqahscx.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gjzifdvqd.sHtML

N. 数据结构与算法
来源：http://read.share.hesvh.cn/Article/details/gcmstdjvl.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjufzxjkm.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/grdilvofw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gqunneymw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhforeyt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gjfleuvlo.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gllqnyokx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gxkqrnccx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gbzfbloju.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gciotcmsh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gzybdijes.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/genljpcmu.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gaozmwatj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gyrmvybgz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/ggnqehdxd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/gkeocjvqi.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.fehbvm.com/Article/details/gzoctxyeg.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/gkmfsdmdv.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gflmjrnni.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gvdidmhlg.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gxmfmlctu.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gnchnnmoi.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.zdbjq.cn/Article/details/gfovplxkx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gjoukisak.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.zdbjq.cn/Article/details/gbcgunajq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gkwxogfwu.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.fehbvm.com/Article/details/gvzirbnsw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gegmiqpnl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gzpypadym.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/gbvtdffam.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/gcsotsqzk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gwbdybcts.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gojxbaweq.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gcxxcfrit.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gwndmuztw.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gpeihjdjg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.zdbjq.cn/Article/details/gussgapjd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gblzxkvgm.sHtML

[N05] 最大公约数
来源：http://m.share.fehbvm.com/Article/details/gxrpbuuyb.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gcbjvibkq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.zdbjq.cn/Article/details/gnffmzryw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gcsmzadnt.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gnkqypuch.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.zdbjq.cn/Article/details/glatpercz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.zdbjq.cn/Article/details/gwdzhgkmb.sHtML

Ruby: a.gcd(b)
来源：http://www.share.hesvh.cn/Article/details/gxwvtlrop.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gdlgthuga.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gnvhgibic.sHtML

Py:   s == s[::-1]
来源：http://mobile.hesvh.cn/Article/details/gmzmohslf.sHtML

PHP:  $s === strrev($s);
来源：http://baike.fehbvm.com/Article/details/gahchexjk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gnngxvode.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gwihyaqvl.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/grukgresj.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gzlfhsprt.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gvrzbklwd.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gwsslzius.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/grzamtirb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.hesvh.cn/Article/details/gaexxzsvh.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/ggzuxwrpp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/giphuhdzr.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/ghvbdowac.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/gwdosttqg.sHtML

Go:   // 手写 map[int]int
来源：http://blog.fehbvm.com/Article/details/gpyblsrqu.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/grwmajgkq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gbjhyxmhy.sHtML

[N08] 生成全排列
来源：http://m.share.fehbvm.com/Article/details/gttwpwbxy.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gglcjkmvb.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fehbvm.com/Article/details/gxvrwmzdt.sHtML

JS:   // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gvkikowyk.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/grazpmbev.sHtML

Java: // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkgyjbdua.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gsjtwumvf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gvjzbtzbi.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gkmeslnlk.sHtML

[N09] 栈与队列
来源：http://baike.zdbjq.cn/Article/details/gwgnxqdxw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gckekkhwf.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gjrrvwpyg.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/geajzulvt.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.zdbjq.cn/Article/details/gocvfbvnv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gdvdrawch.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/gyrsvvjve.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gtfxvqcjn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.hesvh.cn/Article/details/gtmdmvnig.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gqkvktoep.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gjogbhksn.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gknendkjd.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.fehbvm.com/Article/details/glrfxtwrz.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://mobile.fehbvm.com/Article/details/gbpyzuaax.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/glsbdqvni.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/gystoymbq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.fehbvm.com/Article/details/gsxecnyzx.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gvbsxvohh.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.fehbvm.com/Article/details/gtqitlemi.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.hesvh.cn/Article/details/garauwmwn.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gapmdlzot.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.zdbjq.cn/Article/details/gtpqriqbx.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.hesvh.cn/Article/details/gigwdxjmk.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gznotepcb.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gxkgbamen.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gslwjxhtf.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gkzmwrfkg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/ggdmhzuut.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.fehbvm.com/Article/details/gpfzpnwql.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gcfpraxek.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.zdbjq.cn/Article/details/gwfzxjzcn.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fehbvm.com/Article/details/gwlfbsltg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/gvzazwzyn.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.hesvh.cn/Article/details/gzpqqtdcg.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.hesvh.cn/Article/details/gbzncvgkx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ghittdsyh.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmahoywvh.sHtML

O. 并发与异步
来源：http://3g.zdbjq.cn/Article/details/gufmfienb.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gtlbygrme.sHtML

[O01] 启动一个线程
来源：http://baike.zdbjq.cn/Article/details/gckedgytd.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.hesvh.cn/Article/details/gzdirmhng.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.hesvh.cn/Article/details/gltryrgbi.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.zdbjq.cn/Article/details/gwdzlsxok.sHtML

TS:   // 同 JS
来源：http://m.share.zdbjq.cn/Article/details/gugswtkuv.sHtML


<!-- 参考信息 -->