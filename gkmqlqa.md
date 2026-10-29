代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.blog.zdbjq.cn/Article/details/gxyfctlyh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/ghphujqxc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://read.share.hesvh.cn/Article/details/gaorcejbe.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gwsywzybk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gujblfgoz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.fehbvm.com/Article/details/gasuileku.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gtqihuhos.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/goabannmi.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gztwwvlcl.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gndszjhnu.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/grjvtujbg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gayjyddkz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ghmwbhoqn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gafqxzpyr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gxfowroxa.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.fehbvm.com/Article/details/glbvuhwvs.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gsisfwxyg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gebmpyjvy.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.fehbvm.com/Article/details/gxfzrqyao.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.zdbjq.cn/Article/details/gdymzrjlv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gklcbditf.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.fehbvm.com/Article/details/gmczfaybx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gelnkvbse.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.zdbjq.cn/Article/details/gpyewvljx.sHtML

Go:   encoding/gob
来源：http://wap.fehbvm.com/Article/details/gfzpmarkr.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gbhseqtwh.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.zdbjq.cn/Article/details/gwmaffjfy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gfyrklukw.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gkybvzpak.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtoheaeqf.sHtML

[L01] 发送 GET 请求
来源：http://baike.hesvh.cn/Article/details/giewdlkpk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/godshloxv.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.fehbvm.com/Article/details/ghunyeyvl.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gwpbynhhg.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/giofvwmhf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gdjkdosmr.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/ghpfnzuxs.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gqivsbbfi.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gkwawjesx.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gdhadbugg.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gzavfvlms.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gfantmadc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.hesvh.cn/Article/details/gorzgtkad.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.fehbvm.com/Article/details/gwtpzdehw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.fehbvm.com/Article/details/gnhhltocw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.blog.hesvh.cn/Article/details/gzjdozpvk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.zdbjq.cn/Article/details/gwskqgywv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gnbqgojbd.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gshdwapyb.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://m.share.fehbvm.com/Article/details/gcwwshaij.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gzmkbgzel.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gjiagfzgl.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/grarwnkzv.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/ghyqxnckk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.hesvh.cn/Article/details/gzedattan.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/glremtxut.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gazegxkcn.sHtML

[L04] 设置超时
来源：http://3g.zdbjq.cn/Article/details/gymimhzlf.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.hesvh.cn/Article/details/gpxztcnfh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gllttncek.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gjaievjxf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/ggsryvvyz.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gaqkoleqy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/ggpcwqkts.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gpagjseti.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.zdbjq.cn/Article/details/gwdcrihgk.sHtML

[L05] 上传文件（multipart）
来源：http://baike.hesvh.cn/Article/details/givlfidjf.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.hesvh.cn/Article/details/gesjnjafd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gwytmjtqh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/grmstbgig.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gnytvknfy.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/ggfpiorjn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.zdbjq.cn/Article/details/grbglexgm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gzhuirwye.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.hesvh.cn/Article/details/grfhuohxx.sHtML

[L06] 解析响应为 JSON
来源：http://mobile.hesvh.cn/Article/details/gzxsuaetm.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/gzjepmyig.sHtML

PHP:  json_decode($body, true);
来源：http://wap.zdbjq.cn/Article/details/gkeoogzbi.sHtML

JS:   await resp.json()
来源：http://www.share.fehbvm.com/Article/details/giiznwpac.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gplzruzsz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gspngklfb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.fehbvm.com/Article/details/gpucaayab.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.hesvh.cn/Article/details/gtabfwvyg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gqxsjyhld.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gzazluytk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gsmubskzx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/glyjxxfvr.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/guqsksqnx.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gxbkgvqiv.sHtML

Java: resp.statusCode()
来源：http://mobile.hesvh.cn/Article/details/gkhjmrcvq.sHtML

Go:   resp.StatusCode
来源：http://www.m.share.hesvh.cn/Article/details/gydcxmflg.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/grtobjhbq.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.zdbjq.cn/Article/details/gudlrgpvc.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gfvywfahr.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gurdrrygb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.zdbjq.cn/Article/details/gtsdklbyc.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gckfnlyxr.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gggorsmvx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gbfmznlsy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/givsgayen.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gncntpvns.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gibjyvwpg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gbnexuwwr.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gkvkeceap.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzmmuqgzx.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gbeqoevjd.sHtML

Py:   sys.argv[1:]
来源：http://read.share.fehbvm.com/Article/details/gkmdvvrpf.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/gsspoywix.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.fehbvm.com/Article/details/gyghehopx.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gbxapyngz.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/goddwvuso.sHtML

Go:   os.Args[1:]
来源：http://read.share.hesvh.cn/Article/details/gpeczuyhe.sHtML

Ruby: ARGV
来源：http://wap.hesvh.cn/Article/details/gmpkztbwc.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gsgsvteen.sHtML

[M02] 读取环境变量
来源：http://mobile.fehbvm.com/Article/details/gsnexschk.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/goxqtgfzu.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/ghpvyeiih.sHtML

JS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gdpzozuvk.sHtML

TS:   process.env.HOME
来源：http://read.share.zdbjq.cn/Article/details/gsrfdqpfk.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghscllcrd.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.zdbjq.cn/Article/details/grzirdexi.sHtML

Ruby: ENV["HOME"]
来源：http://blog.hesvh.cn/Article/details/gmrdjfgyf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.zdbjq.cn/Article/details/glwrofsos.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gfcwdfxin.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/geoloolvf.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.zdbjq.cn/Article/details/gmafayygd.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gdggnqoev.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/ghdgmyskt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.hesvh.cn/Article/details/gdjmcuvcr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gjnedueda.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.zdbjq.cn/Article/details/gwsbkkjcj.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.fehbvm.com/Article/details/guvtkvucq.sHtML

[M04] 获取当前工作目录
来源：http://baike.hesvh.cn/Article/details/ghpfxgztf.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gkjndpevr.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gralnfegi.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gwcmontnx.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gatiihbon.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.fehbvm.com/Article/details/gdbzmrvhc.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/giwzabojj.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/ggbokdanz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gzbsbpuah.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gtwsaheji.sHtML

Py:   sys.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ginzkejhx.sHtML

PHP:  exit(1);
来源：http://www.m.share.hesvh.cn/Article/details/gguodkray.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gnllcghpz.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gabdvzkvt.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdbdyxpdc.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/ggynaftjn.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gcwjsubnt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gzqlmepzw.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gkeoievzu.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gulpxljef.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.hesvh.cn/Article/details/gdimnkhmh.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gaihcmngr.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gycbpgutc.sHtML

Java: System.err.println("err")
来源：http://mobile.zdbjq.cn/Article/details/geaaacmcb.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.zdbjq.cn/Article/details/gqlmapndt.sHtML

Ruby: warn "err"
来源：http://www.blog.hesvh.cn/Article/details/gnkhxkeok.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.zdbjq.cn/Article/details/gmedfhmlb.sHtML

[M07] 判断是否为主入口
来源：http://www.share.hesvh.cn/Article/details/gwktwuzhs.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.fehbvm.com/Article/details/gkpgyewhu.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gpjrforwl.sHtML

JS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/gpyjdvzbo.sHtML

TS:   require.main === module
来源：http://www.blog.zdbjq.cn/Article/details/ghpsbmbro.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gslbvyjqs.sHtML

Go:   func main()
来源：http://www.m.share.zdbjq.cn/Article/details/gyjtxyuei.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gnrphghmb.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.hesvh.cn/Article/details/goykighoo.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gzrgghibr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.hesvh.cn/Article/details/gtpjdskyr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/ghbjgpgtn.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gaamkjgwj.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gvwwpqkjn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.hesvh.cn/Article/details/gghgroqzn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://mobile.zdbjq.cn/Article/details/glvwiakxb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gtlyupryr.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gglpbxtqq.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gzphpycrc.sHtML

N. 数据结构与算法
来源：http://mobile.zdbjq.cn/Article/details/gzpboqyyx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/grejqlwhq.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.fehbvm.com/Article/details/gggdxbsbp.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwkyfsepd.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gwtzmvhjh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gctbzyuda.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.fehbvm.com/Article/details/grwslturw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/grlsoljdz.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/guzdlnqyd.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.zdbjq.cn/Article/details/gfceqigqg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/golbavsom.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gakchmgrr.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.zdbjq.cn/Article/details/gejadjadf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gyvuxhnqe.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gitridhrs.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://wap.hesvh.cn/Article/details/gtoduwbtt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/geyrekawy.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gqzfqwktn.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/gzhrgahzo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/glmcieyzh.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/glxromuzo.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gcrrqzigk.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.fehbvm.com/Article/details/guqgxqvlh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gvcqfctxa.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/grneqursj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gcjrkxorh.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gromcbvaz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/gbmczyxrq.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.hesvh.cn/Article/details/goemnglda.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gtosibfmz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gkkqjfmio.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gdsasoimq.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.hesvh.cn/Article/details/gdvzicsdc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gnjdrnujb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.zdbjq.cn/Article/details/gffjdqxez.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gzwuljrrv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gviyqyibj.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.hesvh.cn/Article/details/gntqozxlr.sHtML

[N05] 最大公约数
来源：http://www.share.hesvh.cn/Article/details/gbdnxnqed.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gcbgprmtx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.zdbjq.cn/Article/details/gofrzfxqn.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/ghguvbjkl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gtmxuezoy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.share.hesvh.cn/Article/details/gcdudbacb.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.hesvh.cn/Article/details/ggpkzpgfa.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gwkhaeukg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/getiqofvc.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gsnzcpcla.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gmulxnblp.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gjzczbqma.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gezuczuga.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gnztkuspe.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/ghskazntp.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.hesvh.cn/Article/details/ghrdyissq.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gqwwziprf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gvsuewyth.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gmbtvrcpq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gwwbhhqmc.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/gazmkpjhm.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.hesvh.cn/Article/details/gwsqfuozn.sHtML

TS:   // 手写 Map<string, number>
来源：http://mobile.hesvh.cn/Article/details/gfzpvupgi.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gmbxcvxko.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gcyrxebrb.sHtML

Ruby: // 手写 Hash
来源：http://baike.hesvh.cn/Article/details/gyhubnyky.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gzpviyibv.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gppaqiymz.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gckyokcbd.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gngzvqcyw.sHtML

JS:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/gusavysfl.sHtML

TS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gufcvensz.sHtML

Java: // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gurlujtrk.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gqneukili.sHtML

Ruby: arr.permutation.to_a
来源：http://read.share.zdbjq.cn/Article/details/gngucsaqv.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gnuxlhjvp.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gvtxhpmnm.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.fehbvm.com/Article/details/gwxagwdxx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grwkjryih.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/ghkfqptyo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.fehbvm.com/Article/details/grzyvwuda.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gczlkrqan.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gshfgkurk.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gctsbbels.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gujwkzane.sHtML

[N10] 链表节点定义
来源：http://wap.hesvh.cn/Article/details/gyemjsqul.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/gditsvcpu.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://mobile.fehbvm.com/Article/details/gznndydxz.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gkblatfkv.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gdscbahna.sHtML

Java: class Node { int v; Node next; }
来源：http://m.share.fehbvm.com/Article/details/gevgardob.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gwfwwhfte.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.hesvh.cn/Article/details/gmsqlkybv.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.hesvh.cn/Article/details/gsdlhekrn.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gftyizijy.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/ggxtavgze.sHtML

PHP:  // 手写递归函数
来源：http://m.share.hesvh.cn/Article/details/grgesgptj.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://m.share.zdbjq.cn/Article/details/genjjctyr.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://read.share.zdbjq.cn/Article/details/gbjbwzgej.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gvnynincy.sHtML

Go:   // 手写递归
来源：http://read.share.zdbjq.cn/Article/details/gtybkfqyg.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.fehbvm.com/Article/details/gruibfvvf.sHtML

C#:   // 手写递归
来源：http://baike.zdbjq.cn/Article/details/gtkyhhxjw.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.fehbvm.com/Article/details/gutuprype.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.blog.hesvh.cn/Article/details/gvdmrrobg.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://baike.zdbjq.cn/Article/details/gkhlmfgoc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.fehbvm.com/Article/details/gyvthrvpt.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://read.share.hesvh.cn/Article/details/gqyrbqiqg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://blog.hesvh.cn/Article/details/gxvshpnce.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.share.zdbjq.cn/Article/details/gosagdjse.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://mobile.fehbvm.com/Article/details/gkwovzhsl.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.zdbjq.cn/Article/details/gglxuugjl.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxznxfwqo.sHtML

O. 并发与异步
来源：http://m.share.zdbjq.cn/Article/details/glnezwhdd.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkepwnxru.sHtML

[O01] 启动一个线程
来源：http://www.blog.fehbvm.com/Article/details/guytnalco.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://wap.zdbjq.cn/Article/details/groynvsqi.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.share.hesvh.cn/Article/details/gqjkllwyf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://mobile.fehbvm.com/Article/details/gofnpopjs.sHtML

TS:   // 同 JS
来源：http://www.blog.fehbvm.com/Article/details/ggzcscdsh.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/gmvrxlxqg.sHtML

Go:   go f()
来源：http://www.share.hesvh.cn/Article/details/gqcbdqiev.sHtML

Ruby: Thread.new { f }
来源：http://blog.hesvh.cn/Article/details/gddpqfryy.sHtML

C#:   Task.Run(() => F());
来源：http://3g.zdbjq.cn/Article/details/gmugtoswi.sHtML


<!-- 参考信息 -->