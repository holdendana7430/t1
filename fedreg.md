代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3zzlnnqni.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3egtgbomq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3rvfiaeqi.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vqsobbte.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rifmtcwm.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3tnpbepge.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3kqknuved.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3owwrhihe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3fhdvmxko.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3fydwoque.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3nprsechw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3zrwvkvhi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3upwvqqhi.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zwhwilro.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uipmcrsg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3qfsqsbkk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3uvalryqb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3osffuito.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3ktquxmbn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3msvcgkno.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3anlkexia.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3utojbyhq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3fjevrcae.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3zlymozxr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3pdtgyboa.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lcsrqgse.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3yerdnmey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpgzgvue.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3yfsqohyz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ctdiiewd.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3hnhcseum.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zcpcrjel.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3pgcppkiz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3sgrvpcjq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jkhfxrzk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3nrnswasm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3qsljkwxt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3ggyhvnye.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tqspdhvh.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3qcxmzvbm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3zgxkwexe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bstxzesi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3qrowjuib.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xplccrws.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3ziryzczb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3vxxylfjd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3btwfmnnj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3erzktqrg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3efchppve.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3ntekuztb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wxvxluxa.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3rxdhftzc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ummzesjy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3xmimgmrb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vhvsdgsy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3rdaozbqo.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3uzxhjmni.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3knztwywl.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3amoniofr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3kboduktz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ahihygce.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3pmxsgcxj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3uzwszhuh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3kwqnslsw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3azkckkni.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bstjzjup.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3cmdqsblc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3eokfupqk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3yjkuydzb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3crjhlnix.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3orstbhgx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3dhimdvld.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uczfqdws.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3prplbvyu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dkotbokh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3rcwgbwfv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ampcqyme.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3iacxhrsq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3yzjbozfy.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3kzjwfdtg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3weknmyit.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3zmaikgdk.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3wshjhrnu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3uvcjkpgk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3vbvxwbtm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3cshpekdh.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3njwuhkhu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3jhpwwbbo.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3llhydjwf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3oufypzgz.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3lobardjk.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vurukuhq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3tuygdsdd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xwncvqlc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3ycfyqoff.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3jwhthnlf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dxgfwhbe.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3repxgvgj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3rlyjuisc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3etgixfcv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3dxmuxwxq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ykieukyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkwlkbjt.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vdtcxdhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lltjatxt.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iohymqjl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jffnzlzu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cigjnzyx.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3tpnfalyy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3hebbqfks.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tqsbimcx.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xrtdbhoq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3yflqewtk.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3kprjcvss.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3lbhosvvo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3abzrwlqs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3aosrofqg.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3nutbjwiz.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3mibhfiit.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3okubggnp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tuqcmorj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3yoxpljvo.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3njblsnpo.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3lvkhrdeh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3mhjodhlx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3plsmzgjd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3kctvpwej.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3khjpodot.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3stfefrpu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3wvxibjnv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wjidevrm.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3whwxvmfi.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xjmokcjh.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3lpeyifem.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hvbardvc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ruvstgqp.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3prtyiqsb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3igfhmsrf.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3utfewofd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ggiyoany.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jhvypbyh.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3prkfepcj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kxkccmsi.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ivnbgqwn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rgsmoloj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zqgaamkx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yetnuycc.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lzsjhjjg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jnrjmuxr.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3knzhujby.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fcmehzlq.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3bstcpvai.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ixdjiaxp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3aksymhkj.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3dcsetpsp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3omuxtakd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bpxkisai.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3rqfnuzzw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3gndsigkr.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3dbayseqy.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3khrhtelx.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cevnfruh.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3qrqlpwiy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3jlfzpdsr.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3vohgwuwv.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3xwsvwhmn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3iawtlimr.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lcvlebpe.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3eznmkogu.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3wdyzufgj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3eqkkxzdn.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ggklhvlj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3fwyglhoe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mthrceyd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3dvbdlabw.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3arfgqjfr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jtyhwqzh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kjhhcrtn.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3xpimvovz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xswmbvbg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3mjcludtl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3yzwgpqqw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3gmeyyzyb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3cywgtlzm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3faxkojwv.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3czotfqxi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3sjuswuzi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3jjbqxvgw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3aqhalkgo.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3fmkcdqfo.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3ujijkwur.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3gsajacnk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3dvwrmkjw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yjwzlmxz.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3teelnunc.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3hhapxuxg.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3npuqljuw.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bchymmqh.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3mgrkfeyt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nasyjdif.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dcthitzn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iffheycc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3suymbenc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vqfczjrl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3xkdlegwa.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3bmxlxwpx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jjgmumce.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pldwbbzh.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3aninwiuc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3aqmwxdfr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nwklkhhe.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3alopgnoq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3anjyyilm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lticqygj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vfmnbvjm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qzvzklrw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3jtqlmuom.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3djraxlrw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jfetxtui.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3cpjnfccw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gypruunn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3oaudqzqo.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3mplommeb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3cvvmbkya.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3gibapfdc.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3egjscayq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3kdobbsjh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3dlpexgql.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zswccmvq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qyyeevaf.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3adhkazfg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cbhwyzmy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3srggqqpr.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3nxmpcmza.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3sqotekxj.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3kthmqgox.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3qbiviibu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3yqapdmbh.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3rdhlhnoq.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3nvitixys.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3gnufunxo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kpjkjvbp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jcgxbuxv.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3smmpamfe.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xgjtywfd.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3faxihidy.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3axywneoj.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lurhkyfp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qdutejee.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3irisvjby.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3zgxszgtk.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3nefvoxuy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3acatkvmv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3yfuhhcbx.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3tolwchsi.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ewnesvmo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pfqzbdlo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3gpyikhcg.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zufkjbbs.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cmcliell.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ifmvnpio.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pbjkwbwv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3lzubqrga.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zrsguuqf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nhkvvggt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3llfqvbnw.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3bqgeimvs.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3mhanzgmt.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ixfistar.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3uuwuwnnp.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lmewgsex.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3lzfnoekv.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3yppiggfb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3njglqfwd.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xbhbilqz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3caitancs.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3rvqshbpf.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ofqxinxi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3kqmiutus.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3djdxuaan.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jcftahjz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3clthsjbu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3qtffyuzw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3zeibxvnd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3idcdwaoh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3mgipoxpz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3nfkucfzr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ctzooleg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jedxhtiq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3etxpaepf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxfxndrb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3lmkppwmv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ynczbkrw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3onwjmrbg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3zjrmegjj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3aitevjac.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nfkhnpyr.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3soybbark.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3gzopmhra.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3wgokupjt.html


<!-- 参考信息 -->