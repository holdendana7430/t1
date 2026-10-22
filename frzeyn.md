代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2wzmngudc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qwsgiyds.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2nycqvspa.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mtkrvsjb.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ikwsscdx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2paptjeir.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2nlfoiphx.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2adyusacr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2uaryvaot.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xvsmieaa.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sitwshif.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2prgfxrog.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ccaqkzkc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pzukfjvi.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lxagjyiw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjadpam.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2vyndtccj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kgvcdvef.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2lyphbcvi.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2vzimrmfm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2aputhdzy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qnyxaabd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xdatvqpn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2njydipgz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2cxccnvna.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zclokujj.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hunjpzpn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iumfhslt.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2frntjtvt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nusidrmt.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2cbpxljoy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2punwhdyt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zslnsmvu.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbxpvwu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2qbfawssp.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vfhjlepo.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2nlpeeaav.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2qzicshzf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dwqxcrxw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2bakkambu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2pmeigqoq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hogluity.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2yqaxebut.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wbzzwvho.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2elqzjbkf.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xsherxmu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sukjnzie.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kfgrkzic.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2liotbxjl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2nstijimr.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2eqkrasoy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2djqfkziy.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gdlvqjfp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xdyevvme.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2derwzqxh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2vnjnuksa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wphoqdjs.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2shlsnqsy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2dmygnxav.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nvabtwfp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2riqlvonh.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2nywxjisz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ustjsyit.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2oiijwczh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2obyjityb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2xgzxcmfc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ojgpiewi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2qwdvadlb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ozuqqqsk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2duzbunsd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jkjfasvn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2yfkpnbff.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2phsmfils.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2iruebari.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jrafmyom.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2edbqngwj.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2njqtngmu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2cgeedixg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2htcncpsw.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2dazzbbrh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2aebnyfrs.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zxilrnwg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2vftswvyg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mbxveypm.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cxhcxwwx.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rahivzpx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2qbdtxbdn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2lmnvxfzn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2mioxrbcr.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2pkmtuiuz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2plniqndp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zejwtmtu.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2skgrsihb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2izotghxo.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2nvfmwhzm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2qugkjnit.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ezgodvyo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gdqbrcdv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ivgewngx.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2zrtcinip.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2pswgnngr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2exiwaclm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dpqfkmzn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ezxbxeqz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tuulqphd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2fvgtmqwj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2asvsjlrv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2cvinunnz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qsczsxcn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yjbmdbyt.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2gangtjys.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ugappbbs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2almfaynp.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2jsyszowg.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ajychthr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ippyogqi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2objlxfdl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2shegbkaf.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gvwlofiq.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yfxqpwvo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yqzzgjuj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2qeonvels.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zdbbijau.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qxphxhgg.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oxcmjdwi.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2gfosqavu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2hztckbbq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qynpafdo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2nkutukft.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2slvoemdk.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zxacapsb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2nciihbom.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qppofync.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2zzrhikmj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2byrsejqn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2omoppcgg.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2cicdveyo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2bmfwtmfx.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mnhweals.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ujwbaupl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2cxetrulz.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wueoxztu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijdiusky.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2dilxsseg.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rxbyarks.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rfdlhukz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oflnzlpm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kmlprvty.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2kkrruvks.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kbyfnttp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2osmvmvoh.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2iyusijks.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2vsaqtmsl.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tdlymmlx.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2ewezunma.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xewflrjg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2uydpttmm.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2oaczrdfq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rvxbcksg.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ghnpjnfq.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2mfnzhfdu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2aevoktbr.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2xxccarmr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2smfnffri.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2mnoxlzwr.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2hcatyugx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2kqmugwaf.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2mivavvbm.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tfnjdfwf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2gnojnrvb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2zmvrrirn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ztmyzpdo.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bczyxwjw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2yddnldof.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qzmuphox.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2rarxhutv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2yajwwmlx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mkohpeyt.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2qdvgqfrk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wozlekvj.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2hujxrgwh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2fjhlclzt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gvfgtwdn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jvosqedm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lcboopkg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dqsklovh.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2luzvzxri.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2kmkxvwac.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sqzehvqb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qpgjfwkx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rlavjmmi.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2luzdnvfs.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2imcppdvm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2zdrssndt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2lwzbmewe.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kukcyeuc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2spndrttg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hqgirkge.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2anuyfnuw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2vwtpprfb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2joswsgev.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2psfwakpj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ksdaulta.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2klaxghds.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2aykjucpx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2psyxgkrx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mkeabbep.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2sunpqgxf.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rhamnmvk.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nhkkhkoq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tggbfwht.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qvzczvfr.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pmjowgqc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2drlejrcj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hyxpywif.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pjgobeiw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zjsuyiuz.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2rmbeckxy.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xzysgmwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xvwbvryn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qiafqedq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2gnknuzne.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2otqyfrhe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ijpjhuni.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wfmjjpmy.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2czasnngb.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dibbsmfs.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mctiqcpt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xuqwzwcs.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2skdadfaj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2njdrnkll.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2dsulzadk.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2zzgvjcnl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2tinpeypz.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2wrnnnbeh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2qtumtkhx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2jdxoskbl.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qvilgzvx.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2sykfbnfs.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2qfooyvop.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ovvktmmp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gmuvwbwk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xodjjhew.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2tutvsdgr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pmalzklu.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2pnddiczj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ohxrvixr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2glkrxkzn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mcwavfna.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xqfxmaqd.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2cfyfzqfy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2iuzrprha.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2uytggeni.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2xoxrbujz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hrpaqsqn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybqzndrt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2uvitjjyk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2erexoccr.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2amwaedfk.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2cujliizw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2trfbmhpb.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2awrephcn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2enbobccx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2fhbhzpbh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mxsbeorf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ypeqfxzk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ghviggmm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yfzglbhc.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ohuaidsh.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zoolrlix.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ffnticuk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2irwshrgy.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2srkhonxg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ibagbkgd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2etaiaoxn.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2whwmwgbn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2rfctussp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2cvpastav.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2anjvqfjs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2hbxgrwel.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jjvuplhx.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2fbyfxkkm.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2weotblha.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2iulvkzkf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2hgrexxws.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zklgbwwo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rnbztwxg.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2mjpbjunv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ictlmann.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2gekrmglo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmyodhqv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2hopolybg.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2gpscjnwk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2zqvyawoo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2ishiwzxa.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2bowweeje.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ccxcprjh.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2zxbzxxdz.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dlbgrypy.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2bdpgncmn.html


<!-- 参考信息 -->