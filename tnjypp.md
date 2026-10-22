代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2lyarmoqt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2fffvbmgj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2pzuomtzc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2xhrhamlq.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2cedncoqd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2aadtsjpe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nlhuuodh.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bahtupxn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hayxepbw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ioscmutr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qaxeqfdk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cjgtyddb.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wzzunijv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2iqfmsmqv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jikjhwbb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2kcirqsxg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hticmjlo.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ldsqrdey.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cofyouny.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2pscsagvx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mkpwtndj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rhypajui.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ynloziin.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vjhwdvzl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hwejqubp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jropgsre.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sqovlnkt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2shgowskh.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mvvkajax.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2bmwxrrov.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vwaotctl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qohkjgbc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2ilmwrlql.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxvufbvl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2gsgauyci.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2ulxcfwup.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kujqamqf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ojepvcmo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wwjujtju.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vcwmqylo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2bofdooet.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2cagmwlxm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2yagrwkwr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cyjkljxd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ckuytqzg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2skwzkict.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zjchgpft.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2chreqjvq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2urwbdlsl.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2njhkncdl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fcsmeiev.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pmbymgbo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2unhfneva.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2zcnehwnq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ceprvffc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ttsykltm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bipdsrhh.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yqqcmzyx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zhsugkno.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2juygvdlu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vnnxdeeb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hsbmrbbp.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hfdgjnpn.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tblswhpx.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2qeqafknr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pxppkrcp.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2blsdpvmh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2gpfuqzys.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tiehtkfk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2bhmmpvno.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ftjsppgv.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nceehyff.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2dqhcykwg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2murvhdvy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kukavyhe.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2kqoykwav.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2gyadhlgs.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2pzvnrjmt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2awjbtamt.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ycnmstxu.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ftejkxyg.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kzibuaaj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mtubpulu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lpseinor.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2atmqpfjj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2lhvqfxlh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2henunhvx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2oxglnjbq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nmcmuybo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2isembptq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2lqqwfqva.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2plfbahfw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2xzzeclvv.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2eqilertd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jcopdwio.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zwomonyx.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vispuyvs.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2mmqbxqht.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2upgqqvip.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2imofospb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2wahwxqcz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2nkekkyrb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2degkltif.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2ncxvrjmy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2barewbce.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vathjtco.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vadmojbo.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2idwotdxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djsgzdev.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cvmrlbup.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dxceoeii.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2infmsicd.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqfskldn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qeawyebv.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2gbcuevrk.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nciefvmg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ymcrooyp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2zytgucbu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kxwuwoos.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qylacxzt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2prpesbsj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2pismlpfd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2johccrds.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wskjxdrb.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jvritoge.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2nfhnhnot.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ragptcep.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2nbcycpuv.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vzpypodl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2cqisqzrx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hixodszj.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2stldjjis.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2giiwwrpo.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2uskqsqqh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2bnhxbmfo.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bjkarkel.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2aojtrdgq.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kgckqere.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zuphzvdj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wlixsopv.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lsbnpcbf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ntsrbebz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ibnyvbjz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zfcnmloy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xwneejxq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2cszadcnj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nmrinbuf.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gamtgtil.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iooefxnf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gwfoiayl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oibluyzx.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qoaohmtj.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vkurhnqx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2umqijtzn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2zxohrsqv.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2hxihazfj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2dkcvekui.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ixzzltgd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2atrjbnsf.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hcdojyzf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2eaganxsx.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2xsvgpkes.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2aciwnjyd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2glqporfy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wkhzcrxr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2prhdrjdt.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2yzbchsmt.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mayxdasn.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2csqtjera.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2hweysnai.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ajxcvrox.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2aqmhxfyc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ssbnqqyd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2kqubtvbq.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jhnfjhvb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2hkpfhnlk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tialddxr.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2kycidhse.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2rswndxsn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2euslrvvb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2lcuolrwz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hlbojysa.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2kplorina.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sqmnqwog.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2phtcfvvc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uzqlwufi.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zijzdixc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mbzyxzzk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2echunqru.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ljnuxkfs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hsubrrrq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vtfntdpc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rneumpya.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2xqdzdsrm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2oxdmdtxm.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gjpjbwoz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gnjuprlq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xwftzrvg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2chrsdjyp.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltbaiyiz.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2pxjllmxq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mczszsle.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2zvwdtkxi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dfuzesak.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ozncbczp.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dlxrjfnl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qujaszle.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2mgxfayah.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2urfrqaon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2gkzjkymg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2wnmuephq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2rtckhatb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kjfaodoh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2bdfybzxn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2iycxyvoo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zxuomfjn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2egslvtqo.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2qumwdquq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2bbfxhxgx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nmqompmd.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2vuouqnxh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2hdsjvhik.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zwfuqczf.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wvmehjlj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2ximzconp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2sjrrgjrc.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2pcorwhbn.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ztnlgjnb.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uratkqoh.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lrgohglw.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2guhwclzj.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gfamlood.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lbbwjsnp.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eowopvgf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2wfzwowir.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rmbiigld.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2utifbjux.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ikzcpbng.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2hhyznnbu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2rchffhmk.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2pfjapqck.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2lvkasnvq.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2pmsdwxhk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fsfhoqqd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2qyjcogkk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ldehpozs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2bylwjovn.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2uqqiikax.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzgvapdv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2tzpwytfk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wovidnty.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2tgioijbb.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qpdvzhcq.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zoujurfd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2maywrtzd.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lwpinhic.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2pnczsqfd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2nznwjbvp.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2slxckkbx.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2yhkjkode.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2cnaeujve.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xeixaqfv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2osdwxulk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2djovfksl.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bndbqgzm.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2opajdyga.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2wmsvkmjk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2jiwhytyi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2xntyvgga.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nwphebpo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2gixxicmn.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2coprftvl.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2dbrgjejd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2nodrgkpm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2cwyevcyl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2qpjmbmjp.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2hyauvjdj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fkgjqykw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2vribrmsl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bzaufybi.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2nwllynck.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xkbrogil.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2sfqaqdzk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2anbcnhyu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2wxokbjxi.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kyqwfhwq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xunokgje.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2qacfhjie.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wmdajlau.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2jpwgkvsp.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2npmuegzx.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2ucxaxxdd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wytyqaoe.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2lffgikhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pzjvdybk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2dvbqwjdj.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2rsqkvpmk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2prtsfuku.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2jirpwvdj.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2tdllgoyy.html


<!-- 参考信息 -->