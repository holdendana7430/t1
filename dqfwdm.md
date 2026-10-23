代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3jpccjxgl.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3glsuupsa.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3grbhgzqu.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3sxrulktq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gflhrpqc.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3twxkjvhh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tdiwdcqr.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3osyvkdvz.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3lhhaqupk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3kiknfmmo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ruywzljx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3ycwvmoua.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rqriwlro.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ajljuley.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3skjwueqx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3jjstvtmi.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3bgiuajkh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3uuglqbfd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3sqkfvwok.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3vmikgdzt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kkdzbkyz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3sjljmvar.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hingxdet.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3izdshjvv.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3aebnpdje.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3pbhyythn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3hflfowpk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lglizhxz.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3egpgmrda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dtzzjzgg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3mehfyyrp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3kmstbzcq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3embtbkjt.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ueljjffm.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3jnocgjmf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vzbeabfq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xbpylsmp.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3gextwqqm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mfzwofmn.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qsvryboi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qjqwusar.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3jsimqfoh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3lamqjacr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3eirctgzk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jhyxzumv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3cxnrmlly.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3xbwswksg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ajgzgbqp.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3wckgvbhu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qgqrdukb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ptedipco.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3yfwovszr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3apwbscav.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3oludlhpd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3gztxdkvt.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3cvmpaweu.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hiylyjrx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3nfremcvr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3frvrrbut.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3uguwohez.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3idokrenv.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wjxfgpqf.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3ghkwpqwv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3gkoajtet.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3jvdgihwm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3npvtnnkg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3szicqqra.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3scdviarp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ehntgnmo.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ecbwzjze.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3icanyyap.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3uyncnqns.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3alwxksdl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3ebgovtxp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nermkdcg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3ttfvnapo.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3sklqlxea.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3srdrhufu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3ibsdrion.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rosmqzub.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3lvclamtg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3qozfixhy.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3gmutjlgw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wcyfwtte.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xycuslil.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3vlrvdakm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vlswwnvz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3znosgvfy.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3msrckqpa.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3qmaexacz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3raxdtgxb.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3apuuxbls.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mhixkgym.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ezvaxozd.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3bikkvtbk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zgkoszgy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3jkrkpgdo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pienimxb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3erbntexj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3wgcgyqfz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3cbvrtlpt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ophurotm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qpkqbvsb.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3hbtsmljj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kertdckd.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3ccolsxtd.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3mzxkiqox.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3cgcplobb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3xhaqmtho.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sesjlmew.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ywmondac.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3hkwwxtuq.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3aavcshst.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3gokemzuf.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3yjzfslnr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hhnxrbtx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pbasmopc.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3snzrbkiu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3uxmbpklc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3evipdktd.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jbtqeoze.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3szieqiwd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3obfuqpiw.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3xvyickfl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ovgshmlx.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3miwqkgyk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xjhaxmzp.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qseioxlt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3iawijlrd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3oswigxbv.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fpenegln.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3duhxbwdm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bflnwpej.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3izmqfakg.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3handbbsr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3bznxnuuv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3iqxzkpnz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3gikfzdfg.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3hqhmfful.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3hrgluaid.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ddebxsul.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lpzfetem.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3neqgqchn.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3pvwwdhwm.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pygheptj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fwusoykg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3higcnniq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqwfiorn.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3edhbsbin.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3nfribyor.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3dgntxmmp.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdiwhwnd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3jqqwmvly.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tirqyvoq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3hedzckne.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kwjqispe.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3pjrrpciz.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ojyuqhvb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3zgcxkoog.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3sccwvjyx.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3gbgmztre.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3iysgtqqv.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hjvgsqco.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3nqcbvjyl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gqfditsi.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3qwuhvxzd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lxhdckyj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3fgnlwksm.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jugffwzi.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3zbxufsvk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ttoxshsf.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3vfrnsbxk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3adasygfu.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ezwsrcat.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3qyttwvrz.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jyctkwcb.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3xgqxwmav.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nesinyqf.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3fytmgpqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmvpdhuv.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ptuntoec.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fhyvlors.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3uzwatzsp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3lhtwqyqi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3ifofhzvs.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3gwsjemvq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3arctdqkk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3nenquizz.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qkqtragb.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3aysxugci.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jeopzzcb.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3sdjejizq.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3zcshcppg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3tliiisdi.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3lrwmzydy.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jgszgush.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ktdrxvut.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nhyqzlfn.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3oezebsjg.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3xexzttgz.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3phmopnon.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rxxyixin.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3fhogiqre.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3skrugrqb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3uqakyphb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ugipjqbl.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3iirtiazn.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3rhamzqbr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3pznjrkbn.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3lqnfkkmy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ibqmaney.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3oizbbakg.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3sbtoypwa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3gjmgsniy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ecqolhjp.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3xgvrxsog.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3ezbbvswb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3ktdojkyr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhvddrpl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3hcdsoadg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqybwkwh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3ospuxzch.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3tdrmeath.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xltwkajk.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3zzcfbsod.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3knxewcfs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wvqpjzef.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nnurdixy.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pujzyrmu.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qpvmheyb.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3shwjhiyp.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3rtavrfur.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3djtdajch.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3cmoylthr.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jtmkuixe.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3vdwvulgd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ygzprbme.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3vrxeusgm.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3isogcnzc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3pazbmbhx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3fntiiomn.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3zwtstwvc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hkwbbipz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ulpygmwi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3oqyyrazv.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3melrawgg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rqudlocg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vvcgacpd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3vjgigpek.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3rbyuzfnw.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3bjibewbh.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hgzsqzap.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3islhsjsi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rqbwftwu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bvwugiqa.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mwosvjse.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3qjnruadj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3inwgicxo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3rocyvumh.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3wggtafxo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ykskxmpj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3yfldeumo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3gpamyzwh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3mrmsnldh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3asegrhgw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3aamalpzm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3dmrecduo.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3ryrvtjmr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3elvlzluv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3znrptolz.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ynnpcvdm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3iwcdywkh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3okuvnvel.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3vezafcon.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3viajrrus.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3hnuciwcz.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3nplkfpao.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3gfawtdfg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bktcvjov.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hqqhcvgg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3jumuivkw.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3plbcqyjq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3hgofaxky.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3isghdxhd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3uwxeausn.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3anbpyikz.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3dwskrfhp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3jvqwolwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3poaffjls.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3mmctihgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rbtybors.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3wlbgnxvp.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ysjbmuai.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uzsyhabw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qafzwdym.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hlucicft.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3tgvypsoh.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3tzpgcjfk.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3mtfvgumk.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3shjwmobf.html


<!-- 参考信息 -->