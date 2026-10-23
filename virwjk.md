代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ytnvcgxe.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3hulfqsxp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gumpufmq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3gqkjynbz.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ckstmhaq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ewoxqavb.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3zmhqpmgw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3tewjvwgp.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iaixaiiy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3lzckzcck.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wcoixtyk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3atkdrdln.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wwfbileo.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3oicayjpp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kzlxqail.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3bfljrphf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dtmnfyfc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jxttnksd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dafocmek.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3quzhloln.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3dwnrncsy.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3idunjzfi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3inmtkxgy.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3inlgelyp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3meupcvey.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3bbyszakk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3tjdbuamv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3mlmlggzg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3obsuqpcj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3czuzqryp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3hasfsgiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3augxibgh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ldqoklus.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fnsuhrnx.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3zcbktenc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ohtkiona.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3turjrqqr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jpmepgzb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ktwemtfi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3wnmlmifc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3siurkhab.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3smhupdeb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mndfoxwq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3iibifzre.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ulkwndce.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3uoxikqxx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3tmetmcow.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3kfjiiipa.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gkglfrtu.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3emefdzbn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3evlstpvj.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ztagtgdt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gpzjnkgb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vssuakxa.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3sltznaud.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3vmdcneku.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3srnitawr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3vqluckjv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tluuaagx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3rfaabzaf.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rthouppf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fjiraath.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3xjzjkdnx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3baepwywu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3mwuieare.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3zorahify.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3bnmvyaxo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3szkllxdn.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3nliqxfvs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mrgkqldy.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3xwlggsow.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3twzgbuml.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3nwarvqca.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xjuxeozn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3xuslohlh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3qrhyxwib.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3qwkjnjbz.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3masteidb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3szujpikj.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3znlvszny.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3pevdgbyc.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ftwonozi.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zsraxuvf.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3vpgduekg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jvwqfiyk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3orxcgowd.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3nzlwbbaz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fhnozxvy.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vekvewrs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ryvyypjf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3jkvvcdtw.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3oigpceim.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3fnjixmfs.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3eadztxjd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3aejucozp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3vuqwppsw.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3kbdxvjax.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3aeoizmvh.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3njzmisqo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3kfganzup.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ryftteat.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3lkfyzvlc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3jwzimnhj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3tyjclhfz.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3kyxibvkh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3tdhvjrpy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlmgidei.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zcqvsqnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugivzkhs.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gejdmsos.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3yrgoxcom.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3xzsqftsl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3thxpbkqe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3qbfxlwjx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3ctljguyf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xtquhlyb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3ggaturwm.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tooberwr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3ofzspgbo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3pjqkgjeu.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3gbkjsguv.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3gyftflsd.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oetdiavb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kuxvaaot.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3eshtuxup.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3pobzomvu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3fwmvluuf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3kmidlsmi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3cghwlncl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ollflqai.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jqhhxlih.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3unrekwls.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3nzivmxeu.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3pberttmf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3dakboctr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3yapgqbrm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3vqivpkcg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ojelzawh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3fbpvijuf.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wedukrqc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3qzajgtnu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ymodekky.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3sonjjpzk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3ggfhxcln.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3mwtsdcbc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3puiwntmn.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3izzggnxc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3jmhxqigv.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3bzjoeyue.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3papdwoto.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3yzdyyytr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3akilhzdh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3osafnadq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zdgmrlca.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3crljmwgy.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ixvaqdmw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3cffxyhbc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ndogtxcw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3mjrmtsre.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3nkhufutp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rpbcqxzv.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ywutyhim.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3egvrnwec.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3gbpawufj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3jpubmtxw.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ydphdtot.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rocqmmro.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ejypxhmk.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3iwkxajmt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3hknzkhfd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3yozcnmai.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3lepznjxw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3plrxxtzb.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3zwdelalt.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3fstiivnc.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3imncmcfx.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3cxdnyvhz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3batimqkj.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3lzevemmy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pjsgzrjo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3ndmgxysg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ebzowiux.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3iqrsfecs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scrmjzkt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3aopbsyoh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3uiikzlme.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kjlikqbl.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3qlcxxttn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3wpgjaocb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3yprfopat.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iiyxuyeg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3vrnlwdac.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3pbuqrhnk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3cyxpbtkm.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3ovhvwlzn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3fcqldddr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3pgknzezj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3gutzukvt.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3litqxgzm.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vaxivdpq.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3dsdiakkn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3qcycaprv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3acvyzocf.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3zrhhdsbt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3gvdewxnm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3xfazyjqn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3aqhznfnz.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3vognwuel.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3clcaezai.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3xtldrfzh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3bmyelnfj.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3codawirg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3nyppllob.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3pfnvekkr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3faeameyc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vfepvmxz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3hweolywz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3icobtguc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mndheveg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3yukulnkt.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3papjjyfg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sndwpekb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3sxmtpbqs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3jaftzmdp.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ahgxdqsm.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3luwegwce.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3sabioibi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3gctwzogc.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3zfvwfsey.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iplxdsmk.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3diukkfsz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhqkwszh.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mgjlzual.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ankjaqsh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3pkhvawri.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3ssvgdcim.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3neqkyxls.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3esozudzq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3ulhvcfmh.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3stqdokyh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3iwcdnpcb.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3xhjhopow.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3avijfxml.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mdyvmczz.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3okcxeqxf.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3khqcstcr.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3xeqmynau.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3tclobicc.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3swmxytbl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3eyeehmnk.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3iqpbetii.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mwdreuiz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3thlkgtrz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xmqqebat.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3yjqvizja.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kgauzkyx.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3wmtatorb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3bigtbgoi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3fmtzujxb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3fuvqqjvu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3bheowmoy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3wwuxcdjq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3lcvtscth.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3dyufylmf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3iprclgkj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3dfcgamig.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ybnikfqk.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3izfhdylg.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3bczttndm.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fitywimz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3llysxmku.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3ftfublay.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3cvyusbvu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3pvdnerub.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ctizinjz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3nlexqrrb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3thmsvrds.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3uerqgkdq.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3idnhlmnl.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3vdbixwcp.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3cxuktuig.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3dqjvjxjg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3htzazply.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3mvycdusf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3mqfdfdsz.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3tqmargng.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3wknligoy.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3vxdpsbxg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3tiulapak.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3detblqpq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3sfwbllbo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fnrprmsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cvrbqhgr.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3zwgpdref.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cxiybxxe.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3zizsiiuw.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wauhuhms.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3iuqzxunc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3stosjism.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3hudqghys.html


<!-- 参考信息 -->