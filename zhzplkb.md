代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gezqvgkru.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.zdbjq.cn/Article/details/ggewnqhbh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gxuiveleg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.hesvh.cn/Article/details/gcwcqufbd.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gzjhjqfng.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gehnfgomh.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://blog.zdbjq.cn/Article/details/gtzjdxxpn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.fehbvm.com/Article/details/gutukxair.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gcyuxgrep.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/grtgacvws.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gsepwvavx.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gijuywrll.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/goavftcoj.sHtML

[K07] 进制转换
来源：http://m.share.zdbjq.cn/Article/details/gbpjifujg.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/glxknyuhk.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gnhudetrf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gtvstncem.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gkzkmyiff.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gcdmzwciv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gyruompaf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/gqlpdszsi.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gmlnzhnxt.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.fehbvm.com/Article/details/gcccvcemk.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.hesvh.cn/Article/details/gtjnpqnhu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/giuaxngbr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gblkxgepf.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/grqfxeyzv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/ghvmftpor.sHtML

Go:   encoding/gob
来源：http://www.m.share.fehbvm.com/Article/details/guceyxbci.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gdphjxthe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.fehbvm.com/Article/details/gawencpqe.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmgrpqyqe.sHtML

L. 网络请求
来源：http://mobile.fehbvm.com/Article/details/gqtaljzlx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/girgsxbto.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/ggzxbmqst.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gomgybmdc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gaaoorokp.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gncrdtmtf.sHtML

TS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gmrzzpvbe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.hesvh.cn/Article/details/gmtqkrucy.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/guystedbp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gludwebwc.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gmabqwyiz.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gawzxulat.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gmptqptkp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gpyraslvj.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/giqrnbngx.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.fehbvm.com/Article/details/gpelybhaj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gvkyzgbkz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gmpuwjfmb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gyksnfcgb.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.hesvh.cn/Article/details/gwuovdpdp.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gympfkvzs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gmhhlydkx.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gkshmflbi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gelkseydx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gdvmexabd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/ghugstbuq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.fehbvm.com/Article/details/gtipuwcfb.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/ggnrkyiur.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gxawucosp.sHtML

[L04] 设置超时
来源：http://www.m.share.hesvh.cn/Article/details/gnxhgqwen.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/gzutjweir.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://read.share.zdbjq.cn/Article/details/gsysptdyv.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gpijzmdcv.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/glpglhjfd.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/gzsmiiwol.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gfzfkmlnx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/goukoncvl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.hesvh.cn/Article/details/giqkvcpqz.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gwpaeoloq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gevtfifek.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gssxopcdr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.zdbjq.cn/Article/details/gwhtqzpar.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gwgkauaru.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gnwtwaicr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gdkkfdtnt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.fehbvm.com/Article/details/gghgcsjmt.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gqzqroikw.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.hesvh.cn/Article/details/gpzwdlrku.sHtML

Py:   resp.json()
来源：http://blog.hesvh.cn/Article/details/gyzakgxhp.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gcmpvbupw.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gequvkuyv.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gemtvmnbj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/guixtraed.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gsdjttbiq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/gklpgsfsl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fehbvm.com/Article/details/gixeozqcy.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gajkihdhc.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.zdbjq.cn/Article/details/gbftufycw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/greuuqnto.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gjfywwbrc.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/grvmxodjx.sHtML

Java: resp.statusCode()
来源：http://www.blog.zdbjq.cn/Article/details/gvifumbhq.sHtML

Go:   resp.StatusCode
来源：http://baike.zdbjq.cn/Article/details/gvbvjivik.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gpjfyjvrk.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gcaffutrg.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gnoiivdcr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gxrvczouy.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.fehbvm.com/Article/details/gxzyvsctr.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gzoxwfpre.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gwizxobza.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gepijtbwe.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gjydsgcvk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.hesvh.cn/Article/details/gbfphxrul.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gpgiamgep.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqnldlctt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gisddlxtm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gizwxibjq.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gcgtdffbw.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/ghrnxukdv.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.zdbjq.cn/Article/details/gqqwfjvof.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/goihtzsbq.sHtML

TS:   process.argv.slice(2)
来源：http://baike.hesvh.cn/Article/details/gjgelpdrj.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/gpabgqfkw.sHtML

Go:   os.Args[1:]
来源：http://baike.zdbjq.cn/Article/details/gvulappvr.sHtML

Ruby: ARGV
来源：http://3g.fehbvm.com/Article/details/gbltrhnch.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gtaztaoek.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gpfsayqvo.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.hesvh.cn/Article/details/gonjoghhe.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gygxqjbpr.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/gdetdtyse.sHtML

TS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/gcskssoes.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gcynkzoga.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gcjezbofr.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gluwhsoqq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.hesvh.cn/Article/details/gdkgjmxnj.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gcuqupcqs.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gijnwulxr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gkajsninl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gxsdmxlon.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gpnepzlau.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.hesvh.cn/Article/details/glpymosqg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fehbvm.com/Article/details/gurbrecdv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.share.hesvh.cn/Article/details/ghqjzdfyi.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gpnnissfe.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/ghvxpkxwp.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gzxgeejqe.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gdsvaoqsj.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gbqgrqcnp.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gpfeqkmwf.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gjnlccxyu.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gtoxcodnm.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gefdvzrql.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/ggszlbcfo.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gwrajqgvh.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/ghcapezme.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gsifzbvvh.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gmynuquff.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gvwifmcbg.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/gjehxoulo.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gydvjkuzi.sHtML

Ruby: exit 1
来源：http://baike.hesvh.cn/Article/details/giwmoazip.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gsvvvckks.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gcvygxgvi.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gzdcucdxe.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gfmkklcbu.sHtML

JS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/glrrdbljx.sHtML

TS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/glzzzsdre.sHtML

Java: System.err.println("err")
来源：http://read.share.zdbjq.cn/Article/details/giyqdrrem.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.fehbvm.com/Article/details/ghqvbzngp.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/goqxceoii.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gxrkthbng.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gyzwcbaeb.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.hesvh.cn/Article/details/gkzbrkqpt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/gqznnsejq.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gytkqmbkj.sHtML

TS:   require.main === module
来源：http://m.share.fehbvm.com/Article/details/gxrhkogba.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gaxhqukxy.sHtML

Go:   func main()
来源：http://www.share.zdbjq.cn/Article/details/gfdsivcvy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gzqthvqhb.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gpuffnrrm.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gbxuuqjcc.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gbpjiuptl.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gljzmfqwx.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gnvaorejf.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gilhuqioj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gwjbwgihu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/ggxntzpfb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/girkcjpro.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gumhugluf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gebvrqdmu.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gjpbefxuh.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gajcejciw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gkveldqms.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.zdbjq.cn/Article/details/godiitblq.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/gwkqtyoys.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/ggvywasgx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.zdbjq.cn/Article/details/gyfhgiigg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gqwhyxfsu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gnhvoupuy.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.hesvh.cn/Article/details/gxoqurllt.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpnmymefx.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gcfemmrya.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gxsebtcdp.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.hesvh.cn/Article/details/gnnvrtyzj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gajpxuyub.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gbarlfhja.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gpnwutovb.sHtML

Go:   slices.Sort(arr)
来源：http://wap.zdbjq.cn/Article/details/grhqrbprq.sHtML

Ruby: arr.sort
来源：http://read.share.zdbjq.cn/Article/details/grcatpzct.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/giwodvnxg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.hesvh.cn/Article/details/gwlxyqhsn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gkzvnfjea.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.zdbjq.cn/Article/details/gcumybsmg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gwqldjssp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/gaysrinmh.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://3g.fehbvm.com/Article/details/gioctzsiv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.hesvh.cn/Article/details/gnscdzzsd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gmqdzbjsl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gnklqefeq.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/ggclhhjxw.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/ggsuuvscp.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.fehbvm.com/Article/details/gjanvhdgy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gdbpgnoar.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gfvlqbasd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.hesvh.cn/Article/details/gwftfplaa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/gfswbhnch.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/gywkuwizd.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://baike.zdbjq.cn/Article/details/gkqgjaydj.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/ggvrhzuxn.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gplmifsxx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gtnyifsvl.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/ghoyhtqzm.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gmucgupsf.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gmfalkade.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/ginuqxrsq.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gmfsbbiuv.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gtycunhfx.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gfcjlbboc.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gwhewvowp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/grqcbmehi.sHtML

JS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/ghdklcfiw.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gestftler.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/glxjkobvf.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.fehbvm.com/Article/details/gsawbiyxi.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/guhjfhkgf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gnjhlgufo.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.hesvh.cn/Article/details/goyhhpjem.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gljkobwvg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gxmpmvruq.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.zdbjq.cn/Article/details/gcfmfvcks.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gojmryuqf.sHtML

Java: // 手写 HashMap
来源：http://baike.hesvh.cn/Article/details/gmzxjpnxz.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.zdbjq.cn/Article/details/gxzeahnmu.sHtML

Ruby: // 手写 Hash
来源：http://mobile.hesvh.cn/Article/details/garxtalmf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.fehbvm.com/Article/details/gjxvhskjr.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gijtwynvc.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gacwwpnqc.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gsakcwwoy.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gontdvimu.sHtML

TS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gmedlkqkm.sHtML

Java: // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gvwvdbxwi.sHtML

Go:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gpboycfat.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gravcqpbk.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gshzgfuvt.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/gdjosgrjr.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/grecuixok.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gkaiwkjef.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gctoymvou.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.hesvh.cn/Article/details/giiwlzjru.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/ggxokyimh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gavkkgnbx.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.hesvh.cn/Article/details/gzbxrzftt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gzjagistn.sHtML

[N10] 链表节点定义
来源：http://mobile.fehbvm.com/Article/details/gtnbryvzf.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.hesvh.cn/Article/details/gvvrdeqiw.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gosoeddcr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.hesvh.cn/Article/details/gxqilqsqx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gevetpfiw.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gnmmthkjv.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.zdbjq.cn/Article/details/gkfgqgdmc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.fehbvm.com/Article/details/gwhtsokdz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.fehbvm.com/Article/details/gzkquzcdp.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gbayvvtlm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://read.share.zdbjq.cn/Article/details/gzxblrale.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/gxnzkcfra.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gzwzqrfyt.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.zdbjq.cn/Article/details/gmhuhcurh.sHtML

Java: // 手写递归
来源：http://blog.zdbjq.cn/Article/details/gwvalqvvh.sHtML

Go:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gqsvxangw.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gqnflcauc.sHtML

C#:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gilwjrnfv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mobile.hesvh.cn/Article/details/gaotmskdj.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gbqstfyna.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.fehbvm.com/Article/details/gmbxgpjua.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.zdbjq.cn/Article/details/gzrgbhocp.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gmbkdipwt.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/guhmcsorb.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://m.share.zdbjq.cn/Article/details/grvpnszqj.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/guloxqnaq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.fehbvm.com/Article/details/gyicncplr.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glbmabndy.sHtML

O. 并发与异步
来源：http://www.blog.zdbjq.cn/Article/details/gkzvhqmpq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gsmihnoqz.sHtML

[O01] 启动一个线程
来源：http://www.share.hesvh.cn/Article/details/gjtmiwpkq.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/gckmoexpo.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.zdbjq.cn/Article/details/gdkszyzfb.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.m.share.fehbvm.com/Article/details/ghxsoztdq.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/grabpsvpe.sHtML


<!-- 参考信息 -->