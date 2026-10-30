代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwroabygt.sHtML

[K07] 进制转换
来源：http://wap.fanxiaobao.xyz/Article/details/gfubfhfmx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://baike.fanxiaobao.xyz/Article/details/gcptvldgf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fanxiaobao.xyz/Article/details/gxmkwucml.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gduorqybu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fanxiaobao.xyz/Article/details/gobffiyly.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fanxiaobao.xyz/Article/details/gfakxsviq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/giklijeyc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fanxiaobao.xyz/Article/details/gzzyasauc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrkkhecy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzzdgacu.sHtML

Py:   pickle.dumps(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gsptdbfey.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gwewegpfg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxqukrqq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfktmmfzo.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fanxiaobao.xyz/Article/details/ggavncttv.sHtML

Go:   encoding/gob
来源：http://mobile.fanxiaobao.xyz/Article/details/gakftdluw.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fanxiaobao.xyz/Article/details/gllctuwfn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpunbiqs.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gltodxokk.sHtML

L. 网络请求
来源：http://read.share.fanxiaobao.xyz/Article/details/gzazoffyl.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golruwasu.sHtML

[L01] 发送 GET 请求
来源：http://read.share.fanxiaobao.xyz/Article/details/grywdhypz.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.fanxiaobao.xyz/Article/details/ghzhqvekg.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwdfvwnoo.sHtML

JS:   await fetch(url)
来源：http://3g.fanxiaobao.xyz/Article/details/goolggjdb.sHtML

TS:   await fetch(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/grpribkil.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fanxiaobao.xyz/Article/details/gsiedkbmh.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyibqeqw.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnymkgas.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.fanxiaobao.xyz/Article/details/gbvkpixee.sHtML

[L02] 发送 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gxeuppqed.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fanxiaobao.xyz/Article/details/gshclywbi.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fanxiaobao.xyz/Article/details/gazfkvrkn.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fanxiaobao.xyz/Article/details/ginjaivcr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbhugpyl.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.fanxiaobao.xyz/Article/details/gqyjpbqji.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcitorjw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.fanxiaobao.xyz/Article/details/gufmubeic.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwrtkngk.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fanxiaobao.xyz/Article/details/gpssrogiq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmzfzana.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnpnjoot.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fanxiaobao.xyz/Article/details/glkuqelgh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fanxiaobao.xyz/Article/details/grizebvda.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fanxiaobao.xyz/Article/details/gimmwnyyy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fanxiaobao.xyz/Article/details/gzqtjssdi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.fanxiaobao.xyz/Article/details/gwoebfyqv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkpnuqyha.sHtML

[L04] 设置超时
来源：http://www.share.fanxiaobao.xyz/Article/details/gdpftmthu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.fanxiaobao.xyz/Article/details/gwieynaii.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.fanxiaobao.xyz/Article/details/gsmphhjne.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fanxiaobao.xyz/Article/details/gfbiwvjvw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fanxiaobao.xyz/Article/details/grkmigafw.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fanxiaobao.xyz/Article/details/gogubgxho.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyhhsucq.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.fanxiaobao.xyz/Article/details/gurspmhei.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdshivwnu.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fanxiaobao.xyz/Article/details/gopvceepg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fanxiaobao.xyz/Article/details/gklqnaytf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiiyrfzi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fanxiaobao.xyz/Article/details/gygpusmle.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhzhgiqu.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fanxiaobao.xyz/Article/details/gwbprafly.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqeiiqylt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcnwgquj.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gznocwgzm.sHtML

[L06] 解析响应为 JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gxadpkeqm.sHtML

Py:   resp.json()
来源：http://read.share.fanxiaobao.xyz/Article/details/gssjcgwaq.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gesxylvwl.sHtML

JS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/girdbbene.sHtML

TS:   await resp.json()
来源：http://baike.fanxiaobao.xyz/Article/details/gxeeugrbh.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfvmdpqs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxaugfeay.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.fanxiaobao.xyz/Article/details/grwpwsqpg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.fanxiaobao.xyz/Article/details/gyonnpyvt.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gxarjngqd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeybhoyz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fanxiaobao.xyz/Article/details/guqlhvlaj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.fanxiaobao.xyz/Article/details/guttcpdtx.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fanxiaobao.xyz/Article/details/glnqmcesw.sHtML

Java: resp.statusCode()
来源：http://3g.fanxiaobao.xyz/Article/details/gdqhhmpoj.sHtML

Go:   resp.StatusCode
来源：http://3g.fanxiaobao.xyz/Article/details/gsscrsoyn.sHtML

Ruby: resp.code.to_i
来源：http://3g.fanxiaobao.xyz/Article/details/glcbkwwao.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdyrmcwt.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fanxiaobao.xyz/Article/details/grazwzetf.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqrzgomt.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fanxiaobao.xyz/Article/details/grvpbmeww.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fanxiaobao.xyz/Article/details/gwaplomqb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fanxiaobao.xyz/Article/details/gvcnfvbca.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fanxiaobao.xyz/Article/details/guziuqzjb.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.fanxiaobao.xyz/Article/details/gwgyddtlt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqllhnxsh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfmyfzja.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gihlmocsu.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.fanxiaobao.xyz/Article/details/gdtgdpdvq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gxopokyhb.sHtML

[M01] 读取命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gfjzmpjzl.sHtML

Py:   sys.argv[1:]
来源：http://3g.fanxiaobao.xyz/Article/details/gauovafad.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbragcsf.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fanxiaobao.xyz/Article/details/gasqnbosa.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gilbsdisv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcirnfkpg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gouhobanm.sHtML

Ruby: ARGV
来源：http://www.share.fanxiaobao.xyz/Article/details/gmzuuezit.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgaxitys.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumqnsfjl.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzxzecpb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfamzghqv.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmesotsiz.sHtML

TS:   process.env.HOME
来源：http://baike.fanxiaobao.xyz/Article/details/gkksdkqbd.sHtML

Java: System.getenv("HOME")
来源：http://baike.fanxiaobao.xyz/Article/details/gjosdtvbk.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fanxiaobao.xyz/Article/details/glydjduzy.sHtML

Ruby: ENV["HOME"]
来源：http://blog.fanxiaobao.xyz/Article/details/gjimsohql.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fanxiaobao.xyz/Article/details/gwqgfbgvn.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghvsglam.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://m.share.fanxiaobao.xyz/Article/details/gpcvemifn.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fanxiaobao.xyz/Article/details/gpvzbfzfl.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fanxiaobao.xyz/Article/details/gctoyrahv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gjggskwvw.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fanxiaobao.xyz/Article/details/guoxxjmfv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzoygprd.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fanxiaobao.xyz/Article/details/gqndjlmlv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnfdgyip.sHtML

[M04] 获取当前工作目录
来源：http://baike.fanxiaobao.xyz/Article/details/gzcccjgjn.sHtML

Py:   os.getcwd()
来源：http://mobile.fanxiaobao.xyz/Article/details/gupxxjagi.sHtML

PHP:  getcwd();
来源：http://baike.fanxiaobao.xyz/Article/details/galbzbhfb.sHtML

JS:   process.cwd()
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxtccrcm.sHtML

TS:   process.cwd()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhqxqaqo.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgaygggg.sHtML

Go:   os.Getwd()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjqfvfew.sHtML

Ruby: Dir.pwd
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrjrilen.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsbsmalt.sHtML

[M05] 设置退出码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsyybftjy.sHtML

Py:   sys.exit(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnehlnkz.sHtML

PHP:  exit(1);
来源：http://www.share.fanxiaobao.xyz/Article/details/glhmycdpy.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdsyntcip.sHtML

TS:   process.exit(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gsvksjjad.sHtML

Java: System.exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gyqkcvkdo.sHtML

Go:   os.Exit(1)
来源：http://baike.fanxiaobao.xyz/Article/details/glmnxazon.sHtML

Ruby: exit 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxmcouflf.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.share.fanxiaobao.xyz/Article/details/gxrcvtuuo.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohclezyq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmckhvor.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fanxiaobao.xyz/Article/details/gwedsvhdy.sHtML

JS:   console.error("err")
来源：http://3g.fanxiaobao.xyz/Article/details/gpyiwyeuz.sHtML

TS:   console.error("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtculxze.sHtML

Java: System.err.println("err")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzreskgo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkomqfmq.sHtML

Ruby: warn "err"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzuhjonj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fanxiaobao.xyz/Article/details/gccehvlzj.sHtML

[M07] 判断是否为主入口
来源：http://wap.fanxiaobao.xyz/Article/details/gugymxene.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fanxiaobao.xyz/Article/details/gcbskyjsv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fanxiaobao.xyz/Article/details/grzbguorw.sHtML

JS:   require.main === module
来源：http://3g.fanxiaobao.xyz/Article/details/gakoysrgv.sHtML

TS:   require.main === module
来源：http://mobile.fanxiaobao.xyz/Article/details/gicpxxjff.sHtML

Java: public static void main(String[] args)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmhzuwrxo.sHtML

Go:   func main()
来源：http://wap.fanxiaobao.xyz/Article/details/guhtkehwl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fanxiaobao.xyz/Article/details/gvrlrmaxh.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fanxiaobao.xyz/Article/details/ghutswuqo.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fanxiaobao.xyz/Article/details/ghwperijm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqqzeweu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.fanxiaobao.xyz/Article/details/gitchtjxa.sHtML

JS:   process.platform;  process.version
来源：http://3g.fanxiaobao.xyz/Article/details/gyccrwwxf.sHtML

TS:   process.platform;  process.version
来源：http://baike.fanxiaobao.xyz/Article/details/glljymeah.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxodkxium.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fanxiaobao.xyz/Article/details/gimrtmjvj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfqbsdxh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fanxiaobao.xyz/Article/details/gorihgxvp.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbszrirg.sHtML

N. 数据结构与算法
来源：http://read.share.fanxiaobao.xyz/Article/details/govjqvxso.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glgbzxeny.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxbyqali.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmfelbxy.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.fanxiaobao.xyz/Article/details/gtietnoma.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fanxiaobao.xyz/Article/details/gmwgrggct.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgbejsbc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gliljxten.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gplrsqdek.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhtcyqfp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fanxiaobao.xyz/Article/details/geibzdseq.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fanxiaobao.xyz/Article/details/gpbojsgbe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxormibx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gttrjijjg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gququrveh.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fanxiaobao.xyz/Article/details/gmmvzsejt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoimhuow.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcisdfuyr.sHtML

Ruby: arr.sort
来源：http://m.share.fanxiaobao.xyz/Article/details/guyuegnbv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.fanxiaobao.xyz/Article/details/glwxtvdbx.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fanxiaobao.xyz/Article/details/gthfptdty.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fanxiaobao.xyz/Article/details/gueocxmhs.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fanxiaobao.xyz/Article/details/gaoknqfcg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpderdmf.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fanxiaobao.xyz/Article/details/gpymxprct.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzwuosqb.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqhbxugeh.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgjbuzau.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.fanxiaobao.xyz/Article/details/gvuprkxbs.sHtML

[N04] 斐波那契数列
来源：http://wap.fanxiaobao.xyz/Article/details/gtrflwsst.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/glrfodlye.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fanxiaobao.xyz/Article/details/geyjigrfd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcmaffxh.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxrvwhry.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fanxiaobao.xyz/Article/details/glrazwwjh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.fanxiaobao.xyz/Article/details/gqjpjxkdz.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/guzhsudpn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrllcmev.sHtML

[N05] 最大公约数
来源：http://wap.fanxiaobao.xyz/Article/details/ghfxsyajo.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fanxiaobao.xyz/Article/details/gheoisysh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.fanxiaobao.xyz/Article/details/gbpnxwqdk.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fanxiaobao.xyz/Article/details/grobiapqq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fanxiaobao.xyz/Article/details/glctqtybe.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.fanxiaobao.xyz/Article/details/ghazysylf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.fanxiaobao.xyz/Article/details/gmnarmkln.sHtML

Ruby: a.gcd(b)
来源：http://3g.fanxiaobao.xyz/Article/details/gafagatwg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fanxiaobao.xyz/Article/details/grgrhrofi.sHtML

[N06] 判断回文字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gitqlwwdq.sHtML

Py:   s == s[::-1]
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxysufqd.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxydaylnw.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtexknrk.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fanxiaobao.xyz/Article/details/gpmxybwot.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fanxiaobao.xyz/Article/details/golyinazn.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fanxiaobao.xyz/Article/details/gycdzqmmw.sHtML

Ruby: s == s.reverse
来源：http://blog.fanxiaobao.xyz/Article/details/giwipjpfy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.fanxiaobao.xyz/Article/details/gvluuqszz.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fanxiaobao.xyz/Article/details/gvwottuil.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fanxiaobao.xyz/Article/details/gemhcmgge.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.fanxiaobao.xyz/Article/details/glfadirhl.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gczuwdayw.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.fanxiaobao.xyz/Article/details/gctwtrctl.sHtML

Java: // 手写 HashMap
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxnxmdyv.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fanxiaobao.xyz/Article/details/gxchtgolg.sHtML

Ruby: // 手写 Hash
来源：http://3g.fanxiaobao.xyz/Article/details/gfwdmwyvt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvcjrtov.sHtML

[N08] 生成全排列
来源：http://m.share.fanxiaobao.xyz/Article/details/gyizyxshf.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/glvdzoctb.sHtML

PHP:  // 手写递归交换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvmtbkes.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhwlesku.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/ghawjphku.sHtML

Java: // 手写回溯递归
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkouxmey.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjfibcpo.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqexgyva.sHtML

C#:   // 手写回溯递归
来源：http://3g.fanxiaobao.xyz/Article/details/grkiaifup.sHtML

[N09] 栈与队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhzehedz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gqiqmcztd.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.fanxiaobao.xyz/Article/details/gjspidltn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.fanxiaobao.xyz/Article/details/gkthrwnfp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvvuhfpp.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fanxiaobao.xyz/Article/details/ggzsbccow.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.fanxiaobao.xyz/Article/details/godekzwgc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyiuzfoq.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.fanxiaobao.xyz/Article/details/gdahxliab.sHtML

[N10] 链表节点定义
来源：http://m.share.fanxiaobao.xyz/Article/details/ghytznahx.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.fanxiaobao.xyz/Article/details/geacrfyun.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcscfeyhe.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnrabhlg.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fanxiaobao.xyz/Article/details/gqljummut.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gokukgioj.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibeiqfwm.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqzistph.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwbpwbop.sHtML

[N11] 二叉树中序遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gskwatddx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://baike.fanxiaobao.xyz/Article/details/gsykkhwsa.sHtML

PHP:  // 手写递归函数
来源：http://m.share.fanxiaobao.xyz/Article/details/goyvreouj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwtudrujc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fanxiaobao.xyz/Article/details/gpezwhlea.sHtML

Java: // 手写递归
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcuzfjsa.sHtML

Go:   // 手写递归
来源：http://blog.fanxiaobao.xyz/Article/details/gkbsuyqhq.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.share.fanxiaobao.xyz/Article/details/gygvwmvvv.sHtML

C#:   // 手写递归
来源：http://wap.fanxiaobao.xyz/Article/details/gjdpvwukc.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgsybcqn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fanxiaobao.xyz/Article/details/gfvbuxxiz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.fanxiaobao.xyz/Article/details/gesqckzos.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjoqnaoq.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.fanxiaobao.xyz/Article/details/gfwdokxsg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.fanxiaobao.xyz/Article/details/ggkxewchx.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdqcgcrzb.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.fanxiaobao.xyz/Article/details/grlhqjniq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdprgglit.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganqxwhsv.sHtML

O. 并发与异步
来源：http://3g.fanxiaobao.xyz/Article/details/gqzkxzdpm.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbizpvfv.sHtML

[O01] 启动一个线程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerkvpmeb.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.fanxiaobao.xyz/Article/details/gacyggwra.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwyetevw.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlflgkxz.sHtML

TS:   // 同 JS
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzenuzhne.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzhsaaop.sHtML

Go:   go f()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsllnnur.sHtML

Ruby: Thread.new { f }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggxdnzmoz.sHtML

C#:   Task.Run(() => F());
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtkolsin.sHtML

[O02] 使用线程池
来源：http://wap.fanxiaobao.xyz/Article/details/grupwvdsu.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnsuxtic.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://blog.fanxiaobao.xyz/Article/details/gukmkwdza.sHtML

JS:   // worker_threads 线程池
来源：http://baike.fanxiaobao.xyz/Article/details/gppubxkcf.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fanxiaobao.xyz/Article/details/goifzxwsv.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqhkxtpx.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahbkabws.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://wap.fanxiaobao.xyz/Article/details/gznooeyjo.sHtML


<!-- 参考信息 -->