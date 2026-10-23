代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3egjmbtfk.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3rkdbbmjr.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3qupkywia.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hdftfota.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3mroshspg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hoyhbkvm.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3mukupobr.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3owonxcaz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3atuhnpje.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3xprvebcd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gqkkinex.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3tsaomxyc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cwmmrreq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3rbfixtep.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3fhbtyzey.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jgxsrgxw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3xberubyf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3cfefvpwj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lohkzvzs.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3szlgwcbk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3aczpjmmk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pfgrjqvs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tauibbuj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3ubhofoxx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3gpbbkbup.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ldfcgbpl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3arocevre.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3egjzhega.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3mmrlukua.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3royccwpx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3rxglwpvn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3aevdehlz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3hitwxvoz.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wmimtqus.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3ichnzbay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdduarfy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3qixnwrad.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xitjdkmk.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3zvulsaot.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3bvzvduwo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3cevjpijb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jiqyfrfz.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwovlfv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3aftgjlwp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3amwadozy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ucbjrfbb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3xzyqwxyp.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lhutpqvm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3grkojaql.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3vqmplylw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ggyqztin.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3btmhlckz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3bghzbysm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3nhqxwqwv.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3zysgrtfq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xcbxlubo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3rqhkatpl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3kxvkuykz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3dvytftad.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3vlzxktop.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3iwefyjpb.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3ankqkjzr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3ljvdosuy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3cqqlfaew.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kynffmhn.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3gfatekma.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3ehjvjchp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3vvxtlnxk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3kahgowke.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xerbmdfi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3spyjpafi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3igqmktmq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3qrepglme.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3zubunomp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3yirukrlt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3nkbdmuxc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nwrbfagv.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3izvkgwdh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ctvmnpdt.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3smoflziw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3owuzmndr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3wbemlgtr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hkdttwfp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3akumorhm.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3tasmvvai.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3xmlgunlc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3eezxsrmb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sdymtgkm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pohkzzqv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3hhvpcibg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3ifdqkpej.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3lijysqqf.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jjemsfve.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3gqhqjfdz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3qhfdesrw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tmnyhxzy.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3xiwdjzhk.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3pvhirwkb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3vpuqejwx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3uquusgxp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3unvtobhm.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3nhbmygfh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3gvqqujip.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qifhhlpj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3yfhqrduv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pdrzfqse.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3fnukyeus.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3onjjfrmr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3mivbukfr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3iyrsyacj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zahfyjjg.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3kgfzucbw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kufadelp.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uwcogequ.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yjintbbm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3iagizjpr.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tzusquwp.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3azvnjizx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3uvtomxhq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3azinhehj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3jvjnakky.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3xujzstrd.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3miqnndso.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zaplvpcn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eikskqxp.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tghcxobu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3mlyhegqn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3srsmnomc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hxlzcffy.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3ihnfvxvt.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3bqpwmxsi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3laywgejq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3rhoebzmr.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3zkvwshrj.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3loxonfnf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rgrnosoj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3uvapbbpo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3upbotczl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3uvvvtwup.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3gkogaumb.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3wcnuiaxx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3vacwdbud.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3sfaxlhur.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3itxbqhmr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3mvnawgpv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3oftauygt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3btdjezsw.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3snfrdycr.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3wbeorgqp.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3idmtnkna.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3dcmfqdlu.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3grftmaqb.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cfkmyypq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3frksrxcx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vwvmlcfi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3igamyfrf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3umusnowa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sezkaqng.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3hldukwdk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3oqpsmlwj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3tmfisuzy.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3luwuawtv.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3coshycqq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3agqpmyeb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3gjlhddwa.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cxzylkwz.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gkfotebi.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jerhcysw.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ggvbtast.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3qybnchfo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vashcoke.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ksfiruqm.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3evfzfsmh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3okkmotbb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3pkqnxfin.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3yhntoywx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3uqhkqwym.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ibtehtvf.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3zfpkpdur.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jcohktxo.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3cuqdwyni.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3heyupdpb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3bwmxwgwn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3dtbmqdnh.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3sddckenh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mztqumah.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3snpvscib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tbhxmrzk.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3qhsezpyv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lpowogoo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3sheklzld.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wcwoxduv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zzihfgne.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3nksfqcii.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3ufzsmrhh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3mgywjejm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gvtgzctw.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wbzpuspz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jzdhzbql.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3kmdwulgg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3bfgpentv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3orksretf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mttjjlrj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ejlhazht.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3yzvytvda.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3gwpmruyz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3maoqqunj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ekanposc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pigqpofe.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3qlbanetm.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3eabclnki.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vgnyfgih.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3cbnxerwa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lutnvlkn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3xskmdflw.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pgdmpmsy.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gadbyxia.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bstkwxev.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nkjjygbh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3phqueljv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3jdavxuvj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3vmxtpcxp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3hfezxqic.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3fbrwaxdk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3pfkvtdoj.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3egvgfbnd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3wsisgxhz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3pkxjxsfh.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rjmnbnot.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3iclnvrot.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mfplqxmx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3necoqeuw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ezarcuzq.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ghcyuqak.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3taujjwka.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fxzgoutk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3htlijgru.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dplhiysg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3wxjrgvxo.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3vcoycwin.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3afvabefv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bxyzkuhm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3pxspqije.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3dxdjzwlr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ygvghjrh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gwmoongj.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xkvuqbok.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xmcmjvlf.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3ldfskdgr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3jnkiqdam.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xdjdfcdf.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3yeuwiemh.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3yqvjnybh.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3vqmxyxyi.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wkicvfrq.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3biklkynx.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ryysbdmu.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ihcgvzav.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3jehosjjz.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3scrxbtql.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3llhfauud.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjolbzpo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iypllykb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3prfakhrc.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3wzkmeznh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3tnyyrxqj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3thoricvn.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3apphdamf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3bqxsyixb.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pyrjiypw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ggnovgxj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3qxjjwkco.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3uwzchytm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ezssjroh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwutzwcc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3asueazxc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3rslrynyg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3ukuoqcse.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fwxhnnww.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3qvawlcqk.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3irxzpjuw.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fpbdqvoq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3cixftqld.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3eurjzamq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3gyojapnj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lkjajcjc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ndnjajyd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3gividbxg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3mzlclbqy.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3imkaovcu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rrrmafbb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mnthtnga.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jzmxsdnt.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3olncbyku.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3qjebgszn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3hlzpdgut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3shvirbgx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3xqsxpfok.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxcghoad.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3otwqlhxc.html


<!-- 参考信息 -->