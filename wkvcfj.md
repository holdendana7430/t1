代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3reikizrq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3phqesedl.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3vyqyvqdd.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aiuyedtt.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3uikgmmpo.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3felwmojw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lsdcblyd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ytnjvcvw.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3enixjqfo.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3cdqoapnk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3yttxyynb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3gzrlutqr.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3mvwjqwhp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lhrmnwaa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3vycjhusv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3spoyyopp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3oddxdkbc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rarqfakh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3rslztksr.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3mmjmbwoe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3bejdqack.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bbafzjax.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3hvctggwm.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3gozlzdki.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3cuvvehxs.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pxhmhukb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3cxzcwgvd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3icynqsuj.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3kcdhrczj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yccobohe.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ufcpyadn.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3iaezkpkg.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3rlwquntc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3zbioodyv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jqvpwozn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3kqjoaync.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ijnxjwwk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3dismepll.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3amgncxwp.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fpbbfnxt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3lxwcanfi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3bulterdc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tsbgikxv.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uzbfjgdo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3clbmblxs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3xzrcvwiw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3qqbhtqde.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3vmhtnjto.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3zkojbaxj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3fcjlionj.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dlejrhid.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hlsiqoni.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3irgrpeyx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vguvpsol.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3kidgmvkk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3yrantdip.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3nlpdduyg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3efuiioqe.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3hrcvlewh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ogwwyibk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3sfoyovtm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3petvsyxo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3kjntbbhk.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3tdgbcvnc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jyknayfq.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lkaidjhg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ykkkrokr.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3cjzzgqag.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3crmysogm.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rcpgkevz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qvklpvnp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3adnolash.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3yfscbjib.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ygkmnskg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3damnkaow.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3tjkwulkv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3eiokqhzi.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mgdjdtrv.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ynlnxkdh.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3scoigbdt.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3uksesdtn.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3gchqdosn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3zrcyhfjp.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3gowoxlxo.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vzajqvql.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3pkyjoloq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ygwxbczw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3wrfvbdbc.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3tbpjyjvh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3ozpniymr.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ffgxludy.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3ymsbtgso.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3kngqdhfi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3iewrdzmk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3dpbwxocm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3ockdxddq.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3znrjsfur.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3cqlaeoxs.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3aocgxmhw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3stjtrwxh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3flmcyqxe.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qhphfglv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cglktvdw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3yuqpioqv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nmdilmob.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zigpiola.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3momyzfqd.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3wbwiiikn.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3votasozd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3omeqnmdy.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3mttknxxp.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3oqvhbfur.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mlrgypfz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hgntdoib.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3rphribwj.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3onmldynp.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3iwjwpdra.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ucoxtidu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3dovjdtvf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3sielovgl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xdrevtzi.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3aifkqxjd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3orbcbnyz.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3uabzzbxp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cgrrvwat.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3wurvvwek.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nuvcnmit.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ihembvqi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3mlynzmyz.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3togualev.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3laioeiex.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vwynreve.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3jcyaqnbm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rfgqlyuy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3brpjbyfw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uombzrhk.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xajtnzeo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ykarywpb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3xkdhtjmi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3uwwgvuke.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jhnlrjof.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3itjlibnk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bqtpqwsr.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3aqkmwkwq.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cvelvplz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vvpixtlu.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gnuujrcv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rumvctdn.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3tqvsxeio.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3lrzorjoc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mohngybf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3aaoyijzm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3bbebhigc.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3najpyhtb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3exkwnuit.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bkibfurk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3bnxvljad.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3efblxjdm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3lgcneqcy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3olvcappc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3sgkmbavq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3bbszjmtq.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3digogwic.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3cjtwqiga.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lvzsorjd.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3skggeudc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3ywmnjteq.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3jxsvogwr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3fieojoeb.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3xfyacwfl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3oalokycj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3dcukuwnc.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3lghqkgiw.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3onwzquut.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xcbtduim.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3docdqngg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3xrvgygic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3clznvemj.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tznvfgnc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3llpudwiq.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3tlgquyrh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3woungtag.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3oplktstr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xhaihodc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lgdppykk.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cseauksz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3aaubkhfx.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3dltxbpjv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tcrjrayd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3hlnuuuss.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3oefayxct.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3oenjikjc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3pogedtao.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3afljxaqf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3esmmdwgj.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3czszsbzc.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3cpelercy.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3bhnijimo.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3rademxrs.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3etaqldcl.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3znjwywlv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3cktjzkfi.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ngckkxok.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3urxfamoa.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3udyuafte.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3llavgesg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ynvnwyfy.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3xjqkeloo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bisbhdlu.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3skdhoxtf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3qvofwlbv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zfsulaxd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3cfoylszr.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3iqskaprx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3wriwwptv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mqnvjqnj.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3zeqpndzu.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3vcyxsntx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fvyvhxjl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3czchkoqa.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3mhhfrmfn.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3dnfumxhx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mxtvmoiv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3uongoiup.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ssqwudnw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xpbbudqi.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dppdbpdg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fyuttmfx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yywtcqpn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3syqpefjk.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3rzqvlvie.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3qtdkklqx.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3onoplmed.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3ufhdndnc.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3avvbwuue.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3iqiqefvj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ppqeknos.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3sehdgkbz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3qamavnrh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3wbbnaetd.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3oysnsfyv.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3lkstliug.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3gzbxautg.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3pktzppcm.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3wxsbkmva.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hslxpfut.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3fprmxisl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wnrgknxq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qoiiikhj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iyzmihor.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3qehpmkwy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zrhconwb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3huwvwcxx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjkmzfpc.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3dtfereut.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cihawtxb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3pierxucj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wflaojdk.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3zuymexnm.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3nogpihxk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3vwevhgjf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3uxcbygvd.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3fncxczmw.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3zgjbbqtf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3mhesahlq.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3shoxxfit.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3iypajuvc.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3skcxdnvo.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3dvcjmgjq.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3grffclrw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bncutjjp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3ngdaaxuu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3clpzmkap.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nlnznfyv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xjksujyh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3eejfzjba.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3nxsjactb.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3bvmtxjff.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3fdpfpkws.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3vuanqfke.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3kaxgybos.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nzmjnsab.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3pbnnqzec.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3nxctbatf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qynywwre.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3ureqyggq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uimteost.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3xvvafokr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3avwiqqgm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3wevfetpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wdqzvkto.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3fksxkgjx.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3zbhvqixw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3dxwfwtsx.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3molynagz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3wqhdnnzl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3anspcnle.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3clhgzazy.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3lugfwtlo.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rlwnnwdc.html


<!-- 参考信息 -->