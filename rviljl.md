代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3rizffzbd.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3udpjtgcs.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qteeqhir.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3svcwydou.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3cbaoyotr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3wwbgtfap.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3hiycbqvg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3sghdnawn.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3zrcxegex.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3oyrhanvm.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3ndshmszh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xicceuzq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3xyxloabg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3goykrqjx.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uhumrcfh.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3cgxgmvqm.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3evrcklov.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3pyfcsugy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3iihhystm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xfkhssnx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3piwpyppd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dfpbfbnn.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3xkoexniu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3mxuyxaos.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3tmgkksic.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3urknlrnl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3iefbydus.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3waydkkds.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3bkvodfom.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ocjuyfum.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dmvivexj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3szvwtfwb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ifffogtp.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3jructpks.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3ctzhunfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lsxajecd.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3pitypjoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gadxcpki.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3pwyyiaij.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vxnpgllv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3vyucnohk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3dwaxkqhx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jfsciwib.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vxhkrzok.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vadzmdko.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3yjxmawwo.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qihdrlhn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3exhemihe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ktzicsey.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kjllmpfm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3jfyaxsww.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3twsecgzu.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3cccnxyar.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3bwpwkigd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3qzfziiya.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3roiyytvz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3qzexcbnq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dmeefnct.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3nmmreddd.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zcufjxxq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3itmnirmo.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3brqdypgg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tjckxfxe.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ltqeuazg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3wthjptjk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3pmxtzlob.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3hbijwunr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3pcobalff.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3jqgtberx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3vdhxhuom.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3blnxwnhm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3owmdrtqe.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3inuvlngl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3jmraiopg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3sqslhxui.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3rfzsadui.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3opxllqox.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3yamivgib.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3zhaurjqz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tjkylefe.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3woagluvm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3zlhluzrd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qlkpuxcr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dtygixru.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3prkofbfc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3uskzmlsa.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vzchyfcd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jammgfor.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lawfhmqu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3mvyypbdi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xlruqoad.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ikmexzxb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3ougzadtk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3xezqrtwx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3bassjqkg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3zbdpylwm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xsvkkvym.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3qwpthjwn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kyvezcqg.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3rggeoawd.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3lrfvhzgv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3hzbkcvzx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3secejpuj.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mmufahac.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3aqzjofjq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ubcugmqa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3nbxfnmke.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3tumgtcji.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3platkkzz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3psydeucu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsbtswbo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vsybjscq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bqfwxiwx.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3euwqzijh.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wctqyios.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3gbyspqpx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3jpurtvek.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3whxjpysy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kmhzzhjn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tgtnugjx.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3ggvrubap.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3khrqznst.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3esvmyuym.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3iqxstfez.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pveyqejp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jwyuomll.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3kiabnaht.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bsnapxtq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3fiqjlmyb.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fhqqufqb.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cwujhzny.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3zvhksart.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wlrdbuqp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mmtldyci.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pytnmgdv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vrcjiarl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3medopobm.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xtciwjro.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3tmmtyigh.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3qjpzwgdl.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ozalplyz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pgdrdkch.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3bezotidb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xeerilqn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3absdfqah.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3kucvzqmq.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xbmtfkyw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3vuzieorj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3tvzpreoj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ozjnkhpx.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kyothusl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3hqndrzyr.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jfurmiqc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3phgerfyh.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3augqalvr.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ddgvekmr.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3oerhwyjn.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3ndjhezsc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jkvbwgya.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3syxnxaxs.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3pdzipacy.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3wrlvdcvd.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sgqpbgct.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3sfpvnsul.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3qyngxlkm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3scdwbosg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3bqxtzcbi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3pfqjgnjj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3llpwllup.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vyvfcczf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vkgmrngb.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qtvzylvq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gdvgxksx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3pzybnnbd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3imdqtpnq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3tcxfwixl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3zandlncb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3btzcsgxu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fcynujye.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3ehbygjne.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mxoofrlf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lkptxggg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3mmvgtner.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3rftegyap.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3fwaquqtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3amgnhkdw.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ejgmxclg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfdgldnm.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tksdsybt.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3igrlvnjt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vebtfkps.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3rrdkmlpv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3eluozetr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vehsjtat.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ljodozwh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dngvjpck.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3dnobnpry.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3sdrehmke.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3vajbncpc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3cvpfsdcc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zfomabao.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3mjqyajvq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3oakjsjec.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3gelnpowc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ljmgkcfu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3nsozqiuf.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3tbrgfpua.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xrsnriop.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dfmeopic.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ozgmopez.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ndzzmpkm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3psgjxeyx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3yunehbys.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3awxsbphy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3vkvcmwvq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3tqbjkveq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ubftuqba.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3ftpmknln.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3grrrqeay.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yuwhaocs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3guuxjjxd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3uupqfinv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3azibbuyd.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3drgdcxbv.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3uagjafic.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3utjvsqlh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sbqwdmil.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3nvlulstl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xsjfeoos.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3rmxzjraf.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3htyljnuc.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3xnwoxcsd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvdhuvgq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ruyyqtmh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3xefihktb.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3jykffdik.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zlpglnqs.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gpftccee.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3uotfbtqi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3dzyjbolb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3hucprnfy.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ueafltpc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3eqkapria.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3aimstcic.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ycczpdln.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3qcswoyuf.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3kqdfwslz.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3tngrssxs.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3yosvbbah.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3ewqbeggo.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3cgjizppi.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3wcfxiajz.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mzpdgurn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3unwcdlyv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3inccdfym.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tprxwsfs.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3uehqbogf.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zcsyqqhj.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3klugqwhv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jtglowby.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3nbqmoacj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xonsyxkl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3vrvjchxz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mhxzuycp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3cwtndity.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vlayfppp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3gqsndxck.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3zdhjxnia.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3pczbhnbd.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3ldcowuro.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3wrxrgutv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3uorqmrch.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3udjdszwc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cntrasrl.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3glffwqwf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3pszaprmg.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3nkuclmgx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mtsvwspp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3jmqluwoz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qwtcytsq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3arvftogl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3itvoncyf.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3mhtsnvqs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3dghmeesp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hkbaipgq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3weeeceap.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3houtdnyr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3znqaubwa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3vetcqfml.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3wiprfckc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3vipzfwxo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3jvojdokn.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uhrasucr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3obmhksof.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3uvpgarmc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3dirodcox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3whlodbqi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nthzslej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yqfumpyy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3hvxrpaco.html


<!-- 参考信息 -->