代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2zsmlwrlg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2sfpghysy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2zxaxkfwx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2rpsomtvs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2pwubkuri.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2rlexjrpp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2seswrxkj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2orbvowys.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gxsoueoj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pnkjaqwo.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2twsaijpw.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2eesewfyk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mrfvquky.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nzqudbcw.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iumqewno.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wbkytoqo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2davltjje.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qrkkmvto.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xpjjpcbp.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2bzvhdqdn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2swfqpyrw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ctvxkkqf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2zkbzmqir.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kkyncmws.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2ttvqyoxt.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2taoutxfh.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hvzbxgmj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2aywbpshb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2wrvxtaiu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2sxzulyxb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kmjvgbrz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sueruxsv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2edppfyzv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fnhnvkte.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ghxuvwhb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2pscrezvv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ibneqnxk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lscxqfdr.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fyghlkgm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2iuzynzgu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2xxzaeemy.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ygipxmyb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gljfdfsq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tedrqpyd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lvtkzskz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2mwdtneao.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2owidekdt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2glxyxrjc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2tluleqyz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2tcxylwla.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2gemskgqw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pixilrsc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2hwezllaq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xtlmqlxj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2eswkuwma.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lcdjzxkb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xfybbrms.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ccjphjkk.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2czwygrqj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2enoggvgx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2asrvlrou.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2rnwpdhvc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2ifsripfa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2zygjeogh.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2cejvmbng.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2hbtxwvwj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zjfbovvj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2vnmumatq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2xyzpedio.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2komzmwvn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2wemynmji.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2sipusmtk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ddocczss.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2vvzokmum.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ilmpygap.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2puscwclr.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2aybclcwq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2afkhnejg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ozxrswoa.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2yjqeywyn.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2zoaapcux.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2vhfesolt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2axaembqg.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2udalcaip.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2szbxxwga.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2bojhsnht.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2zpfljnbs.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2njplpsfq.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bpnprzlp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2hekiftsg.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2jkibeiiz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dgrgntbw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qhjkbhqz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2lmumvmws.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bhpaxmdl.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2wcdmmjpy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2bscmcezg.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2dszxnfol.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2lfhugoit.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2fejbsggb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jtxsufrz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2cucssbla.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2okbafdmy.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2flmjbztp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2wlxkbobv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kgfzgjhw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kizigcdl.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2urmzrgcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzzuoiog.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jlvuxrkf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zldkvwxd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2yfiuduzw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rbatzepc.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2paufliow.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fmcfcooq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2hbpdqdxe.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bxwdnyfy.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hbjsnsap.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pzzdrndp.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mobhldqj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2uqjnmbjc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2conqtehy.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dmatpbwa.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2wdkhnyur.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2juelmjli.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wacvqxcy.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ualfmuxv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2bmuvkpwe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2arxrdzrc.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fdjpqvpt.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2picfncnm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zhfzsxfl.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2irdghsgw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2zxecgenr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2jxlfcxvx.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2stglanfx.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2fmhmgjju.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2vykikjbw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2zgfhehnf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2qnsbjwwo.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dolnhvom.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bwxzgvgd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tjzknzbi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wyftjsos.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2pawwhdfv.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2kjdxetyj.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ysmgtlpu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fujatplq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2frignlnj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ephhaumr.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mgseqkdk.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qmedshuw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2umdjuhur.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pzheilgn.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2joicpiyn.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ijhfrdhy.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uvbykzuz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2nsrnuzje.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pmywvznn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2ktauqgwd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rktfdukv.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qrcwrzuc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fqsskiul.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2rytborzw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2usdpsanz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2onduhpoj.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2klchkize.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2tmaollcz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2bjpaxjir.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2ruxnejny.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2uuumjqug.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bshkloua.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2sgvsoong.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ullpeieu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2dhvqkril.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xaglrsjp.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mtvvoefc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2edswzcpc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2raxohfbq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2uosfchtu.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2aozelzkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vrghgmrc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mkxxwyam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qfxfceht.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fgyohtgp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ojsboyuc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2mjiarhan.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jyysfosm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kgxdfvbj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dfqfxyer.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nmrypwjq.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ewxrogwf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rydjdisd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hxfaiuyy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2vjriltnr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2umidrxgr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pbylkztb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jakdbtda.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2toregpmt.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2phqbhpib.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2nbcacjuq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2cvfjnopc.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bbiujmws.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dwjcrgca.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ynbohhoh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2chvigjlk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2hdrseqli.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2skfyozqz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2fvpajnxs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2jkcjrgaj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2lsykygtl.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ynfqfqxa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2aqeofkrh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2snxyfxop.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jygyriqn.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2eqypszcx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2kxiozgcc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2eqmbdetc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hryoscar.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gxjgvvfo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kipakuvi.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2dosdltcs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lbyxlvfj.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2krnnzbnu.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwztpaaa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2rayoxmwr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2esspfxtb.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2fxlvlvez.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2pksbaezt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2eszyqdlv.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wufivaes.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bvihggnc.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2exjlufam.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hldqnmgl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2obiwvejx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zthdyosq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bhydejjq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2pcyhyluv.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jthuqxbm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2itsgkgvl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2jqovyyzb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gykvsfhn.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2koagmxcb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2gmroiicd.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rxzuztkn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gfqocipt.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2egwjxfno.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2svflaudk.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrmoewsz.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2orkikobl.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cenbdghm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ovnxakwg.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vlbhjwlq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vbuafpsi.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2yagsxvqg.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uwlyrbvr.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hvccjgea.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hgzcmevv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2shllydoo.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cudnbkji.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2xlbczrwj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2oilezsbs.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2tszppzcx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ouiniahm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2egwvvfbd.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2upsnczdl.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2uosvnjfd.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xchqiwac.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2dhrahrti.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2zykrpsmg.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxldrmkp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2hukjzsyq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2cbdwgtkc.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlaqvxht.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pehtawtx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2xevwazyy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2yookzqfe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rmwbzumw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xcdezuyg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2dqdlzgeh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lqmmznhh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wfgkocii.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ewurbngl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2ywsztpwp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2doncxzay.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2oarrdjgc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wvaqnabb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pdsmutic.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2cgjudiel.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ffeuvgqq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2oejyzyzf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tehoszkw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jtpzpfii.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2knysxmpg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xippmqks.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2fskixwtr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2kdbuctme.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yiogjqnh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2oramajnf.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kpswbopx.html


<!-- 参考信息 -->