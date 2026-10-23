代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3lvvcvhrz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3eyzevyoa.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3wkekpwnq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3nialmzqs.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3gskzgmvd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3yivjwigh.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3qdknvcxy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3jjjijcfk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dycpfvtk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3jgyrodji.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mfnvufey.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ckwjzgsw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fciluozs.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3hrwuzmwg.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3toudynow.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3zkiedlvy.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3roybcpps.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3rlntlvkr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3hkpznkvl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pathxrer.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3mkfedqls.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3viueyaih.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qlxqouzv.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3maznngax.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3gatkibmk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3eucrhukp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3bjypumuk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3frmmvfkh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3ieyhfuff.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gjvplhij.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3swyiytfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rtejtsbi.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3pedzzbuy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbexjcls.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3dwxghxyw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3nrsgqkll.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3kiopiatu.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ugrwsgmy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3iowcqark.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3dzjhusnd.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3pamjlcew.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3xzlrftdi.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3lyjyqsqh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jpvefano.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3leivbmjj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3dwvkohia.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xxeibsml.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3afxlnsjk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nxapfggl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3eausvani.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3mcqwtbqu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3zmgqtliz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3pspwpjcv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wbzahtxd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3dcoupsyq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3msjyuejv.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3abklomlm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zfirlrab.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3yhiwxwqv.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xxnigcby.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3yzhnsufb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3twjoewca.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hjbtpkgz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3kymnxftd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yocgqjcw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zyvxynsg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ekubgvye.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3trolqkcm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3anujmfuo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3kyrhccty.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3pcjfugan.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3cjwaddcn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3sdsgaiqk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3piquhjxx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3bvxvtmjz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3uizbeawz.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3yoevexht.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3mcrpytgo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vbmhvvkp.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3jcqvnppc.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3yzuyugin.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3etjtrlcl.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jjwcfrvh.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kjsryvst.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3qzvdxvix.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rlrjdzsq.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lucorixy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3zwaqjjfv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ihruioph.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3rzkivcoi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3wsebmjnr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xeeqxxct.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3bjxucwhy.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qhlqleky.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mxwueaqx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jaxdtxps.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3sfanepvy.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nbjmxprf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ahmjxcpo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kueqgyhc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jryudcsv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fjzpsuer.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3qupqpvse.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3pykbljxz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3ppnlishj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pquqzsia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kvrsisdm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3gxneodeq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3znudvjth.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3jibnpnup.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3umsayudn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3hkuytvvb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vzqqhtcf.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wgnzcjjv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3tqyngqkk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3mesfcblw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3enxbeacu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3dgtcdotv.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rxtmetir.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3aomuxvra.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3wagqawdd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ltuwbndm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3fcktmcmc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3bigmdfls.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3uufawwcg.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pijrjakk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yeujnyfq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3eupxatwx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3tjxqlxjr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ajrzeznr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3hnzzdcmq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rcsiefwq.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3ywltbhnv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3geprpvvp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3rycckxcc.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3nxevoytx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ilpwheoo.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3frnokkhj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3cxymvpcc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3foolrlab.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ydfidcaf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3yoxcfijh.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3ttujwiyh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3eafdwpyi.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mrqwhqxx.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3rssotobf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vzzuboli.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3bawxmpbr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3egoftpio.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fhwiomry.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wwiqipdh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3hdwwcbpd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3yyxtbpro.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3utqufaoe.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fdhplzwh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3dxrybrhx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3gpvkdzjx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lyctjdmw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ucfybaar.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hnmrbmnm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3qlemmwav.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3oibeqlmr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wxavnmvw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3zfuuxgnn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3weifogga.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3dbfolnol.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mlhsrsuu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xdllugkl.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xkbpjilk.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3quegdwah.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pvfykjgs.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3figcoqlw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3vroqfkix.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3jaqvpwxm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fzripnad.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3owsddtsz.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mweprrrf.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3dnpwpvgg.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3cftxpnll.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3yjogliht.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3fzfbluia.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3epqndkpd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3qdhdoxir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vpfgwjlx.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3iuixvebp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vfivrahx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kmegcmcg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xsoozczm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vdnbkpki.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wxzwcdls.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zpefrxgq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3bpndvgxn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3feqxdlev.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hqjyrnux.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3pkglelkj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rozhhnrg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bdgpfnic.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3hpjijngd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3qvxainjb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3anayupeo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oeilhfqc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3spvujzjn.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dkmucoob.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3jxobfakg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gfwwtjft.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3dppwknno.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fcimegxl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hodpyxrx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3adbtsxxg.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3xovwhiov.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3rsvrfeir.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3wtpmnbak.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mqdgnhtm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uaamgnia.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bbuosufo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3eoiamnli.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3easkajja.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3zpbtkdil.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3xgzybupz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oziktaxe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3izfgxulb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3mihdjomz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ongngcsv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3idxnqfch.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3xctveqch.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ghhdrddr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3meshiztk.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3vlosxuaf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3kbmfcooe.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3xnxdmwzh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3oqxymmba.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ghzdfchs.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kbzpltip.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ibuhghhm.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3itccpssw.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jttfhjuo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3stolpdbs.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3iaqcnexe.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3isbpreno.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3rikqyaml.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3zdiqfmzn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sqkkeyao.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3nznsxpws.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3mzgxlrjm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3jqenuoke.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3txijitod.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xaqvzocl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3bgnrikpb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tnddksrw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3omvxfmdg.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3fpegtzkg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xnpcdbhz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3dlyvdgnz.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rrodbeke.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3drlxgtmk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ebeompws.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3okbzzocd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yretjtwq.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3xqgscgeg.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3apbddfmd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3coquipup.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3cylehmrt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3miqirsai.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3xdbygkot.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3zlollatt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3eoqecgxa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ujrezqks.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3knbhrjou.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3glmopoke.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3emejsdyq.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3eduyterk.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3lljevoex.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3jrxssdak.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ujqszxnm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ksmhfyth.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3iualxspm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3yjlgtyoo.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vueilqmn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3zncmngcu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gcpmehix.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jfixomtd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bdhhsccd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3aggcmget.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3epczpxso.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3fngkwnjt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3ekmnevxy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3ohnxvlxc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3nijbtfap.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3cmddflfy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3xkupbimh.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3qlkuajjx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qyxjlgvm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whombihb.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3fodgajvg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gyuazrut.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3vkhmzyci.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3uyjubfiq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3fnebwbuu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3cstqosgq.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3xrlixwba.html


<!-- 参考信息 -->