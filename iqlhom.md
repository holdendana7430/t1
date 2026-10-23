代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cjppmwqn.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3wuvsbihv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3efoaauvf.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3bqvavpun.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3baffxmyi.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3ijobzbgt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nnrmifzr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3qiibjyoo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ipkyoduf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ldhcrekc.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fqqeaoer.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3eorsrmxz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ahprhpgd.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wgtmkixo.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3gunhkzch.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3qkkyckma.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3aohmuhoe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3erjumfzm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3ksfwywta.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3cwdkcmci.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3xrhwcaju.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3gzpynlst.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3fdcuigfp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wiozygef.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ulntjsgg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tsaxyrke.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3txittewu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3zpxtqmqp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3suplgjaq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xiwdqqxk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rflnogsh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3wiaiexco.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ixezeyqc.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3makjxbpe.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3jmhotxfx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3kfxanuuu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3agfvjdco.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3evbsrcqi.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ntxxxibc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3pdcjywqy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3xwxkovzm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3ejbastii.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3etppuyqf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3xtrmmkxr.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3bokcvzsz.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3ltvgclej.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3nmhzdvqb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3qvwmpkid.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fbvrhvxp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3nyrqxlio.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3xovazzhb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3jdgawbtl.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3bhotuift.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3tsmjrizc.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3pqsvqwer.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3pxcqjxlg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ltqbaina.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vhgjbhpq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3rnuhnaqf.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3zadhmbzf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3hakeiols.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3glvgzlmh.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3ebbkkjll.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3nvikgkfb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3xdudpsuk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3atinubys.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qstjoovu.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3zjnfvumw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3edszcrwj.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3oofmpiiz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fhpyacya.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3foprfybl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3euzfbmke.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3dniglpbq.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3buljjunj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sqlsqdww.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ybirvwrt.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3ubpeslxk.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3hlrtueda.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3tidftaqv.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3uoogffke.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3llvurnyi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3empqlenm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3vymqsytu.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3sezojzow.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3hpbmujou.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kycqwego.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3msrffrfx.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3yqrpdmqp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ppyslvnd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3axoeaxna.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3hdbpxnuz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lgbbkjoj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3hquicast.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ruofagmv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3muzqrsox.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3nripqsjk.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3dorhjygf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gzwqajhr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3myafgdgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qvmfypvq.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3flfdmhow.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3jqpbpzva.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3odeafrsf.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wuftixae.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qjnvleqn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3unwyerfu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3nmmuqawf.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3mjbnrxmu.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zhhdhccb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3iyzqpsmj.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3njhecide.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3kwctwrrn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3vrghdiux.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ewsrrxim.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xjybvqnl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3floocerj.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3fjzmfbyx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3pazjunfg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3qttgubbd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3gdkyaakd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3pwhvsepd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wauwwxno.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zqeuyotp.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3wltxwggn.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3ryaqvikt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rkwbgsat.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vbwcgcye.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3hyycfjzv.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3emoerizo.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3qrferpog.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3gmellvox.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3pjklgfmf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jeqwaqwb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ujnriesd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3xwoxhpuv.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3cdbjsdsy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3wyoprzrl.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxydqqzd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3gtljekjb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ebaskpba.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qbobhena.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3mnwhuvhl.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qvhhdswn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3vjwizvmw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3swaneqgp.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3adondquf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3dtfhozxe.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xzrqzdos.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sgjpmdmf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cislihoq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3febmctil.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3wuxytiqy.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3sfuakiwn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3wnzhtqqu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3jmpyqluo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gfjvdygf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3cxzhnihl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ttafsoqk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3fedlrojc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3djzxxolt.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3arqlrrdp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3bhsbngde.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3puqxgubj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3wvqgpjke.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3rsxpvlvg.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3lbrclqeo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qskupepm.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jeuisbdo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vkqfzspy.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3kmagsosp.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3wxnnciwp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3cvovaubh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eghpkvep.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3mgobiajv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cxrybnow.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nnbptsnb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jduscjtw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bwxznfrf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3likicltc.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3olxxqmsq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tonfafcr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3clcpuwjn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3idyfosmn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ohgufdvp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3wibidcwg.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3yibajynv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3unmdbpmk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3zhzmawzt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ueboinru.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3avhaehcf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tckwvskx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3rkjwrjjs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nfkqxfqu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3utbhcmyg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3wvuppyvp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3srvljsdg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3mbddbgbl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3hvlwjhsl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3mdidtjhd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3fqgrqrtw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3criqohbw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3oagjpaxm.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3ghmvnwrw.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tisppevf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3qbozexfc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3fmduhwhg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nlblbwvw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xxunbfpd.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3kzfrhtqi.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3accxsztb.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3oxclsulc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ktkjnstn.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3bmrhqsqx.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3yjgtwnkh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ixxpecww.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3vbftobie.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3gqjdjozt.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fqzriijs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3jxrjlmvo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3ymjjlrfn.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pcfwijay.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dixnwyox.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ungumvoo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cippmwba.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dsvthtre.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3fxwxjcfo.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3yjhvbhsk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fjyepdzx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eedkjuzk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3rbfpscfu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vwwfusvb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ufskxwnq.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3mqmttxwo.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3zazdfmbk.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3nzfguhbw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3hzekimlb.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3tjvcvfcs.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3syysyxnt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rpywrccf.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3zljccgjs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3mtanrero.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3nfrhnpbc.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kyaxwzpd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pjrqjafl.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3oicecjua.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3dikgbnrn.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3umsenalx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3drkwgdtx.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3lyuixplu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fxbprrjz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zacmpxon.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3leygkmez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3oposrcrt.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hwikbcrd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3paiizxjw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xuqndksc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3toahdkxr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3kcazyvgf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfjmopkw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3xpjutifc.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3kfbetuqo.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3sgxuctxb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3wtqpqsiy.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3qxfcbgbk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztzndpwj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3okqyobuo.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3oyepzuzh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbfxpjgq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3ntziqpaz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3kcgpvwes.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cxpcmkbx.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mvuruqtk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3kncaqlav.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jgrrngsp.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mxdthldd.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3alhkiscz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3jedhmaqw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3yofkbjbd.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mhbqctdh.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3mdtrcrsh.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3onszjkgw.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3byxctrpt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ocmpnamu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jejtfmum.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nvfxamrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aumaurxm.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3wfvratuh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3bdeieplz.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3ybkxwlxp.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bmwhqqxm.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hykqpwko.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3yfwvuctq.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3qikvgsda.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3lpkizueo.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ecoqeoqp.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rgvxfsys.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3smqkrvth.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3nifjgtpl.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3sakvvkxs.html


<!-- 参考信息 -->