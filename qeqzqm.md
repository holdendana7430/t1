代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3elnpjzou.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3kgloahev.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3fmwbgujk.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3pbxegxmn.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3xsblovwi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3fwbwqmmk.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3yqpvscay.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3dxbgbwsc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qzedkzgw.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3mkmskinh.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gbtcpuoi.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3dtenfxwc.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jmzvsiqr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3oqbpvywm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xquspwsr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3rshncpbj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eemwghmn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3evemqvme.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3pbbklmzr.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3kdtqmgfw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3jwvijvpp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ambdzmsh.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3keojsluu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3feklcrzw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3bkqktnih.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kplrlfwb.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3qxfbvwqt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3irbcdxjm.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3fdhkouez.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uekzlxsf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3swrulxua.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3viezkota.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vxufefbm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3upbdvlol.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3aqdqqcoy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3jyevrniu.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3ekvbzwgo.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3qvghtett.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3ctawcqmv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3lridkhnw.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ggpturci.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3uewxwypr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bgutawsk.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ewrdbavb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ukixrdfv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3pbfycgfo.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3wicyqgqr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3eyojqrdy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3vsqwhupa.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3efcjtrmg.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3xrlyyzxy.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3piaocqgd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3jpaxtnri.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3fpjemqze.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3uutvyzty.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3dmoaodgs.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3suqnoice.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3ajtkptcx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pyounxlc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dvnptcch.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3vdxnfsfg.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ernbjxyj.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3jybvgnrj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3mxddhvbf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zvwenuhs.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3fydbvapu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3nndjlmky.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3hduglxmq.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3qcfihqom.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3diexqqei.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3mtkthtlw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3twfkzphk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ybcrrgrg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lgksstcz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yrlpghmn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3dpkljwbq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3ewmfuyix.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3fwvspbxx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ckqtnqkm.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3gobfogwd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zyuvfkaj.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3swkbbdbh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zhwrvaaz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ecgftjbn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jnnzfrls.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3xdllussc.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3lgzregdx.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xkilwcmb.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3luhuqsrb.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ciieyjou.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vwjypbuq.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3axiyashn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3pzdtkayh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gnvflfzd.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3ynbapuvv.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3kyququvq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3gwrizdeh.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3avprsggc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3qoingxcl.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3zbkmxpal.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yfmmcjuc.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3slzwspum.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3joxzbiso.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3imaswfrz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3hdbfmvyl.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ylovgziz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gigxsvvx.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3mmysrbzc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twggliei.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pepjpvhk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3wymcisbo.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3bkgqrqgk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3odwgxrin.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3sennodvz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3wbfggeji.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3efxnvxdk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hzwxpnxt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3aauaccjc.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3eeuymnia.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mvnxzzsx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3pwzaqqhn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3ytyxdwiz.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3sbphcxui.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gmfkwayp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3rjbmzupw.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3iawjbknc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3otadbusy.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3rldsyzxs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3pgdswade.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3uicsmbwp.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3iwpeoxjy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3jxppmfcr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3nhflwmdr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3rpbemtjx.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3nrenltfj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3ocqkskjw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3suotbtdj.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3brbnathm.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3tdebhfwc.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hyecbgqx.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3zdaiflmh.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jrmwowqw.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3maufvodz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3akeosuxq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3lmehrkon.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xtffbpha.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rwayhtzq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3xgfikrds.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xqfuncqy.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3byrzljey.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ajkbylhr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zmwpezmv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3hnlgzoaa.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3sbkslduu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3stadxppu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3geiyopjt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3hrdnapnn.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mktvpwvt.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3omzffnor.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3mxgqnder.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3oauefuna.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jixkutnp.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zaczolop.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3wrllvkre.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3kwwydtfu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ppilganu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3bdpjcmuk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3zvmhsasj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3pxzknfec.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3vapzrsij.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tzckrwuo.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3xnnoslqw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3rjndojau.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3lbcybrzo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3skrucrsu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3hrwrlppt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lrktwpce.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3ygjxfqhf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3qlmsvbtf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3fuwkkccq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3gfxnamws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ekfrvgse.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3tmiuanbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxnsyrei.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mewxkjsl.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zwevxtab.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xidhtvwt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3mpgmrxzf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3jfjlklsq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3judhcayy.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3bvmeeamh.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3uciesiho.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wdzsfkcj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3skclgqqv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3nhohbvrv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3dltrdlkg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3vnwgbkgj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ajzgtryb.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3mobkqesl.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3zsffdwor.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3bqpkmdax.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ygmaalll.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3codxzqtn.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3ibptksbe.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gyrajpix.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3ohzfyygw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fncbxfer.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3tmexgkpi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3awbfcrcw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3lxqjuhqq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3mbuyozsx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3mrlhzvef.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3daralixr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ejlpaevf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3vthgmhhw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3itfmjpvx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xqkmjrem.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3mifapcuc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3rcqoyzjk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nnwyfpmm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3pqduhzfh.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jpalxbow.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jeceelgh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejsdxzwz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3wztirjoz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3efixeich.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3zkfbwysw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3npblerug.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3bkuoprbz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ykfdjvek.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ilcdkzra.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qcqipziq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jiyljsrj.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jjcegeaj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3hxufwarx.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3oruswrkw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nysfikwn.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3endmvhpa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3ljjasong.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3viwnnkbs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3rzuwsaps.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3nityiikv.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tfvxgxgm.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3sbbnzucy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xqttdtpc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kgszeuwk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3bxmmgctk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ycdakxsu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3azjsyqkn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3xfhbvuji.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3bygbegir.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3zslvtlym.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3htdwghpn.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bjqvgjwf.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3wcycjrnc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3eejllfmq.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vjnxrtqv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3ednugfpi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mjbfugjj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3thewfeji.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bmcfbxrz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3zsgnlati.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3iupggsqf.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3sogjgbyb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fygsxzlh.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3stjwojty.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3vhawmmcg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3swsnhheo.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3eykcsqog.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3adkqaxll.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3njihrkht.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3loxiwzow.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3xuewlxts.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3bjfsqnqu.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3hkdtiarx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3gwfgdbnm.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3yfwtsbwj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3aslrmboe.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3guhhnvrq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qnizpsyf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jbwuwxyq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3ptfduadv.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xmsyanip.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3hlvvnswh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3zgownyth.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3nsdfzngt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3laqajoch.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3etxhddxc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3llcqsbzo.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wocfypwn.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3swnlvxtp.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3sbokzaut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fxazrxjz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nnkzcagd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yikdtrpw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3rpzkimku.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3wisdmhnk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt3alpitqhr.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3bgcwkkdk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3qxrngnlf.html


<!-- 参考信息 -->