代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gxwrybqje.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gstployxm.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gyldygkge.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gwhxppxdf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.zdbjq.cn/Article/details/grnfqkbfm.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gpslorrcp.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gmuwwpzcg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gxmjyuyml.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gvudawcvv.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gtspkzgxg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gzctzqxmy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gnlhviolc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.fehbvm.com/Article/details/gqfqrpytn.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.fehbvm.com/Article/details/ghkvnmdkh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gwnbgpvxp.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.fehbvm.com/Article/details/gkkkyssjh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.hesvh.cn/Article/details/gxvwlzyax.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gnjekeehx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gwyrxvhyi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gkglhriwn.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gydaevbyf.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.hesvh.cn/Article/details/gsxxsmwum.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gzmrmcdbh.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gabaxfwgq.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/glxbzjdst.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ganzpykga.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gzjdakqah.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/ggmzcopxe.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gqavrsmpe.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gebwqyopq.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gaeozhuho.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gsddfkbfx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gtxuyhodm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/gwwatcouz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.zdbjq.cn/Article/details/gyynzkqlf.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gluutldgr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gnpjwdaob.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.hesvh.cn/Article/details/gvvjsaehd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gsnrddhvt.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/ghrxgpbyl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/ggecghnze.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gxefyhneh.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gvalukiky.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gsurgodtf.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gkshobytk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.fehbvm.com/Article/details/gyuzgkefs.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gtafckawv.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gallbzhpx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gtxrkcvmw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.share.fehbvm.com/Article/details/gflljnsla.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gstsayddg.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/gnohzhfxp.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gxlxmsalr.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/ggqvkdksb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gzemtlmal.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/guaoyxkpa.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gipcbbesj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.hesvh.cn/Article/details/gnepgcgik.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/golomkpdh.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/gyucrqvzc.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.zdbjq.cn/Article/details/gozkmuapj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gzpokhrst.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.zdbjq.cn/Article/details/grskkipzq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://read.share.fehbvm.com/Article/details/gcllhgbqj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/glrxqinpk.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gsnifvgzg.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gfcpkxzcb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/gqdbztjpv.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.fehbvm.com/Article/details/gxyndhmgi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gibsopplj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/glvmxxbdn.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gxxpyckiy.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/guegdycre.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gmomoznhs.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/goqczruus.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/ghscewpoo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gclqgyvxx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/ggobjglys.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/gaiwcewdf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gcqsfagwv.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gwxpqtymf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gaezslafs.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/guxvhbnqs.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gmhgtarnc.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/guexdkzec.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/grgbzujez.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gjoezictb.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.hesvh.cn/Article/details/gytcqdmig.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gasqxkjda.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/grwvpodku.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gpcaeorup.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gjqzjgfpo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gggtazlsi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gkywaurux.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gltapiunw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/gwbgoqlyb.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gvaqvsupr.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wap.zdbjq.cn/Article/details/gzpivkxtl.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxjmtddfr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.fehbvm.com/Article/details/grjzrxlui.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfkahueta.sHtML

[M01] 读取命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gxyaxmvdw.sHtML

Py:   sys.argv[1:]
来源：http://wap.fehbvm.com/Article/details/gdxrhgyyq.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.fehbvm.com/Article/details/gsfqhytat.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gkhthuihb.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gfvixfzbq.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gdnijzdtk.sHtML

Go:   os.Args[1:]
来源：http://wap.zdbjq.cn/Article/details/gczdqxcat.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/guuokgngq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/glhutbjxp.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gbjgnsfao.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gzaaadoen.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gpnhlbsik.sHtML

JS:   process.env.HOME
来源：http://www.share.zdbjq.cn/Article/details/ggnbkqfin.sHtML

TS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ghngxpkfc.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gwpyzhtbg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gthxvziuc.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.hesvh.cn/Article/details/gauzdljkg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.hesvh.cn/Article/details/gtmylumuy.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gwvmmnlpg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/ggqzaubee.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gfjwtieek.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/gwimouhzy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.hesvh.cn/Article/details/geonjjien.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://blog.zdbjq.cn/Article/details/glkcvzvhz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gxtcekuey.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gitpokidl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.blog.hesvh.cn/Article/details/gfooobded.sHtML

[M04] 获取当前工作目录
来源：http://m.share.hesvh.cn/Article/details/gojrwiabe.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gyhsnmnom.sHtML

PHP:  getcwd();
来源：http://www.share.fehbvm.com/Article/details/gyciatnic.sHtML

JS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/glaufqllx.sHtML

TS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/guldfvfcq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.zdbjq.cn/Article/details/gbczxdmrq.sHtML

Go:   os.Getwd()
来源：http://3g.hesvh.cn/Article/details/gksoddhhc.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/gmydfiuwy.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/ghwfhmivi.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gjtxcglnn.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/goekdqvjd.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gnbuwiokb.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/grqqngrny.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gmnodmktf.sHtML

Java: System.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/ghzsqyfuk.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gqyqbsnio.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gokomvmde.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/glrewlvqq.sHtML

[M06] 向标准错误输出
来源：http://wap.zdbjq.cn/Article/details/gdjauwehk.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gtdogkoax.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gtudqaaic.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gfsauhgoa.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gviwromaj.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/grnwuccwu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.hesvh.cn/Article/details/gtswvcdoe.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gnvcuhzny.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gtljbaswq.sHtML

[M07] 判断是否为主入口
来源：http://m.share.zdbjq.cn/Article/details/ggyfkddub.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.fehbvm.com/Article/details/gqviomjqx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/grwjrklrt.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/ghkpexxkc.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gckliwmqc.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/guhxglnhz.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gzizrrzcg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gzvcpvufl.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/gwzsiopux.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.fehbvm.com/Article/details/geuvblsgy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gsagcccqp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/gvzhquyxp.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gjmdxegco.sHtML

TS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gpggpvbwk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/ghymvwtel.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gjhepkuic.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.fehbvm.com/Article/details/ggtojgaaj.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gocwjiave.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glvtwcqys.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/grcntrooy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grlsytckq.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gakdgrric.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gbwolluzf.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gkrcpjllc.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gydtkcpzn.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/guadfypud.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/grdnbxkmu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gsxqnkqwe.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.zdbjq.cn/Article/details/gogdpjdwh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gjjawuubf.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.zdbjq.cn/Article/details/gpqtjwabz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/gpxkildhs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/giinypcnz.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gxwgqjghu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gcxrmwiln.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gzguwsczp.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/ghrklbsmp.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gzczxtcqd.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.fehbvm.com/Article/details/gjhhtxjah.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gykcwcvlp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/gcjoxtrob.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gecxyisqf.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gkkpesjwi.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gzknnoegv.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.fehbvm.com/Article/details/gemcrygtp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.fehbvm.com/Article/details/gsrsqrdbl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gbyweuoxx.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gytyjdbqn.sHtML

[N04] 斐波那契数列
来源：http://wap.hesvh.cn/Article/details/gynyxfinb.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.hesvh.cn/Article/details/getwycgzy.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://m.share.hesvh.cn/Article/details/gzgpanrjz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gxdbzwodx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gqsealbgt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/gojdzguga.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fehbvm.com/Article/details/gepvusrco.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/gljkpoxkv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gyfivagir.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gkenuwuxz.sHtML

Py:   math.gcd(a, b)
来源：http://3g.fehbvm.com/Article/details/gybvmbydk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.zdbjq.cn/Article/details/gsfamfcyj.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gewnzmqpa.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/glvhaojud.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gvefphxus.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fehbvm.com/Article/details/gzapzswns.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/gvancohjo.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.fehbvm.com/Article/details/ghkswqzqx.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gzcihduja.sHtML

Py:   s == s[::-1]
来源：http://read.share.fehbvm.com/Article/details/glhicwmra.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gjdsxdygw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gtsirhrot.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gpogxqaze.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.hesvh.cn/Article/details/gumehcjfi.sHtML

Go:   // 双指针从两端比较
来源：http://blog.zdbjq.cn/Article/details/gtiwoofll.sHtML

Ruby: s == s.reverse
来源：http://m.share.hesvh.cn/Article/details/gmioanlfm.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/gkgnxyqst.sHtML

[N07] 两数之和（返回下标）
来源：http://www.blog.hesvh.cn/Article/details/gwsqgqceh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gugyxvoqb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.hesvh.cn/Article/details/gkkwxzoqe.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gavbqxvrk.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.hesvh.cn/Article/details/ggnkynfzo.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/gevynbgsj.sHtML

Go:   // 手写 map[int]int
来源：http://baike.fehbvm.com/Article/details/gojnrppoh.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gmohtosct.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.fehbvm.com/Article/details/gppewalai.sHtML

[N08] 生成全排列
来源：http://blog.hesvh.cn/Article/details/grxdmhpgj.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/geiwydjej.sHtML

PHP:  // 手写递归交换
来源：http://3g.fehbvm.com/Article/details/ghlzbuyjj.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gaxstwfcw.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gppdmdiql.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gxgdbwmkx.sHtML

Go:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gqtcjhnqw.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.hesvh.cn/Article/details/gpktexeuq.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gzgjslczx.sHtML

[N09] 栈与队列
来源：http://www.blog.hesvh.cn/Article/details/gplwjlewo.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.fehbvm.com/Article/details/guixagcwk.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gjezkwrpr.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.zdbjq.cn/Article/details/ggyqdwiut.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gelpfnnzb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://blog.zdbjq.cn/Article/details/ggayplbsl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gekvzimnq.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gstwdqwfh.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gbrmkkkeo.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gvegnlpbx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/ggrlcqtbx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.hesvh.cn/Article/details/gjtnjhxgs.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gtxhqcvhy.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://read.share.hesvh.cn/Article/details/gqfcvceee.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.hesvh.cn/Article/details/ghniehndr.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/ghxzsukqc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.fehbvm.com/Article/details/gxtlxhlue.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gdlegcflx.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fehbvm.com/Article/details/gcpjnttuh.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.m.share.zdbjq.cn/Article/details/gjroskggm.sHtML

PHP:  // 手写递归函数
来源：http://wap.hesvh.cn/Article/details/gajzceoar.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gnwsbjagb.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gcuepqmjr.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gojvjktej.sHtML

Go:   // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gznjnfzep.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://read.share.fehbvm.com/Article/details/gemragcyd.sHtML

C#:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gzrziqztr.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gaijjjcbw.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://baike.hesvh.cn/Article/details/gqxmzmtts.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gundlawwc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gbpefivjd.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/gsezdpptr.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.fehbvm.com/Article/details/gprofqcui.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.fehbvm.com/Article/details/gbytmykes.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.hesvh.cn/Article/details/gwrobwdnd.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.share.zdbjq.cn/Article/details/gxvfcsmpd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzuvcpwzb.sHtML

O. 并发与异步
来源：http://www.share.hesvh.cn/Article/details/gfmsymiii.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gionubfvw.sHtML

[O01] 启动一个线程
来源：http://www.share.fehbvm.com/Article/details/gswcexlem.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/goacztfsq.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.zdbjq.cn/Article/details/gvenpdvze.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.hesvh.cn/Article/details/gcxcsntay.sHtML

TS:   // 同 JS
来源：http://wap.zdbjq.cn/Article/details/gakomukat.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gfhyfzzij.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gxphivwrz.sHtML

Ruby: Thread.new { f }
来源：http://www.m.share.zdbjq.cn/Article/details/gxyuvmvnd.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/ggncxtgzp.sHtML

[O02] 使用线程池
来源：http://read.share.hesvh.cn/Article/details/gfbojogyh.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/glttdvjum.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.share.fehbvm.com/Article/details/gsesphfar.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fehbvm.com/Article/details/gwrngcazg.sHtML


<!-- 参考信息 -->