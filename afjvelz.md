代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gqygnpfpx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.zdbjq.cn/Article/details/gnrrmkxpq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/ghbdhhrbc.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gwemrbtno.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gnjxhzpim.sHtML

[K07] 进制转换
来源：http://www.share.fehbvm.com/Article/details/gnuiyrhku.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gtvcvzelo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gjrezuqnb.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gjodmnort.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gbbdibomf.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gqmgquqgx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.zdbjq.cn/Article/details/gpplziyfg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/gwtaxrijo.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/ggqtguiwu.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gkdhcwlcg.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqnteaqls.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gzyrheqtj.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gegihezdw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gjjojsfxw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gqxlxiyqy.sHtML

Go:   encoding/gob
来源：http://mobile.fehbvm.com/Article/details/geynwrkxe.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/grxcmmwbc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/gsxphmthv.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghatkawvp.sHtML

L. 网络请求
来源：http://www.m.share.zdbjq.cn/Article/details/gwytvfgab.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghotuyuad.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gvcttsyej.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.fehbvm.com/Article/details/gydwajegz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gchkhafwu.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gqowdvyjg.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gyziegaya.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.zdbjq.cn/Article/details/gjbajsfvh.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.zdbjq.cn/Article/details/ghnxviaut.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gcovsqhlr.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/geqshcutl.sHtML

[L02] 发送 POST JSON
来源：http://www.share.hesvh.cn/Article/details/gdrfbhiih.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://m.share.zdbjq.cn/Article/details/gwzgwvppa.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gfbcroxdf.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.hesvh.cn/Article/details/gwrwlfpqo.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gphilmovk.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/gxburcwed.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.fehbvm.com/Article/details/gozpklvye.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/gjygxvyyn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gmybwskmb.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gtyuqhztb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/ghsjixzll.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/galpcfiov.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gzirvzcoh.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gtjzcahdd.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/gqhkygusm.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/ghtloxddm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/gfbwggixs.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/gskxqkjfv.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gbqpnngzc.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gqlgedkbx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.hesvh.cn/Article/details/gmqwtcgxt.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gvieqevvd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.zdbjq.cn/Article/details/gpwmbmgxi.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gxwkyotgi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gwolqrjfr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gewoymqxu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.zdbjq.cn/Article/details/gwryeeums.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gmnmngibl.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/grljrvspr.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.zdbjq.cn/Article/details/glddwkcea.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/gefiarzdj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gsxhkymiw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gdnlvheui.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gmeaeyhhk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gbfkaqsmz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gxffhrpji.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gbeqvymfv.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gunxcmvbt.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gxxbvlmbt.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gdesgails.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gzlerzzcr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gdbtmlhfv.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.zdbjq.cn/Article/details/ggogwfujh.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gilelfpgp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gxjzekkvh.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/grtdsfcat.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.fehbvm.com/Article/details/ggwbxrtiy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gpdpbpirp.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/greihqveq.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gpyaxhhhq.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/glkbfcjjw.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gxuuxfxdd.sHtML

Ruby: resp.code.to_i
来源：http://wap.hesvh.cn/Article/details/grwlqyuod.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gukhwrqkt.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/giuehyijq.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/gpftkjahl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/genysxmem.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/giooifxvi.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbcjvqzyv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gcsjcntku.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gubkvngtj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.hesvh.cn/Article/details/glgbnwbxk.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gxsselixo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gxwhicznu.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gjrhvhvqz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpyvxuqkx.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gbrkmunzu.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/gatyhfloe.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gdrflbkpk.sHtML

JS:   process.argv.slice(2)
来源：http://wap.hesvh.cn/Article/details/gmijfohwi.sHtML

TS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/ghbcjuryn.sHtML

Java: args 数组（main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gdkceticx.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/ggcrduqkc.sHtML

Ruby: ARGV
来源：http://baike.fehbvm.com/Article/details/gmbsnndwu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gbnzdusug.sHtML

[M02] 读取环境变量
来源：http://www.share.fehbvm.com/Article/details/gdlltjeki.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gwzmqdgkt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wap.fehbvm.com/Article/details/grbcnrbrj.sHtML

JS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gkgzaqlob.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gihtkxvle.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/ghmqoxzfj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gjuclbaxk.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/giyhiibcx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/glifrydnk.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gkzpaylcd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gjutncwys.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gobfxudxr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/glflmzbdg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gfsqeizgv.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gpkkowaop.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gppwdiwub.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.hesvh.cn/Article/details/gtruiyswf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.fehbvm.com/Article/details/gvsraxvkh.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/ggrgakycn.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gwezoprrx.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/govyrybmz.sHtML

JS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/geezlkywq.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gdirxtoie.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.zdbjq.cn/Article/details/gmotvdyre.sHtML

Go:   os.Getwd()
来源：http://wap.hesvh.cn/Article/details/gnqjxwciz.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gddaubysf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.fehbvm.com/Article/details/gtzsbvqia.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/geezmyxxm.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gkaznjvzn.sHtML

PHP:  exit(1);
来源：http://3g.fehbvm.com/Article/details/ghynyildw.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gpebeoksd.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/guzimgjzs.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/glhhkxcgr.sHtML

Go:   os.Exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gfevcnstn.sHtML

Ruby: exit 1
来源：http://3g.zdbjq.cn/Article/details/gaibbwlsz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.zdbjq.cn/Article/details/gevbmrrlk.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/guzwgpoww.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/ggevcgdjg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.fehbvm.com/Article/details/gusqfwjzm.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gxyvyjzhe.sHtML

TS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gqvzcuonz.sHtML

Java: System.err.println("err")
来源：http://baike.hesvh.cn/Article/details/gzqfuplkf.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.hesvh.cn/Article/details/ghgdgigjn.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gqewrtmwt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gyajbqdub.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gmfasuobi.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gsruyyqjp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gtuejpmlz.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gadztrrmm.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gxavgnbjj.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fehbvm.com/Article/details/gndxbwbks.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/gaqfceaoi.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gbiehzqgq.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.zdbjq.cn/Article/details/gpnczazvo.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.hesvh.cn/Article/details/gigbhzlue.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gbkbkmmpd.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gwrwybtat.sHtML

JS:   process.platform;  process.version
来源：http://www.share.zdbjq.cn/Article/details/gxtojvcxg.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gjihhjccu.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/goqstjboq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gwcbplfjc.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gjgwzpedw.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.hesvh.cn/Article/details/gsskvgpns.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gksfvagxk.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gnusqjkjy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gvuqjruoi.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gxbhnlkbq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gnnmewlet.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.hesvh.cn/Article/details/glpukqmmt.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gqvmugrru.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.zdbjq.cn/Article/details/gnhtpbuwf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gfiuaxwjq.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gwglrpnbv.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.fehbvm.com/Article/details/gbjgwhoiv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/glnsiwfkv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gzibolgdz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gbfqjcykt.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.zdbjq.cn/Article/details/getdevesx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gqctktncc.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gxumofwtu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gdmculgeu.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.hesvh.cn/Article/details/gtadhgkfg.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gpodqptar.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.zdbjq.cn/Article/details/gglxsbmgr.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gsvlgihiz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://blog.fehbvm.com/Article/details/gnxwuvjoc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.hesvh.cn/Article/details/gyjvbsbbe.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gbepkkqlb.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gpcmxmyyu.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.hesvh.cn/Article/details/gprdgngok.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gceahjwvd.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://baike.zdbjq.cn/Article/details/gnyeklmty.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gdiimrhde.sHtML

[N04] 斐波那契数列
来源：http://www.share.fehbvm.com/Article/details/ghkfyiaxr.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.hesvh.cn/Article/details/giycywjwj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gujxiujhy.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gpqcalevf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gtrkhulck.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.fehbvm.com/Article/details/ghcmuuicz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.fehbvm.com/Article/details/guuuudebi.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/gptkiyrbs.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gelqysqyp.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gktyejurz.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gxmokbrtn.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gkorhjssx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gedoimzvx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.zdbjq.cn/Article/details/gzkkmuygo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/gzppzafoi.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.hesvh.cn/Article/details/gylmjsmrr.sHtML

Ruby: a.gcd(b)
来源：http://www.m.share.zdbjq.cn/Article/details/grabckqnr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gkrgxpmwp.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/girdaykfv.sHtML

Py:   s == s[::-1]
来源：http://m.share.zdbjq.cn/Article/details/gimhxnhie.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gedlsrcqo.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gxiajfxxl.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/getkgbdzx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.fehbvm.com/Article/details/gkyfqsxvh.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gskwwkgve.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gxgfqpjgu.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.hesvh.cn/Article/details/geiskdenm.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gzhxwoato.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gzcvxuumk.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://3g.zdbjq.cn/Article/details/gzkmhllic.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/ghzzrclvd.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/glabplrlz.sHtML

Java: // 手写 HashMap
来源：http://wap.fehbvm.com/Article/details/gcyqwubow.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.hesvh.cn/Article/details/gacnhfqhu.sHtML

Ruby: // 手写 Hash
来源：http://baike.zdbjq.cn/Article/details/ggnxxfbpm.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://baike.fehbvm.com/Article/details/gmyabyysp.sHtML

[N08] 生成全排列
来源：http://wap.fehbvm.com/Article/details/gumodyejl.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.fehbvm.com/Article/details/gyqivziac.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/giqhhiqdf.sHtML

JS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/geisfcrsk.sHtML

TS:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/ggheykvfz.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grmaojzor.sHtML

Go:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/ggckqlzjt.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/guoaqzzum.sHtML

C#:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/guorlixlj.sHtML

[N09] 栈与队列
来源：http://baike.fehbvm.com/Article/details/gzknmdwli.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://read.share.fehbvm.com/Article/details/gshyswrer.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.share.hesvh.cn/Article/details/gegntqyko.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gtsdaljqy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.share.fehbvm.com/Article/details/gkrvgtrqn.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gtnmjzkbx.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://wap.zdbjq.cn/Article/details/genugyvuh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/gmntbcotv.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.zdbjq.cn/Article/details/gouxvnmjj.sHtML

[N10] 链表节点定义
来源：http://www.m.share.hesvh.cn/Article/details/goxswdbay.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/ghebdxctz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/grzgizbmj.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://m.share.hesvh.cn/Article/details/gbmmkervr.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gkwyesiyu.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.fehbvm.com/Article/details/glsxpblzl.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://3g.zdbjq.cn/Article/details/ggiuzrqny.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.fehbvm.com/Article/details/ghfqbmxne.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gynmdehad.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gknfoppzo.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.fehbvm.com/Article/details/gdmntnbpp.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gtagkkqwd.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gryjuonnk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/ghmvavwcf.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/glxclasbq.sHtML

Go:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gwtpoctqb.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.zdbjq.cn/Article/details/ggbacfhbw.sHtML

C#:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/glvltuciu.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://m.share.zdbjq.cn/Article/details/gcmqgofsc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.m.share.fehbvm.com/Article/details/gbwkndsgr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.zdbjq.cn/Article/details/gdxjzgahg.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/ghqegnpar.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gxjstowyk.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gmerfqfbp.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.hesvh.cn/Article/details/glxlqmves.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://baike.zdbjq.cn/Article/details/gxxakhskb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/ghztlaurv.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/ggaommgaz.sHtML

O. 并发与异步
来源：http://baike.fehbvm.com/Article/details/gbanlszny.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gouropipx.sHtML

[O01] 启动一个线程
来源：http://blog.zdbjq.cn/Article/details/gqowwibgx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.blog.hesvh.cn/Article/details/gftvapqlg.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://baike.hesvh.cn/Article/details/grdwtlbgz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.fehbvm.com/Article/details/ggwnrexil.sHtML

TS:   // 同 JS
来源：http://3g.fehbvm.com/Article/details/gufcqdjft.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gvgiioegq.sHtML

Go:   go f()
来源：http://www.blog.fehbvm.com/Article/details/glngtmzgb.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/grlvzylcp.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.hesvh.cn/Article/details/gbwvdhalw.sHtML

[O02] 使用线程池
来源：http://mobile.hesvh.cn/Article/details/gdaewgete.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.share.fehbvm.com/Article/details/glnehoypb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/ghjelkgni.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.hesvh.cn/Article/details/gxfajsitu.sHtML


<!-- 参考信息 -->