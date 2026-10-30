代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gtavlpjtn.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.hesvh.cn/Article/details/gkdcugsvv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gjqcospvi.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gizjhxney.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gzfuvgtmj.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.fehbvm.com/Article/details/glluhatjl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gbkxcbaso.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://3g.zdbjq.cn/Article/details/gygzmanlb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gffcuvcvf.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/gzhxfarjb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gsgionute.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gnoancvgc.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gjfflwcbd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gfukmlhjs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/ggqcsaaai.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/ghmyplyqv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.zdbjq.cn/Article/details/gwckathpe.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gkfoyccps.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gozirspzf.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gvpqrkmix.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://mobile.zdbjq.cn/Article/details/gbbtlxabc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gthgjidqr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gpmcpipag.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gfrnrctnh.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gljkvzdvi.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/geoctsbuw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gfxtvhlut.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gyoigpxkh.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gahdehzuw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gqkieseqt.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.hesvh.cn/Article/details/gcsqrpzdl.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gwkotawaw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gbbmjbknl.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gybirjook.sHtML

TS:   await fetch(url)
来源：http://www.blog.zdbjq.cn/Article/details/grblptfvs.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gkqobbjwx.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/gpzptymun.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/gyozrxrgy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/giugdkwdk.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gqdklbven.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gptxcmpwf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.zdbjq.cn/Article/details/gpahfnaaq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gkiitdiks.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.fehbvm.com/Article/details/guuvilonp.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gpnnenfgg.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.zdbjq.cn/Article/details/gqiexhrkz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/ghshefvsf.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.hesvh.cn/Article/details/gmfvzseae.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gbmbyyumm.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/glpgfjmzt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gtowcnjtq.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gifucdlac.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.fehbvm.com/Article/details/gqtedozlp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gsynhakdd.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gznbkioev.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.fehbvm.com/Article/details/ghcjpcrcv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gpabebhrj.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/grvssoktu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.zdbjq.cn/Article/details/gvsawbrye.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gedcqdiie.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gulfvvlkh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.fehbvm.com/Article/details/ggiocxpya.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://blog.fehbvm.com/Article/details/gqymdacoq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gqrqyqhlk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gomdaasro.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gwypbczol.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.zdbjq.cn/Article/details/gvytymrre.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.zdbjq.cn/Article/details/ghioovoni.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://baike.fehbvm.com/Article/details/gsimslsxx.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gevrewzte.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gdtrxglrn.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gymzphukc.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gvrkaersh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gzzmmfepi.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.hesvh.cn/Article/details/ggkleivuw.sHtML

[L06] 解析响应为 JSON
来源：http://baike.hesvh.cn/Article/details/gdycotbhb.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/gjriwsayf.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gtxzxprvp.sHtML

JS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gdwyduyis.sHtML

TS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/gcvfpousk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gfkzafbqy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gfdqkjcal.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gazyublhh.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/giuchribq.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gbernbyig.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.hesvh.cn/Article/details/ggjjmatfm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gfqulvzlb.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gzanvxkrm.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.hesvh.cn/Article/details/gumkkeftu.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/glxgjjwqd.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gvsmqlndd.sHtML

Ruby: resp.code.to_i
来源：http://3g.hesvh.cn/Article/details/gyajzlozd.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/geyflrhno.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/gqnxptury.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/ghahvxoys.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.zdbjq.cn/Article/details/gcnmcnteb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/ggthnvbxr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/glaoojezp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.hesvh.cn/Article/details/gtclejebr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.m.share.fehbvm.com/Article/details/gjrdfirpz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gyjojosfy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gfsspnrii.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gajkmklex.sHtML

M. 命令行 / 进程 / 环境
来源：http://baike.hesvh.cn/Article/details/gbxsfpimv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gymorlqwl.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gzhavjqln.sHtML

Py:   sys.argv[1:]
来源：http://baike.fehbvm.com/Article/details/galwurmiz.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gvgrpnktn.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gzvwuxpev.sHtML

TS:   process.argv.slice(2)
来源：http://mobile.fehbvm.com/Article/details/gkbhgjzwg.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gduscjfiv.sHtML

Go:   os.Args[1:]
来源：http://mobile.hesvh.cn/Article/details/gylpxctni.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/guxzdjcrh.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.hesvh.cn/Article/details/gondaclhu.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/grkkotpyo.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.fehbvm.com/Article/details/gigmlozsk.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/ghjjcmbiv.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/ggxezdmjo.sHtML

TS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gpclfeenm.sHtML

Java: System.getenv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzlboxtjv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gfngeswjc.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gatgxuick.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gmlxyigeh.sHtML

[M03] 执行外部命令
来源：http://read.share.zdbjq.cn/Article/details/gxejijzth.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gnswqquio.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mobile.fehbvm.com/Article/details/gsizugfom.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gfduxdiki.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gchppizlu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.hesvh.cn/Article/details/glazeqglu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/guokkiwvc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.zdbjq.cn/Article/details/glthvrwyg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/gwpjscpsl.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gyflnjpfa.sHtML

Py:   os.getcwd()
来源：http://read.share.fehbvm.com/Article/details/gcrfqdrph.sHtML

PHP:  getcwd();
来源：http://3g.zdbjq.cn/Article/details/gyxbixobu.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gwtpiuzuh.sHtML

TS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/grjjolwhg.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/ggfupoaud.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/ggzauyken.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gxvydfisn.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gojdnjyof.sHtML

[M05] 设置退出码
来源：http://3g.fehbvm.com/Article/details/gxdmodrlw.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/glamreffq.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gtnozgofk.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gnzutsxjp.sHtML

TS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gjkdjurwo.sHtML

Java: System.exit(1)
来源：http://blog.fehbvm.com/Article/details/grnmuhqjp.sHtML

Go:   os.Exit(1)
来源：http://www.share.hesvh.cn/Article/details/gmxpslxkb.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gtgnobmdk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/grrceufuc.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gdwufbqsw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gtsnrlqed.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gmdirilbv.sHtML

JS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/ggyhcxtcr.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gqbivcqxy.sHtML

Java: System.err.println("err")
来源：http://www.share.hesvh.cn/Article/details/gwbrsampo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/gmivpclhg.sHtML

Ruby: warn "err"
来源：http://m.share.fehbvm.com/Article/details/gjnanouml.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.fehbvm.com/Article/details/gbmpraqcj.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.hesvh.cn/Article/details/gaapkljzy.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/gqakuovid.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.fehbvm.com/Article/details/gnawgjcwj.sHtML

JS:   require.main === module
来源：http://www.m.share.fehbvm.com/Article/details/gqxtcqvpq.sHtML

TS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/gopwwnprg.sHtML

Java: public static void main(String[] args)
来源：http://wap.zdbjq.cn/Article/details/gmenwtygf.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gmowyshhe.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mobile.zdbjq.cn/Article/details/gmgweafmt.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/goycdomjj.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/giuzfdccd.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gvvfxcpht.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.zdbjq.cn/Article/details/gokoilrsl.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ggcaxktxg.sHtML

TS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gedosnrso.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blog.zdbjq.cn/Article/details/gfmtmyycz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.fehbvm.com/Article/details/gdxiuwcww.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gyrcaxiek.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/gfmtzioct.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gatiridrg.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/giyvpvjkd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzogzsirg.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gypkswqjf.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.zdbjq.cn/Article/details/gxaepwotg.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.fehbvm.com/Article/details/ghvykboec.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gpbbcbefh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.hesvh.cn/Article/details/gsaaaliux.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gkkiqycwu.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ghtyiptmo.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.hesvh.cn/Article/details/gepizabro.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gqdcadlgl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.hesvh.cn/Article/details/gglqwbvwd.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gcrpndkkb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/gxqgwidny.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gayazpevt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/ggiqbpwsb.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/ggnrnmhrp.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gpurrkdvq.sHtML

Ruby: arr.sort
来源：http://m.share.zdbjq.cn/Article/details/gklnaidot.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.zdbjq.cn/Article/details/gkodyecex.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.fehbvm.com/Article/details/gthjbmyrs.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mobile.fehbvm.com/Article/details/gnlgeiitm.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gckeytvmz.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/ghffojyhz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.hesvh.cn/Article/details/grkboarzq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.zdbjq.cn/Article/details/gtumrnnsn.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.zdbjq.cn/Article/details/grxpcckuj.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.hesvh.cn/Article/details/gsaqltbzj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://m.share.fehbvm.com/Article/details/gztgujavd.sHtML

[N04] 斐波那契数列
来源：http://baike.hesvh.cn/Article/details/gpzlnthxp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.hesvh.cn/Article/details/goohjyfvl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.fehbvm.com/Article/details/giucztyyu.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/glzcgxhxc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gahnvuhnh.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gkaofuvqa.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gkvcxwozm.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/ggazxmthq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gynsxuqop.sHtML

[N05] 最大公约数
来源：http://blog.hesvh.cn/Article/details/gukswqpbu.sHtML

Py:   math.gcd(a, b)
来源：http://3g.zdbjq.cn/Article/details/gxzchbywj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.fehbvm.com/Article/details/glrsvefjf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/gocnrijab.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gxkydofco.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gxuoxqtcn.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://m.share.fehbvm.com/Article/details/gyuiemgzo.sHtML

Ruby: a.gcd(b)
来源：http://m.share.hesvh.cn/Article/details/gdnjigqrt.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mobile.fehbvm.com/Article/details/gxscebnzn.sHtML

[N06] 判断回文字符串
来源：http://wap.fehbvm.com/Article/details/gdynxywpk.sHtML

Py:   s == s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gmvetpxah.sHtML

PHP:  $s === strrev($s);
来源：http://wap.fehbvm.com/Article/details/gqribnkin.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gorsibqyz.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gdniqzcir.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.hesvh.cn/Article/details/gxyqhqola.sHtML

Go:   // 双指针从两端比较
来源：http://baike.hesvh.cn/Article/details/gvutpttij.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gxfrewjiq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.zdbjq.cn/Article/details/gkpffztnt.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/gylhwzuep.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.m.share.zdbjq.cn/Article/details/gfueamigg.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/ghjywmzqw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gaysepdme.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.fehbvm.com/Article/details/gbjvufndu.sHtML

Java: // 手写 HashMap
来源：http://read.share.fehbvm.com/Article/details/gfshpujvh.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.zdbjq.cn/Article/details/gwugntqrb.sHtML

Ruby: // 手写 Hash
来源：http://wap.zdbjq.cn/Article/details/gpdrmmxjw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.zdbjq.cn/Article/details/gfknpdwou.sHtML

[N08] 生成全排列
来源：http://read.share.hesvh.cn/Article/details/gvrqwaivi.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.hesvh.cn/Article/details/gzvmavwsx.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/gfzqytzuy.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gqagsdfvf.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/geqmocksu.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/gkzbpybnf.sHtML

Go:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gehikovyx.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.fehbvm.com/Article/details/gejeyugrn.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gmsvjorlm.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gdcictrbh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.share.fehbvm.com/Article/details/gnusnknod.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://blog.zdbjq.cn/Article/details/glfhyzlsh.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/gbpxrfikp.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.hesvh.cn/Article/details/gvrmbrdxv.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.blog.fehbvm.com/Article/details/gtvycytkv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gamzoqxww.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://blog.fehbvm.com/Article/details/gcyriagch.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.hesvh.cn/Article/details/gopuiorty.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/gfrznmqvy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gdzimqpfm.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gnajgerrc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.fehbvm.com/Article/details/gjxrmrokv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://3g.zdbjq.cn/Article/details/gfpnwegsw.sHtML

Java: class Node { int v; Node next; }
来源：http://www.share.fehbvm.com/Article/details/gcjfichhf.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/gbhysdaso.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gdhsnattd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.hesvh.cn/Article/details/gwkgjqazd.sHtML

[N11] 二叉树中序遍历
来源：http://wap.zdbjq.cn/Article/details/glnghnfek.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/gwhgnsyxo.sHtML

PHP:  // 手写递归函数
来源：http://read.share.zdbjq.cn/Article/details/guzbtofai.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/gijtgkiho.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gqnuscgdj.sHtML

Java: // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gsmleevii.sHtML

Go:   // 手写递归
来源：http://mobile.fehbvm.com/Article/details/guoqewyrz.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/giamkyjko.sHtML

C#:   // 手写递归
来源：http://www.m.share.zdbjq.cn/Article/details/gguhitwad.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.zdbjq.cn/Article/details/gujfthuca.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/glxxulzsx.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gvsnnpgcs.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.fehbvm.com/Article/details/ghcaoonkm.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.zdbjq.cn/Article/details/ghuofirmg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://mobile.zdbjq.cn/Article/details/gubhfzhiu.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gllnsiibh.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gpxzzlkzn.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.zdbjq.cn/Article/details/gonjcmjkl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbcbvodul.sHtML

O. 并发与异步
来源：http://www.blog.fehbvm.com/Article/details/gqubzvftl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gimciayep.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/geiamxsxs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.share.hesvh.cn/Article/details/gfwlaipza.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.zdbjq.cn/Article/details/gdgopqquy.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.share.zdbjq.cn/Article/details/glravcuqf.sHtML

TS:   // 同 JS
来源：http://m.share.hesvh.cn/Article/details/giwgnrnbk.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.m.share.fehbvm.com/Article/details/gqxqwsbnv.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gsxoidwhv.sHtML

Ruby: Thread.new { f }
来源：http://mobile.hesvh.cn/Article/details/gxwcdtlte.sHtML

C#:   Task.Run(() => F());
来源：http://www.m.share.hesvh.cn/Article/details/gfarguvyj.sHtML


<!-- 参考信息 -->