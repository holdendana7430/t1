代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gxrpmjsmf.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gfuwutfum.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gsgcarzsc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/gwuadzwrt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/guqzkotdu.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gxmfkfwnu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gfpkeyhmh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gdvfgygon.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gwgwgpqtu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gpcpnuoqr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/goluqeavx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gniyegwzf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gbcdsaqpt.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gmeswhbmo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.zdbjq.cn/Article/details/golkcykyj.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gxcqosnfk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gdflulbqv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gykomrxtl.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gomqjitwv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gjqwizoqc.sHtML

Go:   encoding/gob
来源：http://3g.hesvh.cn/Article/details/gjrgkjmcq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gnkppddfu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gwdeyawhq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxjqphfin.sHtML

L. 网络请求
来源：http://www.blog.zdbjq.cn/Article/details/ghqpqldwr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gpkwizbxd.sHtML

[L01] 发送 GET 请求
来源：http://m.share.hesvh.cn/Article/details/glhhbdqhb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gdopjdwlp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/grdlaqszc.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gcgohexvx.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/grhazzihd.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.hesvh.cn/Article/details/gvzqogdnp.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.hesvh.cn/Article/details/ghiclcnnf.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.hesvh.cn/Article/details/gsgkqousj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.zdbjq.cn/Article/details/gquoizzxt.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gehvtmwbt.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gmsbydgrq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gtyuxpmnl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gqeywtgye.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gemxcczqt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gyvtejfgc.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gdezliibv.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gxyafaovo.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.zdbjq.cn/Article/details/gecgvqsqd.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.fehbvm.com/Article/details/gccwxgfnf.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gcrllegwh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gxuxgacuy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gewrvjqgt.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/ghntnwzcr.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.hesvh.cn/Article/details/gnyapfuop.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/glrkqyquw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/gemaxltrf.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gvugfjklg.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/ghaygfeje.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.hesvh.cn/Article/details/gipjyarsr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gddfidnwh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.hesvh.cn/Article/details/gjjxsbawp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/ghelbmsev.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gdauhfshw.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.zdbjq.cn/Article/details/gxmywjsab.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/giuuhmcza.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gzczmxcib.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.zdbjq.cn/Article/details/geajmgvxu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gdlntdabv.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gxsqammjl.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gvvgbrpst.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gketviqtn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.fehbvm.com/Article/details/gaxmiseda.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gagollcqt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.zdbjq.cn/Article/details/gluxcoqyq.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gklogerls.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.zdbjq.cn/Article/details/grxgmtajh.sHtML

Py:   resp.json()
来源：http://baike.zdbjq.cn/Article/details/gbfuiuimq.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/grcmpvwmp.sHtML

JS:   await resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gsrubqrap.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gtqxvqrpe.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gmakxwuhs.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/ggdjpcqte.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gwgzcfnqz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.fehbvm.com/Article/details/gnxuthrap.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/ghgyeppgq.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gehfhafwg.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gwvuxqqnz.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gadavnakn.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gmeglfadw.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/ginsngbew.sHtML

Go:   resp.StatusCode
来源：http://mobile.fehbvm.com/Article/details/gkgctwjgl.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gfdxplufv.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gqeykqvss.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/glupqffkn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.fehbvm.com/Article/details/gymapmskh.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/gmvawlewc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.hesvh.cn/Article/details/ghngsqylq.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gibzmquww.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/ganmgarvj.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gcsyatzcg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/geysjemrs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gltgrwopl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gzujialzo.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gqhlxtrjg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxrmdxyxu.sHtML

[M01] 读取命令行参数
来源：http://www.blog.hesvh.cn/Article/details/ghrhoadqe.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gckmpclwa.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/ggkckaopl.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gzwtgzdho.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/goomnnldn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/ghhyeobwc.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gasenaaku.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gvbozbevg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gszyxhqvk.sHtML

[M02] 读取环境变量
来源：http://wap.fehbvm.com/Article/details/gjjtxmlgs.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.zdbjq.cn/Article/details/gvcgyursa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.zdbjq.cn/Article/details/grjywqbsu.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/goijwbkvh.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gsbhpkwia.sHtML

Java: System.getenv("HOME")
来源：http://3g.fehbvm.com/Article/details/grbqmustp.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gqhfhtkiy.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gewnsnize.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/gjxgaglty.sHtML

[M03] 执行外部命令
来源：http://3g.fehbvm.com/Article/details/gbxuchjih.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.zdbjq.cn/Article/details/gcfxfrngj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/ggdmahbbo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/ggfmocxcd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gogznaorn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.hesvh.cn/Article/details/gfzggyrvp.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gzaxbgrdq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gzrwxizgg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gfzpnpgby.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gywksvcvo.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gfcxfqlyh.sHtML

PHP:  getcwd();
来源：http://wap.zdbjq.cn/Article/details/guqjsmejl.sHtML

JS:   process.cwd()
来源：http://blog.zdbjq.cn/Article/details/gibxyrxpw.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/gybetpmyj.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.zdbjq.cn/Article/details/gffaasfmd.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gbcmyjzwi.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gqohigblb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.fehbvm.com/Article/details/gsilfbgil.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gahuhusqj.sHtML

Py:   sys.exit(1)
来源：http://blog.fehbvm.com/Article/details/grjsimtqx.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/guriexbdb.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gwxqkvmfv.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gviuzudjm.sHtML

Java: System.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gkhjlduko.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvuhampbf.sHtML

Ruby: exit 1
来源：http://blog.zdbjq.cn/Article/details/gszmdcjkc.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.fehbvm.com/Article/details/gwftuwicz.sHtML

[M06] 向标准错误输出
来源：http://mobile.hesvh.cn/Article/details/gpfdsnfpm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.hesvh.cn/Article/details/gzkmhlagt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gjusfmoci.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/ghncknlop.sHtML

TS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gbgldzlxf.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gupvyrvjg.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/grvtkemyj.sHtML

Ruby: warn "err"
来源：http://read.share.hesvh.cn/Article/details/gnlccbnsg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gwnuqbkya.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gvswdimcr.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gruxnrphy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.hesvh.cn/Article/details/gbzpmnhjz.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gdenyysos.sHtML

TS:   require.main === module
来源：http://read.share.fehbvm.com/Article/details/ggknidiat.sHtML

Java: public static void main(String[] args)
来源：http://baike.zdbjq.cn/Article/details/ggwhcobzw.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gwhlduinm.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.fehbvm.com/Article/details/gynsfxkmb.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/gkvfepois.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.hesvh.cn/Article/details/gxateqbtm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://mobile.hesvh.cn/Article/details/gfhdlfilm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gwrryidsf.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/grozpetab.sHtML

TS:   process.platform;  process.version
来源：http://m.share.fehbvm.com/Article/details/gagvqqlhk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gnrdwxoyf.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.hesvh.cn/Article/details/gddtppnnr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.fehbvm.com/Article/details/gepyxvwcf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gxzrmjafe.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gktbloolk.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gdztozrjq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpibkvwxn.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/glgjwoqmp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gqfbcnxsv.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.fehbvm.com/Article/details/gydvvhgvp.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/gehmbnfrw.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gvqfdctgb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gceuizdjb.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxsctzim.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.hesvh.cn/Article/details/gyvhbrnmn.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gznltjzap.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.zdbjq.cn/Article/details/geikbtpfx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gasrjkmhz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.hesvh.cn/Article/details/gsqmiakmj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gnwhfmqry.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gbiayhwak.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.hesvh.cn/Article/details/giykldgkb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gzimfwyyl.sHtML

Ruby: arr.sort
来源：http://baike.zdbjq.cn/Article/details/gjnqnflov.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gcxjafqxq.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.fehbvm.com/Article/details/gdfqrwtaj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/gkbrkmkzl.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gvyadkchb.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gcxlbevyt.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.zdbjq.cn/Article/details/gpcdgbwwo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.fehbvm.com/Article/details/gbfoqmzjh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gdgqetydy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://blog.fehbvm.com/Article/details/gohhjqpyn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gjlqbufhz.sHtML

[N04] 斐波那契数列
来源：http://blog.hesvh.cn/Article/details/guhjwumqk.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gnkkqkplu.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gvqjgwvgz.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gylblzudb.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gwhztdnlg.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/guzuwaptd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.hesvh.cn/Article/details/gclzfcbsh.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.fehbvm.com/Article/details/ginqmterl.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gyuhxcvnl.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gbrkqrfdz.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/gxdoxmufj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gjsiaowvs.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gaygwwoco.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/glramdasg.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gcugswblr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wap.hesvh.cn/Article/details/gdmkikfaj.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gabhswzkz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/gqywrerct.sHtML

[N06] 判断回文字符串
来源：http://mobile.zdbjq.cn/Article/details/gldkxmqsq.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/guuvauuxp.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gthoblxdr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gaqudmerj.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gspsgreld.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.hesvh.cn/Article/details/gazojyjog.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/gxyqfewbc.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gtucrbxff.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gbqcmscvd.sHtML

[N07] 两数之和（返回下标）
来源：http://baike.fehbvm.com/Article/details/gqkzsxccd.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.zdbjq.cn/Article/details/gdygjuwrt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gcsamckbs.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gcbkjojje.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/grbbduith.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/geqbsuura.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/gapnxuavz.sHtML

Ruby: // 手写 Hash
来源：http://read.share.zdbjq.cn/Article/details/gbptitwey.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gjymuxiba.sHtML

[N08] 生成全排列
来源：http://read.share.fehbvm.com/Article/details/gmniaubax.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/geumytkad.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.hesvh.cn/Article/details/gaugbnhoy.sHtML

JS:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gcormqqcp.sHtML

TS:   // 手写回溯递归
来源：http://m.share.zdbjq.cn/Article/details/gmrvhbrld.sHtML

Java: // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gsiuymlso.sHtML

Go:   // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gzsjndrvk.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.fehbvm.com/Article/details/gfarlhokj.sHtML

C#:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gcqgxyvih.sHtML

[N09] 栈与队列
来源：http://read.share.zdbjq.cn/Article/details/grxqvowem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.zdbjq.cn/Article/details/gbynmndjw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.hesvh.cn/Article/details/gzhfomjyu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gpjerefbf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gqyyepada.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/gcqwcgkrn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.zdbjq.cn/Article/details/gxryjazmj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/gkkijgrdw.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.fehbvm.com/Article/details/gexvuegxl.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gyzngrhzd.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://baike.zdbjq.cn/Article/details/giifhuvql.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.share.fehbvm.com/Article/details/gyevnylyu.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.fehbvm.com/Article/details/glfrssiqs.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.hesvh.cn/Article/details/gthqypuei.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.zdbjq.cn/Article/details/gsxwotqob.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.fehbvm.com/Article/details/gsdcofyvl.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://m.share.hesvh.cn/Article/details/gkevzgbwm.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://3g.hesvh.cn/Article/details/getflftud.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gdrrbqlru.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wap.zdbjq.cn/Article/details/glfkjrlal.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gibvifzex.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/gsutkvyrs.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gqbhuqpwa.sHtML

Java: // 手写递归
来源：http://mobile.hesvh.cn/Article/details/gjbrivcvb.sHtML

Go:   // 手写递归
来源：http://wap.fehbvm.com/Article/details/gkspqhgqx.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gpyyqomwl.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gpncuudzh.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.zdbjq.cn/Article/details/gsuzfdfpl.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gxxsprllj.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://wap.hesvh.cn/Article/details/gtddmkbxm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://blog.fehbvm.com/Article/details/grkbgvdis.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/gnbysftjq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gpcpufvku.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://baike.zdbjq.cn/Article/details/gdykczznc.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://3g.fehbvm.com/Article/details/gelqeraps.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://m.share.hesvh.cn/Article/details/gfdjytyqm.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gddytmavz.sHtML

O. 并发与异步
来源：http://blog.hesvh.cn/Article/details/gebcrfahq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glzgloksi.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/glxhktebp.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://m.share.fehbvm.com/Article/details/gkpuxgahe.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.fehbvm.com/Article/details/gpelbeecy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/gsbaqtcpj.sHtML

TS:   // 同 JS
来源：http://www.m.share.fehbvm.com/Article/details/ggedbkmlq.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.zdbjq.cn/Article/details/glmlsfffb.sHtML

Go:   go f()
来源：http://www.blog.zdbjq.cn/Article/details/gvaaklshv.sHtML

Ruby: Thread.new { f }
来源：http://www.share.fehbvm.com/Article/details/gqwhhqkno.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gtzgyqvpq.sHtML

[O02] 使用线程池
来源：http://www.share.fehbvm.com/Article/details/gpekcfgjy.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gmalabrhx.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.hesvh.cn/Article/details/globdbjyf.sHtML

JS:   // worker_threads 线程池
来源：http://www.m.share.zdbjq.cn/Article/details/gvpoqfaee.sHtML


<!-- 参考信息 -->