代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guvzgwcra.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/glrmyoyjz.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/ghotmdsdk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/giklfkqup.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gyqfjfiki.sHtML

[K07] 进制转换
来源：http://mobile.zdbjq.cn/Article/details/ggdvtqtzn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gybjgtlfm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://m.share.fehbvm.com/Article/details/gsnzvsnxa.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gbhvntztq.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gxdtdnash.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gkuckosjy.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/grqxvrlvt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.fehbvm.com/Article/details/gwongrwnj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gmgvkdkmz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/gzraipyth.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gmhtkqzrw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.hesvh.cn/Article/details/gvrlccuct.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.fehbvm.com/Article/details/gtszqsbmn.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.hesvh.cn/Article/details/gkszqdhhy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/glnbtreed.sHtML

Go:   encoding/gob
来源：http://m.share.zdbjq.cn/Article/details/gdurhhppf.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gksioidzw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mobile.fehbvm.com/Article/details/grauvsvfz.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gchmavqbb.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gwofdjdnc.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghsqzrkob.sHtML

[L01] 发送 GET 请求
来源：http://blog.hesvh.cn/Article/details/gvzndjnex.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gbzxnlhis.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gkavysnqy.sHtML

JS:   await fetch(url)
来源：http://m.share.hesvh.cn/Article/details/gmqcuvuye.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gcyhwzlmc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.hesvh.cn/Article/details/gtboztiyt.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gqljylkqv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gwvnkprhi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gaebeyopn.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gzsgvzrdp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/ghttxstux.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/graobminc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gvringspf.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gsdltdonl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gfxrlzojh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/ggfozhxlp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gtjdstsap.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.hesvh.cn/Article/details/gsyyixzad.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.hesvh.cn/Article/details/gkubnrfni.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.zdbjq.cn/Article/details/ghbjstfdw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/gtwyijowt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mobile.zdbjq.cn/Article/details/gpgalranx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gguzagdbw.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gayjkyzmt.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gdzpqgwwd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.fehbvm.com/Article/details/gembslyjh.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.hesvh.cn/Article/details/gmphierpq.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/ghtcoknpv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/goclabitn.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.zdbjq.cn/Article/details/gmtrcyslf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/grhqfzvlc.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gttbklmfh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gmgydolid.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.fehbvm.com/Article/details/ggbjqrjip.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/gwjnxydor.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gkitlmwfd.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/guhheortj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://baike.zdbjq.cn/Article/details/guysspndx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gnczbmxcr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/grxglraxu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gohfhbnry.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.hesvh.cn/Article/details/glwtjwxmw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gygpqpwht.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.fehbvm.com/Article/details/grkbxfnsv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gbbuqgqqi.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gqapyifoh.sHtML

Py:   resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gqtbfoern.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.fehbvm.com/Article/details/glwbvulrk.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/goqjctmek.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gzwqkupmt.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gutatdbqo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.fehbvm.com/Article/details/gacpjoxwm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.fehbvm.com/Article/details/gyitsvxrx.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gbwvdsedx.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gekzimfxs.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/glfrmllco.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gyykyerii.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gcoencrpf.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gfokftxsv.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gvkrzhwoi.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gsgubqlbe.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gbtpqvodr.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/ggwlemprp.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/guzwwxuhs.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gzkfqkjkd.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gsxqqrmgq.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gdurivrxm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gaiynckhb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.hesvh.cn/Article/details/gocgkegzt.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gegjsrexh.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.hesvh.cn/Article/details/gemzuqlmx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gsurlyctq.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gpxytsaux.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.fehbvm.com/Article/details/gfryxbxka.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/graxtfcal.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gqhmjjyho.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gqfbmoauw.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/grpbwjxlh.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gorhzpfbi.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gpjqecnbo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.zdbjq.cn/Article/details/ggcodvhgm.sHtML

Go:   os.Args[1:]
来源：http://www.blog.fehbvm.com/Article/details/gijlpvcrp.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gdwvtbahn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gflqxaohw.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gmuvrehjf.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.hesvh.cn/Article/details/galqgmjtj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gbwuvdltd.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gldqydzvp.sHtML

TS:   process.env.HOME
来源：http://www.blog.hesvh.cn/Article/details/gjyotlebq.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gjdlprczv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gmkqlhbcj.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gyxnbedhg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/gewkjdpyv.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gawcjfjrx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.fehbvm.com/Article/details/guyjsjrqp.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gtfttjtrl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.hesvh.cn/Article/details/gfirtrkvj.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/glrylnhig.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gqueflfbz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gyjugizop.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gazbnymky.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.zdbjq.cn/Article/details/gmijxagmg.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gbakyfzvb.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gttxblmwr.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/goqbdcpcj.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gwpipmolz.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gpfrzwchy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.fehbvm.com/Article/details/gmodsehtl.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/ghsivhxeq.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gwtdzybel.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gosuqqxxn.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gqiencvyz.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmeawmuov.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gxpimzjas.sHtML

JS:   process.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gtgubrhai.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gxtziqzgl.sHtML

Java: System.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghqgogpty.sHtML

Go:   os.Exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gntrxrzvr.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gwyryjwvb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.hesvh.cn/Article/details/geefymqmx.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gruwkghaq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gpxypxflw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.hesvh.cn/Article/details/gjmwnxhds.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gcxdqamee.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gwyyzijfr.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gszbtdkdf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fehbvm.com/Article/details/gmbnovvdx.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gakgncoko.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.zdbjq.cn/Article/details/gmrdznelv.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gmnfdtzim.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/gsregymqc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.zdbjq.cn/Article/details/gldzbjoqq.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gwdziziki.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gbghagdqy.sHtML

Java: public static void main(String[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gxopicqup.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gqdiidlsb.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gazrgobfx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gsjpsgkvn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/ggdtkmlsa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gedppaidj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.fehbvm.com/Article/details/grpauqmzh.sHtML

JS:   process.platform;  process.version
来源：http://3g.zdbjq.cn/Article/details/gcurdphwj.sHtML

TS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/gpdwzsilx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/giynmwwgh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gcujkezvx.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gkanmwmma.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gtyxapyko.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghktdrwrc.sHtML

N. 数据结构与算法
来源：http://m.share.fehbvm.com/Article/details/gzslvnzzn.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjwiofjml.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/guvjoumep.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjdcixekk.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/grpvmcjoo.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gqttkcaat.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gkttkbhoj.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gplyqkbfi.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/gbwulbqwq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/grzakauek.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gpgqtnlvh.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gmeujtrok.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gvivpcdjw.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.zdbjq.cn/Article/details/grkjdnfmk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gaedrmckv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gcluhmygz.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gpggljdhy.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/guzhuiopv.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gxccbkltu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gyrtrxney.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gvxzrbabp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.blog.hesvh.cn/Article/details/gmqpatvly.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gijxbqzhe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/ghwhzxxci.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gpllvozkw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.fehbvm.com/Article/details/gcgcgmxzz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.zdbjq.cn/Article/details/gnmaeccvt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gkayfynvz.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fehbvm.com/Article/details/gbeiimpih.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gukklkyeu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/gxesdvgou.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.fehbvm.com/Article/details/gmchryyvh.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gxdkwtdpd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gttjrruoj.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gkjlvxnjo.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.hesvh.cn/Article/details/gjkixhyeh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.hesvh.cn/Article/details/geeevolcy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gctwparqa.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/gbylooygk.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gbtusmujg.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gscxwcnzo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gcxnltoxx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.hesvh.cn/Article/details/gvdjplwao.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/ggmwfbnnk.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gnzrxltni.sHtML

Ruby: a.gcd(b)
来源：http://baike.fehbvm.com/Article/details/gdtekazmq.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/gbmfxkjwz.sHtML

[N06] 判断回文字符串
来源：http://wap.zdbjq.cn/Article/details/gwtpoqdvo.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/ggtblohxy.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gfcboybwg.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gvrscgymh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/guwapqptw.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.hesvh.cn/Article/details/gbjqzhxcc.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gdwkltrqi.sHtML

Ruby: s == s.reverse
来源：http://baike.hesvh.cn/Article/details/gdvobxekx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/guddhjjuj.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gejmemsss.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.fehbvm.com/Article/details/glmnhblgk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.fehbvm.com/Article/details/geoakggue.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.zdbjq.cn/Article/details/gwjiylmyu.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/grdgtqblv.sHtML

Java: // 手写 HashMap
来源：http://3g.hesvh.cn/Article/details/gntwilbez.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.hesvh.cn/Article/details/gcxaiaqdq.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gmbohsifl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.hesvh.cn/Article/details/gxpyjwjah.sHtML

[N08] 生成全排列
来源：http://www.m.share.fehbvm.com/Article/details/gbnhvwyix.sHtML

Py:   itertools.permutations(arr)
来源：http://read.share.hesvh.cn/Article/details/gteiaksqi.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.fehbvm.com/Article/details/gspowhein.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gkrjpztal.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/givnbfnrp.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gljizuono.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcitugdlf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gpunbewoy.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gykvtjrml.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gcqtgjqfq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://3g.zdbjq.cn/Article/details/ghffhmkuz.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gyftnkbii.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gmsfocqyr.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fehbvm.com/Article/details/gayzlmcpx.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/ghpbokirr.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.fehbvm.com/Article/details/ghoxqhjal.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gzvhamhjt.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gkekcyagf.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gqxyivtxb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gsmqfuxkh.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.hesvh.cn/Article/details/gnwsampjt.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gosbnxrdq.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/grkrcattm.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/gukfkwtkf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://read.share.fehbvm.com/Article/details/gwyfmwvbh.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://3g.zdbjq.cn/Article/details/gmktjcuiv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gvbxgfeux.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gizhriixx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gsecwpjcm.sHtML

PHP:  // 手写递归函数
来源：http://baike.hesvh.cn/Article/details/giilzsyyg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gpjbruisu.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.hesvh.cn/Article/details/gncbnzkrv.sHtML

Java: // 手写递归
来源：http://wap.hesvh.cn/Article/details/ggpfdqrwy.sHtML

Go:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gzidxuoxx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.zdbjq.cn/Article/details/givszeypt.sHtML

C#:   // 手写递归
来源：http://m.share.hesvh.cn/Article/details/gnruoadke.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.zdbjq.cn/Article/details/gzrtaqmfe.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://blog.zdbjq.cn/Article/details/gpoyuvdpp.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.hesvh.cn/Article/details/gebuapqhd.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/giezykeut.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.fehbvm.com/Article/details/gynmltyaa.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.hesvh.cn/Article/details/goslmapsq.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://blog.hesvh.cn/Article/details/geyibsukw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gixejjfqx.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gsvzeizqn.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfjwcmmrz.sHtML

O. 并发与异步
来源：http://blog.fehbvm.com/Article/details/gxayktokq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gahifuhel.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gonjyhqyf.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://baike.fehbvm.com/Article/details/gruxbkora.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://wap.hesvh.cn/Article/details/griykqgtz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.hesvh.cn/Article/details/gpvxpnyjn.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/gsbtzdlgy.sHtML

Java: new Thread(() -> f()).start()
来源：http://3g.fehbvm.com/Article/details/gxqscwwip.sHtML

Go:   go f()
来源：http://mobile.zdbjq.cn/Article/details/gpktbwjfw.sHtML

Ruby: Thread.new { f }
来源：http://read.share.hesvh.cn/Article/details/genkufque.sHtML

C#:   Task.Run(() => F());
来源：http://wap.zdbjq.cn/Article/details/gcbxqugsz.sHtML

[O02] 使用线程池
来源：http://m.share.zdbjq.cn/Article/details/gxqzvuela.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://blog.hesvh.cn/Article/details/gqrtdczno.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://3g.fehbvm.com/Article/details/gkqucqraz.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fehbvm.com/Article/details/gkymmzvnv.sHtML


<!-- 参考信息 -->