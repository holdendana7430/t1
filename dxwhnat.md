代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gkhxwbvww.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gzdpjyxfr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gmorlqvko.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.fehbvm.com/Article/details/geypbehsb.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.hesvh.cn/Article/details/ggrmtdapt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gcsqfogim.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gwjhzdsmi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gduztqkrn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/grqozxjqz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gvyzgklus.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gisnrucqa.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gynfpqlpm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gnhsrnoih.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gfntijrxr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/grykiqjgc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/guefmtmox.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/guhiyxlnc.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gwktwaybr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gyekhqxzg.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gojnpeqlu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gpqcujxjb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/geuxjlgcs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gyvztxiyd.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.zdbjq.cn/Article/details/gcvyehgyn.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gbsoliqgt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gldeysjkm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gzpgmpsgi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.fehbvm.com/Article/details/gsvtlabbn.sHtML

Go:   encoding/gob
来源：http://blog.fehbvm.com/Article/details/gwlwbracy.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gxsejeedf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/glhnuhihh.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gnbffaypq.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gxssxnsvq.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gpmmvkzon.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/ghpoppddv.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.fehbvm.com/Article/details/gntioxdkb.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.hesvh.cn/Article/details/gzdigmhgq.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/golxbuwea.sHtML

TS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gchbslnxx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/ghrxdbggt.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/getdtbpso.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gqwedwvmm.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.zdbjq.cn/Article/details/giowbhaou.sHtML

[L02] 发送 POST JSON
来源：http://3g.fehbvm.com/Article/details/ggequdpys.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gfferhsqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gqhdodgrt.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/ggcxxggft.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gucnlugse.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.hesvh.cn/Article/details/gxtfppdwq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gemvsyhtb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gqvdqkrky.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gxgnmkuhm.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gbafkmzsi.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/grpqjcsin.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gpfyfamhr.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gegbjwrwj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gnnczbcfo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gveowfhdy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/goptszclu.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/ghholscxw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gzmqqbteb.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/grwibfsav.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gnqsztdsx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/guvrqpedk.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gpahfidqf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/grptumirp.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.zdbjq.cn/Article/details/gxixejloj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.zdbjq.cn/Article/details/gddpgrsvb.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.hesvh.cn/Article/details/gwzcptmvv.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gzzgjpacf.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/gllvllzxn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gmclyinpj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://3g.zdbjq.cn/Article/details/gesmrgltv.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gbimqzrsv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gvdkyxnuv.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.fehbvm.com/Article/details/goykdxxsv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.zdbjq.cn/Article/details/gczaqpasu.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gpxsmnahx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/glaxjzczr.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.hesvh.cn/Article/details/gjvshspqg.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/gspgniidp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/gmocscuxz.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gligjnyzb.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gulcgirnz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/glkqjvqey.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/glejaayuc.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gazckdcem.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gclnagrkp.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gyzsrrerq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gtclpbgdk.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.hesvh.cn/Article/details/gstqnrkic.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/glqzuwetv.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gwkmmgcbe.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/goystjypw.sHtML

Go:   resp.StatusCode
来源：http://read.share.hesvh.cn/Article/details/gjzpfjihx.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gvhjydsgz.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gnwbqiryr.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gnqtwcpsx.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gchejcvor.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gzppgntvd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gzleeyfoj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gefbudubc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gujudkbhc.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gptmdfejj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqdjezlsi.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gfxdkymae.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/grtbdrpzi.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/glbxrpjbr.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gevuzwmea.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gfvljbqqk.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gewxftuhi.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gdpfkoehr.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.zdbjq.cn/Article/details/ghnslwxkr.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/ghmfnhkhh.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/gaibqbgtz.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gnumpgfgg.sHtML

Ruby: ARGV
来源：http://m.share.hesvh.cn/Article/details/gcroovzub.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gfwuiahig.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gzrfqjqvj.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gavzjffry.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.fehbvm.com/Article/details/gfvtgcjoc.sHtML

JS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gzmiysujh.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gmnoxladp.sHtML

Java: System.getenv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/ghunbygto.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gigqscsvy.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gvechgmdf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/ghlmzowgj.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/grerfjhfb.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gbedjtowc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.zdbjq.cn/Article/details/grlgczsss.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/grnesefch.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gxcufrgdy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/gumnustbf.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gxhyazsnt.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gyiposziz.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gtnmmeboa.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gutlzgwhe.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gecxhawub.sHtML

PHP:  getcwd();
来源：http://baike.zdbjq.cn/Article/details/gyuwbbjvo.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gummjpsci.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/guyeltdkw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.fehbvm.com/Article/details/gujeekdga.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/glftfehtl.sHtML

Ruby: Dir.pwd
来源：http://m.share.hesvh.cn/Article/details/gsphmnnkd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.hesvh.cn/Article/details/gmmtxywie.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gytttolhe.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gcgekbmdv.sHtML

PHP:  exit(1);
来源：http://wap.zdbjq.cn/Article/details/ghjyonsco.sHtML

JS:   process.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gxzaqfgmo.sHtML

TS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/ggyxciizi.sHtML

Java: System.exit(1)
来源：http://baike.hesvh.cn/Article/details/gosnykowo.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gtjruzbfx.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/ghhuelwtr.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/giauhqjpz.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/gwqkhrgbz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.hesvh.cn/Article/details/gmcyppdpz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.zdbjq.cn/Article/details/gmpagzjsb.sHtML

JS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/gxuqjqliz.sHtML

TS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gkpkoioqo.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/gimzprntf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/ginqikeki.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gpynodagg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.zdbjq.cn/Article/details/ggmjmuoae.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gofqhbokn.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/ghdffyfbz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gndpahyvu.sHtML

JS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gzygvgdsa.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gmqyyedgm.sHtML

Java: public static void main(String[] args)
来源：http://mobile.hesvh.cn/Article/details/gtqoeozhl.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/ghionruaz.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.fehbvm.com/Article/details/gbuedoirq.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/guntuzplm.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gjyjjnekn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/grmdqtegx.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.zdbjq.cn/Article/details/gfnnkigff.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gypafjnwy.sHtML

TS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gudtkazry.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fehbvm.com/Article/details/glzbtjfwa.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.zdbjq.cn/Article/details/gjlwwkmtl.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gctzhgwpj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gjhxhxrhk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggfvzpnpr.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gamixnuzw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gztygzgwl.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.zdbjq.cn/Article/details/gykpdubjk.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.fehbvm.com/Article/details/gyvdgkfuj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gxerapoew.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gygqwdyvw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/grrclhhyu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gfgwocglt.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gdeppfwce.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gnajikwzr.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gnyajksab.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.hesvh.cn/Article/details/gidnwmyje.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gqkvwiqty.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.hesvh.cn/Article/details/gegvwwjjm.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gnmgcvnes.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gepcrkkbs.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.zdbjq.cn/Article/details/gpzfnepwg.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.hesvh.cn/Article/details/gxyjmbadw.sHtML

Ruby: arr.sort
来源：http://wap.hesvh.cn/Article/details/gfbktvufb.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.zdbjq.cn/Article/details/gnmhoobeu.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/glvajckdg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.fehbvm.com/Article/details/gmoaqookk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gduvmxdul.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/glzkdpopq.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gzecncymk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/gerylphwy.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gvbnehcgo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gysajynmh.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.zdbjq.cn/Article/details/gylslaqzp.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/ghqsxfpdz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gibpjifyz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gyrfgtggj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gdxfgwqgl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/grtunnqjf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/geobivbgd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gafkknewk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gztaghiww.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.fehbvm.com/Article/details/gpldftkpp.sHtML

[N05] 最大公约数
来源：http://www.m.share.zdbjq.cn/Article/details/gczfzeozq.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gpxzvyrle.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/geueczmks.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/guzzopmwi.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gyhbtllgy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gmhzstdsr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.zdbjq.cn/Article/details/gmifnshfm.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.hesvh.cn/Article/details/gncrsdcbs.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.hesvh.cn/Article/details/gdpvsiqlv.sHtML

[N06] 判断回文字符串
来源：http://baike.zdbjq.cn/Article/details/gcuvhizzs.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gpolcuthf.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gtgdaqihs.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gcdcucaga.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gylthnijw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/gxkixojff.sHtML

Go:   // 双指针从两端比较
来源：http://mobile.hesvh.cn/Article/details/grzqnyfec.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/gyxnrwfww.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/guklmboag.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.hesvh.cn/Article/details/grimehumb.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gbqhhlzln.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/ghblyzbuu.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gmbyhgiil.sHtML

TS:   // 手写 Map<string, number>
来源：http://3g.hesvh.cn/Article/details/geqtmsjdp.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gcliepmrc.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gsbigswkk.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/ggslsprlm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.fehbvm.com/Article/details/ggcxghkie.sHtML

[N08] 生成全排列
来源：http://www.blog.hesvh.cn/Article/details/gotzjmaul.sHtML

Py:   itertools.permutations(arr)
来源：http://www.blog.fehbvm.com/Article/details/gzempclyr.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gumcdhkav.sHtML

JS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gesvaekkh.sHtML

TS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzuqaxqux.sHtML

Java: // 手写回溯递归
来源：http://baike.zdbjq.cn/Article/details/gmumwtfsj.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gkbzgxghi.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gsytwljob.sHtML

C#:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gyfgnzsbg.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/gcceszesz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.zdbjq.cn/Article/details/gsttubwmv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/gnkufljdj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gnfyjxyst.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.fehbvm.com/Article/details/gosowoxdk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gaxpqkqbc.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.hesvh.cn/Article/details/giglsltjn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/gpovssejn.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gzzckmgmj.sHtML

[N10] 链表节点定义
来源：http://baike.fehbvm.com/Article/details/gxhwlrkgc.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.m.share.hesvh.cn/Article/details/gxdoflszh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gfkayafep.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.zdbjq.cn/Article/details/glvxnredr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/gvcpgsnhl.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gkdayrejo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gllvtqabr.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gpjlnhoar.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.zdbjq.cn/Article/details/gkljldghp.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.hesvh.cn/Article/details/gdhaueghp.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.zdbjq.cn/Article/details/gitcnegov.sHtML

PHP:  // 手写递归函数
来源：http://www.blog.zdbjq.cn/Article/details/gtfjhlyqj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/ghhugylxa.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/goimxtkkq.sHtML

Java: // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gcmtoatsj.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gwnhpreeb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://mobile.hesvh.cn/Article/details/gcaueaqmf.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gxsogehgb.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gjqqknyjs.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gvfnzvyef.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.fehbvm.com/Article/details/gafrjbuob.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.hesvh.cn/Article/details/gnmsqhlgw.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.fehbvm.com/Article/details/gtokszkyc.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.fehbvm.com/Article/details/ggerspyhi.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.zdbjq.cn/Article/details/gxnphlzdo.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gqigtguey.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.zdbjq.cn/Article/details/ggpfhyveb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gtxwdscnh.sHtML

O. 并发与异步
来源：http://mobile.fehbvm.com/Article/details/ggcifkwyj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/geytgvycz.sHtML

[O01] 启动一个线程
来源：http://blog.hesvh.cn/Article/details/gfjvrhrsg.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://blog.fehbvm.com/Article/details/grlltjzgb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.zdbjq.cn/Article/details/gjbvsfcyq.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://blog.hesvh.cn/Article/details/gjnqjvexn.sHtML

TS:   // 同 JS
来源：http://www.share.fehbvm.com/Article/details/gahnjheya.sHtML


<!-- 参考信息 -->