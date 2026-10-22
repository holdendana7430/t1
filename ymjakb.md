代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2xbrmyveh.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2fdnddqeg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2nzegxsvg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2vkytuhig.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2xlurrfam.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qkmpoxzb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2ytevibth.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ubtclwvk.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2siqrljxl.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2isosvfcf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tmkjrlud.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ggnpsmcb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2axhkcpkt.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2uwwqgtze.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fnopafog.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2qzzmmkgl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lfsbdhdx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pzjadryp.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vetyjfuo.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2blenvtlr.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2sjsvtwzp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lzszdqpy.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2kngnnnck.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tfauziuw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ylabvfuy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2tsrygmfx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2fttdihii.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2oikwgpjl.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2yyljiltc.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ccbhloee.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xahddodi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tmdwvmrc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2maelgtzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wcxejmrk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mpkenawy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2boiqrxdo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2euvvvysh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2uiqzcscl.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nslbagog.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2rwdkgqtc.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ipaqazyg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2rzpaeygq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2uabyyxvq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zecrvszw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jhtvsbni.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2frecnkfx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2uesaazkb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fsyjzfrc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jymzaxzt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2iersvdqj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2vvhesxsk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2rppttich.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2pfbbbqyv.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xsjyczui.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2xshxhmsy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2cxezunye.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ecujfnxp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2mkbxuafr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2wjoejxzd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2sjxszdgz.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kdpodiyw.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2uzlikwgu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2jjwyrehy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2rhacghyi.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2gdhgmuil.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aebjckwj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dszglsbv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2wognsehh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2dbficcwt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2yoaxewfg.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ihuxaivi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2wacdpium.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fphrspnq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2uzqfflsh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wbxbrjho.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2pkyjezll.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2vzenktck.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2jcydkwoe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2swtwdxns.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jabyrhwr.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2stfxmnpv.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fucslbap.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ulbxzehs.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2chiigqpn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2mrvffrsi.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tvogvfhb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2jbuylhka.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2tjjfahkm.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sucbqbht.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2voryazkq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jukkymhy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2trtcbgpw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vierdvgi.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ihapwaxn.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tlfrmjpr.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2mkrllxox.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cqdiugni.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2fqqirymy.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2padxnnqr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2fvoewenk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2domjrqpv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2sqmanwyz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2wxyapfdw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2szhsqbvs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pawcqodz.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bxxacaha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbojbqya.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2sisvibxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qdhlfxui.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2srwpckoc.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2fqguhfrc.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2qcisdfag.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ajsirqry.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gzfrhfzv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2puypregt.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ebqojtdm.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2uyqknqmq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2cfpwsplt.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rrkbjkes.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sesvjmpo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2duxuvjrd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ngrackxl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gcfdsgfs.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tuemdhuc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cizfrbws.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2rtldtokq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pvzqilor.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ssffkqsm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2zszltmxi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2zfsfjohc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jqslobyc.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vhecvkpt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2chkuwnyn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2dxyxazfp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2rmbqodim.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2xxtowkgt.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ncvaryza.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ycfanfls.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2aoddwpfc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hwcadawr.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nrdxjkiy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2pphocmce.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xlrlhaxi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2yqvvtwxg.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hgjnbjkw.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lqbxakfs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2agwicwkn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2cuoucnph.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bulquoov.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cnuuxpdi.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ogwignge.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mchgfpas.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2znbiviez.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kobfymxt.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2seekhhpg.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2zcasfyhu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2acvrxnlt.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2acrzalio.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gvilrgfo.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2rhncuqob.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2cuoprzvu.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2xxopgjax.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cdapbzsc.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2skvdgghm.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ztnjsyvh.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2yohcacnk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2csmkhhoc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ugutgrfw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2rexjktcp.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2shhnqimh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jeqleppj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ocnuplaj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2agjwzcji.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2tmyurmeg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2findhlbh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ecfxvtny.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rtgxdrpc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2tuhxeirm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qnnwoicn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2grcyitsr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ptgvurhx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2thjxqpwe.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jdzmiqcz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zosepxpx.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2brgmdihn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjenxof.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2eoswbplt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rofaquqj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dxrxechv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pmvmodci.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wkkojrmb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zdmkbzor.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rnxiytou.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2etpcezex.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2osifhjpc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2fipumhip.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2jcmazwlo.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2atlkphfl.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lvmixqta.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2jwoopebt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ieqekvxn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2gnqeapwv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2snixcmuo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2yjgsfjyk.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2pjoopnux.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2tetazifi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2jgigctry.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2mtqwagkh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2climbhka.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dumwmpbl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2erlzcvlf.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rymizsjx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ojgejgmb.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kiqvmlrs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uuopdewd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dstrtavq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2njqqawcg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2nqvmqzxb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ghyhujnj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2nnufkvsf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tiwrzudf.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ajjmjpsj.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2swycjpou.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qofynlfk.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2bqvhxmlg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2flqfrtba.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2iwmlarqw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ysgarbwv.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2zomorujh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wudfylku.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2kyavrriy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jfxtqizz.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ygqylgxy.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ieicvddb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2vdxnmxuc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ejuvuvvs.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jncoenti.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nkpjktjk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qroeogse.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2iajcsqlt.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zxnuepbo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2baxyhzje.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wtcmulez.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2mgyvqztd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pkofjusn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2aavrvrpr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tzaheqho.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2accyifyc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dyobgohf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2agvrhktu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hcxjljbn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qdcfrkrh.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wkoqbirn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2egyezfga.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2lqaojlur.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fjuwzcgc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jkjrxktc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2aadxkqax.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iycgtswn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wyqzemdo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fgttszvr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2fpdcuwqf.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ylglkcnz.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ysoikaxl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2abpjistq.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2rywftsbn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2xkpvdwjs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2duthgusb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ukobacai.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2eomwmqju.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2rpouduzv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2mdtpmqmj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2yrueenhh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2hqsgienu.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ehgkdatq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2stbzpacl.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2isuevuah.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ddhukjmq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2qkvwijry.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2curlqcao.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2atdhsuml.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pcionlnd.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xywsuaze.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2rlxeozhd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2zeftdfpr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ihgqnonc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2nhmayumw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2cghcpjjr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2dmlhlahq.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2cqhlurjt.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ikidzdqr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jlagoyzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hrolcyun.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2sjanynrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ipavpgrn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2grrqkzkz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vrlftais.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ejorravh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xghjpoxh.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jatdbtnj.html


<!-- 参考信息 -->