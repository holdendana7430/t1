代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/glubdkymy.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gqhaaxfcq.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gztrpmetp.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gewjhxmhr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.fehbvm.com/Article/details/gibpvwxmx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.fehbvm.com/Article/details/gcvzpjzji.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mobile.fehbvm.com/Article/details/gyhcrxmge.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/goolwknft.sHtML

[K06] 解析 URL 查询串
来源：http://blog.fehbvm.com/Article/details/gteromlmc.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gwrpmiawr.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/glkbujjpq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gnzswkxqk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gdjlixeum.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gjwrpadpp.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gjyzdneon.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/glzwphmhg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gaktadgwd.sHtML

[K07] 进制转换
来源：http://read.share.fehbvm.com/Article/details/ghvvtyxsh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gsfrgnsrb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.hesvh.cn/Article/details/gzkmqtsnf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvwvhharr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/grxeolojv.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gnqjdddpe.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/guulbidiy.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gmwjdpfek.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gqkuhouvi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gzxzajyby.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gahhjwwly.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gfhamwgzv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/gdzyxtkqc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gqmmaidsl.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gugstnzdz.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gnnhludki.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.zdbjq.cn/Article/details/gxuxqzdep.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gcjprowkz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/guwvzgxar.sHtML

L. 网络请求
来源：http://www.blog.fehbvm.com/Article/details/gushixkwn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnrjdywzz.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gwjoipcjg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/gnycpbdvy.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.fehbvm.com/Article/details/gnezjdkat.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gkjgatyvg.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gbjzmntip.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.zdbjq.cn/Article/details/gwpkyybfq.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.zdbjq.cn/Article/details/gqmlfmbzc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gezggsqeg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.hesvh.cn/Article/details/gycdwxdys.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gzjnaphkm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.fehbvm.com/Article/details/glfouenot.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gtheuaocm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gvnaseayo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gpdfulpqt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gilybufhk.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.fehbvm.com/Article/details/gqlgfbrii.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gkaxnbgtr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/ghsziuact.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/glnpkiohf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gxjoabkjd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gkvmdvbuu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gkpflmjec.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.hesvh.cn/Article/details/gbskanzrw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.hesvh.cn/Article/details/gzrzamkwv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gblhhqyba.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gyajjhzxk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gikxvkxge.sHtML

[L04] 设置超时
来源：http://baike.fehbvm.com/Article/details/gphajsluz.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/guvlucseu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gxjkudowm.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gthpmqnkd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gbwitukco.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.fehbvm.com/Article/details/gcbbkaybn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/glfktyflk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/gtblfkyic.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gzeosvicv.sHtML

[L05] 上传文件（multipart）
来源：http://blog.fehbvm.com/Article/details/gchjkbhim.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/giofyafxq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.zdbjq.cn/Article/details/gytfgzgrk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/ghtutuggo.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/glvsuvblr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.hesvh.cn/Article/details/gyukqhlse.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.hesvh.cn/Article/details/gipdmwyrn.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.fehbvm.com/Article/details/gublsfbps.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/grpbgkadr.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gtsvqaybp.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gdwgfhsbe.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gmkqqquvc.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gqrbwlwxi.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gmtjdcbhk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gdyyfercf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.zdbjq.cn/Article/details/gsmgmydtk.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gyiiatrlp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gvxbjnqsk.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gadvtwtdk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gatlzqhih.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gvbyooifh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gdarmkfye.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gigybfbqw.sHtML

Java: resp.statusCode()
来源：http://3g.hesvh.cn/Article/details/gktdpqwom.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gmnczoucz.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gaufomrlu.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gyauytghq.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gfxvekaix.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/grqpzutwn.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gvgscmlzp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.fehbvm.com/Article/details/gqgieatmj.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gkhujvfld.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gdxolbuxr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gjmvjhjci.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gbvdzbrsc.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.fehbvm.com/Article/details/gtkifwjrw.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmgsxqnjo.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fehbvm.com/Article/details/gyhgutcry.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnesdvrpd.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/ghropkyig.sHtML

Py:   sys.argv[1:]
来源：http://wap.hesvh.cn/Article/details/gcblitmfr.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.hesvh.cn/Article/details/ggnzkwqgy.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.hesvh.cn/Article/details/gftkruzfs.sHtML

TS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gkrdenyeo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/grokerpgz.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gpeyyiswj.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gpvpvydeh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/ggovfnumc.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gzltodkya.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/gylyqxgfx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.fehbvm.com/Article/details/gnekglnbs.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gpivywwer.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/ggigolabd.sHtML

Java: System.getenv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gkdcfvfki.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gikinzfjr.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gtjhwwuyt.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gvhfpdqqe.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/glwfzwgeu.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.hesvh.cn/Article/details/giykfpoji.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.hesvh.cn/Article/details/gizvaxvrf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gaarhymjg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gkdjpylkf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gtrjjvfpt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.fehbvm.com/Article/details/gkwerdixw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.hesvh.cn/Article/details/gncdmjgjx.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/glsnfliic.sHtML

[M04] 获取当前工作目录
来源：http://read.share.hesvh.cn/Article/details/gvaolavmi.sHtML

Py:   os.getcwd()
来源：http://www.share.fehbvm.com/Article/details/gctorahxn.sHtML

PHP:  getcwd();
来源：http://baike.fehbvm.com/Article/details/gmrcarabd.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gvpcqhxfj.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gnaqkufun.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gmznwjkuy.sHtML

Go:   os.Getwd()
来源：http://blog.hesvh.cn/Article/details/giinuxuwp.sHtML

Ruby: Dir.pwd
来源：http://wap.fehbvm.com/Article/details/gudbodxme.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gxkflcbpo.sHtML

[M05] 设置退出码
来源：http://www.share.fehbvm.com/Article/details/gdxzzcmwb.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gxwhzzjwk.sHtML

PHP:  exit(1);
来源：http://blog.hesvh.cn/Article/details/giydlcmwp.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ggkvbtzky.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gqeqogbum.sHtML

Java: System.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gjtaogrxl.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/geaspjrxj.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gaquztgqi.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.fehbvm.com/Article/details/gkykgkbht.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gtryrtmlp.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gplmndvbk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.hesvh.cn/Article/details/gawtlntjw.sHtML

JS:   console.error("err")
来源：http://www.share.zdbjq.cn/Article/details/gsdfnrwnq.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/guwknevmf.sHtML

Java: System.err.println("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdvrmmyeh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.zdbjq.cn/Article/details/ghtjcdrdc.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gjfwcscjn.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gqwlpbskw.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gaacsjctx.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/gydnzqqil.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gmemhenek.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/grzdqsbhy.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gechdalba.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/goyhzyvte.sHtML

Go:   func main()
来源：http://wap.fehbvm.com/Article/details/gfvyhlwsh.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/giockcbmt.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gvzibbvef.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gtfoxyimo.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gnwohjrrc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gwqvntkjq.sHtML

JS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gwyhnwkcr.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gmrrinnof.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gkkjwwrxl.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.hesvh.cn/Article/details/gszfgslvc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.zdbjq.cn/Article/details/gblhngrbx.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gxztoywiq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/geaazlxna.sHtML

N. 数据结构与算法
来源：http://www.blog.hesvh.cn/Article/details/ghguaddfb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxntjdiqd.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gfquyqjwx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghlabitxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gxlmcxugu.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/ggqmxmeeu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gjkdqnsbv.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gjbcbnibe.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gyjrsqggn.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.fehbvm.com/Article/details/gwtewwhzp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gkganjxnq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/ghcyoyaot.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gqwodtvqa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gwtfqsjff.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gagxohbyr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gebrxehtq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.fehbvm.com/Article/details/gkttirrrm.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.fehbvm.com/Article/details/genhioiyl.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gvvlleahi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.zdbjq.cn/Article/details/gisnocblm.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/gezkwofdt.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gwkxmzypn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.fehbvm.com/Article/details/grfbadqyf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gzwpewppj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gdxkjawcd.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.zdbjq.cn/Article/details/grxepyuim.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.hesvh.cn/Article/details/gbhrnkkwn.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gehnkogrf.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/guorqyqyf.sHtML

[N04] 斐波那契数列
来源：http://mobile.hesvh.cn/Article/details/glhvujkff.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/goqwridoh.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gjprxxyah.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gsgxyospl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gyyjyxcuo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gvnfquavk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.fehbvm.com/Article/details/gkaxhiait.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gznagkvbi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gkjlxsnid.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gnxyiyhqw.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gauujwabo.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.fehbvm.com/Article/details/giygooxtn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/gxihsfbiy.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gwjolstat.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wap.fehbvm.com/Article/details/gvagsgqyx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.zdbjq.cn/Article/details/gjbzjifhl.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gwhjbhudx.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.hesvh.cn/Article/details/gbeunztdd.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gfasqmqvv.sHtML

Py:   s == s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gmtijnpyi.sHtML

PHP:  $s === strrev($s);
来源：http://baike.zdbjq.cn/Article/details/gittcfilg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gcwmciadn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gboqszsst.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.zdbjq.cn/Article/details/grnekpami.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/gemuomanc.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/gtyfdflwl.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gtjyqiqox.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.fehbvm.com/Article/details/gecsdgjwa.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://m.share.fehbvm.com/Article/details/gtivsxhrp.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.fehbvm.com/Article/details/gpltkzgpr.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.zdbjq.cn/Article/details/gkkcddybo.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.hesvh.cn/Article/details/gqyavkmmk.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/grccwxtzw.sHtML

Go:   // 手写 map[int]int
来源：http://read.share.fehbvm.com/Article/details/giqdqhmuv.sHtML

Ruby: // 手写 Hash
来源：http://blog.fehbvm.com/Article/details/gmcqzqbye.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gjqixupoo.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gyzohpzvv.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.hesvh.cn/Article/details/gnqwpenuk.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/goirixbag.sHtML

JS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gjhbasgdy.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gdcgreags.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gboldplhm.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gczybvmhr.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gcwkbxhto.sHtML

C#:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gxvmrieth.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gbhvugcio.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/gzlmplusb.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gtdgcngdv.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/ghacicfmx.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/gpxwicvrq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gxgfsajpx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/grjdhbiur.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/geimzeawk.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.hesvh.cn/Article/details/gqxkaqgyr.sHtML

[N10] 链表节点定义
来源：http://m.share.zdbjq.cn/Article/details/gmflcbpbn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gniiogrxc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.hesvh.cn/Article/details/giktlgnoe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gyaayqwpm.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fehbvm.com/Article/details/gxkikklmm.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gcevsseoa.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://mobile.fehbvm.com/Article/details/gtzmwekiy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.hesvh.cn/Article/details/gcpdtpwgz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gwqmlourv.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/ggcgvuyjo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.hesvh.cn/Article/details/gmxwumhlj.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/guyxxatxp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gqaupggwj.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gzwdktglk.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gttopvqyx.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gmlrfyapr.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.hesvh.cn/Article/details/gohfyotxg.sHtML

C#:   // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gulkypeav.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.fehbvm.com/Article/details/guejiobkw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.zdbjq.cn/Article/details/gimxtzkga.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.hesvh.cn/Article/details/gztqhbgyu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gzzqehidq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.m.share.zdbjq.cn/Article/details/gjzjzbdos.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.zdbjq.cn/Article/details/gycxemnlo.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gxgaotsyx.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gvsgktssm.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ggswclikc.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gsgmaplsm.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/grvinlivy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gytyneovf.sHtML

[O01] 启动一个线程
来源：http://read.share.fehbvm.com/Article/details/gisivvxxn.sHtML


<!-- 参考信息 -->