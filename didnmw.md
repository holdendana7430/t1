代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kdimrvdq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2tkwwemzc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2spvcuwik.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2qihsznpq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2fniozgwi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2cqhyecdv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rukxfhbe.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2pamkpnex.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ppoidsxz.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2djylvehu.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hbklltqy.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2dtsacgmp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qxmpsixt.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vyuhljms.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tbutyahe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2fuhztrkp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2gnprvkuv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2epifunxq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2xspfzifd.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2attqodot.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hhcrwyyu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2uhoomssv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xpktywfu.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2cqinnchn.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2woernrsk.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2wnidtthk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2uymvunxp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbtwzsll.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2cqcqozfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mexnijdl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jsqlicap.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2befhprjt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2fzpozozf.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ynppkzca.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ywudqdaq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mbtduzhr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ncpwerew.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mkxdsmnh.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2gniehqrw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wjmzdjtd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wlqmftqb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2jyvgpvyo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wanuneky.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2looinitj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2gzbdpqho.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2aemprsmx.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ttvupote.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ryagupfo.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zglglblr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2jlhvvkby.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wvwjawrc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2jsesdhbq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2thyjbukn.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2kgswhsne.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wwrrnibz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2dtysbkqe.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2yszrlnev.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xnxjyado.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dwusgsso.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zlnbjwxb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2fklppheb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2suqkbrpc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2owoefceu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2tonqmgxq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ommaowkw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fpgcmroj.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2dgkjetiq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qdxqvvoe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ughgbozb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ehjmwkmd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rrfzlxzj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2xoqhxupt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2rirkytnt.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2jokegwpk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2topxaugl.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bveffxsp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2igjyjzsh.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2wbgtgspe.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2mjeuqkbb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2tmfpidip.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2lzpwbfyl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nthpysty.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2fyipzkcp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2aodwvjgz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kvrtgbxh.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2zymwcstc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2byjmpowj.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2kcqofymf.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2paqhhxhe.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2iqvyshnf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2lyezhuom.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2jjnnwehl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wuwgzipg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2vgmqkarg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2qruzuvwd.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2zhhtfjxx.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jkitpiyc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2utbkqrqz.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2vsgpurwr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2lvgaqevy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2olbptjav.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2jsarsifn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vgrejfhf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2icfimkmr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiwddukf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qsworkso.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nieyklke.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2kzoniiws.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ktytlfhl.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2iijbgzyg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qtbticlk.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2jzaphxul.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zrghisrg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2luclvxfi.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2sgmugqyl.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2drlbeycp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2pevkcwzl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uwdgnfxr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zliwalzx.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jrpttpwy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wswhwoqs.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2grpxywjx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cfuzmvhh.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2luhwmthe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2jlrpxfus.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2ogikrmmd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2odnmwbci.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2rjeabuem.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2fnefstsj.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fhofnjli.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kdukdpml.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2zvxjzmbo.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2tsyhlklk.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2oifurako.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wynqsolc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pbysiatd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2godfialq.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cwynoxkb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2imijoksd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2fclshzse.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2xgrsyrhu.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2arfdvtwl.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wrzjswqn.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2hjeudxxv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fzpquzem.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lyolbneb.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qicabnpv.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yoppypsy.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rssebqwf.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2cypibixj.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2rzifehhn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nycvbvaj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2phyvkgxk.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vbbsfhfv.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2eomqvfjd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xsejzpke.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2yzdonqqb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pthbmojp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2mrusojqm.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ceetgrsx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wqhhxwye.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2oeyimsun.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2rdvrniyc.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zhuuiacu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2mprrquol.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2huommhfp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2czkmhcrp.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2iiaqwetq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nsiyekbn.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2koliiklm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2oknerriu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ctokzqad.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yrmgqzva.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yzctnfzm.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2mmbxhnbh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fbfygerw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2swrjzenf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eajiyeki.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2jakqepxw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2prenjmsg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ygwmktfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lvkvkvhx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2bvbfuefs.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jyolzdkz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mpzggsfh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tfiednix.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2zexllnpm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2fznvjcyc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gsvfgymg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rgewguzp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ejszllet.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2suukqueu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qlyijifh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2fllqckok.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2dxwehtgy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rgmmuncm.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2dteibkky.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fkxzauui.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wnrhvvjn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2bgsykfve.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2pwdhzefc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mticmwsn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2yysoifgd.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dblqwcle.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2hvsyiatv.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2xoiezsmo.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hedpkfwb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2qngpbbfd.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gihegrsg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zspnuplr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mcpxqisi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2btubycsv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2upliunhj.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2rinbdxtu.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2eijiwxai.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gwnifaym.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ilrvznhk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rhlzlddo.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2debmlmcr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2itrtdksy.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xtreurbk.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hqoqyjdj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2toafdcfp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2wpripedw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2oojypgni.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2dynlheoz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2uoqihkiz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2agqysfzc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zlmblntt.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aclhontd.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2wsmeavqg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2yfgycten.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yrbgsmqt.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2azowfpsk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2yanbifhq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2gvuibttx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2xtehqasz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2whdmtlgr.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2mwoirxys.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2xunyajdd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ccuiyzks.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2toxhtuon.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2tvypbxkl.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2sqmoxboe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ilnbtovk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rwwjonxr.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2utbritbt.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wueupzhd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xryzraks.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kanyiwis.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ffbssphm.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qmuiydcs.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2kuujncop.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uffiarcd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2mhueevug.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2zdcliaod.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pkfkldim.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vbezccni.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wfalbhvl.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rotiviug.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2jeiqxmph.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2vmqhqncx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cznwtyda.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2rcbythpb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zufzgniy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2grqgjnug.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vdafymfe.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2auvqbplk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fimoamxx.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ttfjmhhg.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2cxwsqgmo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2aubwmpzn.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2hipjates.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2joooapsn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2eipgnvrp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bhoaiqms.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2jzzywzhm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2xgyresnb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bpnnjtaw.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2dufhqihq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bpapcvck.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2wmaxgwns.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jdrzhxxc.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kaaefvvc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2uqfowlct.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2qaepnrep.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vzxbsnbk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2lpoozudz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2clbbktvv.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2qwsrpqbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hykrvrte.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hsmvxpid.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2wbehaqyt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2tzousgbh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ehyxdqqv.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mtjtwlpv.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ovlxzvnd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2tjdphdsi.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2bisdaqzp.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2lpweoyhx.html


<!-- 参考信息 -->