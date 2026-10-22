代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2oexqxhjy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2wnejcbix.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2sfclazxx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2vhuuqwbc.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ffqkioym.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2oseoueuf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2oazovkyb.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2rgmhmcnh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nkrsocfk.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2pmgsdxtd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mffmlkee.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2rbxbcckt.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ripnzyqi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xtqzmbjt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2telatoqd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2mbejfgxe.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2estbjmts.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yypvoswv.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ysuoepbv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ktmkqcgd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2prdvujdm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xvwasavz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2shgalzfb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jtdvwdga.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2hwucqfxe.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2egtloaug.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2pjydjwns.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2uybladva.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hhuhlsox.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2dekfqyja.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jwptbfyw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aftpjsby.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2xmqudmup.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2scgsvatx.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2wlmuwtlu.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2pimjytnw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2gokiflsw.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2whjewniq.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2prjxqjgs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2yvabtlsy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2veusfnbo.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hjhdapok.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2hielxbdr.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2agpegsvr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2qraqmfjs.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2teeykwzx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2fxlbwrre.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wwwtelah.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bdqfhtdq.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2izyyjzua.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2pkwisqeo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vmgrlwsv.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2svijadoe.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2usenzpwm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2czwylmyt.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nsjaazuo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2yahlhmzi.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xuopjxvb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2clwapxzc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2flygobps.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zlvyzwxj.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hnmfzrxu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2satcqrjz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2gttelrje.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lwcziaea.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ifpsaraa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2rvwjikcg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2nshmroio.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2aecsompa.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2dzkfsmnu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2wgnemeis.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxncry.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ayzjlimq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2emcgdjjt.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rucvveyf.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2dbjaqiym.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2sthwiies.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ajdswpdf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdswwvdv.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2nwzpbgma.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ldncvghp.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2mpaublhj.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2omylkxrp.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2lrdugavo.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2dhrsngus.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2tlubhnvn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xggftlde.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xoicyuqh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2oismotjo.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2dlrjcvkz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2aljzllxd.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fxfwxylw.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2gwpzrohg.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2xileucnq.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2wsdbsuwf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2rqmscbqn.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ojgmdxes.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jecwesdt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2rqouvmvk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2rdckwexb.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2bptfckvs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2arlhrxeb.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rnejhhxq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2rjaiwqzi.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2qvotfeqy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fqbqzlom.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qifvqkyt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2vriddsat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ivzonzcl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2jtbpnhxf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ovnldlqu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zapsmxvk.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2odgfhqjh.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2brsomvtp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xiqefdcs.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qttbfydz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gegidkql.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ockemroo.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2gilucqlr.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vdnmnzjy.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2coklwvdy.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ezrfyvme.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xmdwyqrj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2caojgxrq.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vgewfpbu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zwfizjpa.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ylbojbqm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2thkssojp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rpdkmbqg.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aczvnfju.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2slsjaovz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wwcpqdfe.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2jieewdqx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jujrjimj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2cfngdghg.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2htlehgdc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ahdqfldh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rsimwdrj.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2hxyadlex.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2agsmwhmi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2guutihip.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eufmcxwd.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2tocnjqbg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2oujldrkw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2iwvtdjoi.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2oixrbszy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ayydysyt.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2fcorsrmy.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qypcojht.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dzwlqzgd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mkmvumjh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jtguoaxi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ysyjomqk.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2gmlwkrci.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ymqduljm.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ecuhmejt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fkuacauh.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2necnbury.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xkmgujkz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2isfyiufh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vtlbrxzf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2tskobkgo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cgarcmts.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2yfschttn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2yxwnjtny.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2mmnszgft.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hnczkydw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2jpqikolf.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ilmqegxz.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2meinymzk.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ltspzblt.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2kziiqocx.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ilnatwto.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2eotrgjil.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2buieehtb.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2lenuqzzt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ewfkquoi.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2zzfkfkfk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ydgdrdur.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2snckjpuw.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2slpfiygk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2swgvnehw.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2azdynwso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hejnnsbg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2uawetbni.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ckvmvpit.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2vabsyltk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2qlmjhmci.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jhbefbba.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vkctobtg.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2sjwkcbyl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2luhhbvhs.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mpbnulrk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2kaorufuw.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2dhuzpooc.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2tppyfbkm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2tsxtpjst.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iaswwheq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2maclivzv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2aojjedzt.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vmatujld.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2mpbcpnup.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2mbtstoxt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2fsxgmjkg.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2jqoqulsb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2othfmmwz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mrbmalqr.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tmvbqhmp.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2kjnemvhl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2bbhwvfum.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2vjnxomev.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kfcuvxvo.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wkjnwbwe.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2rvbrgaqr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pvpkeeqi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zjdiwvdz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2crohritw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2qxurnalt.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ymvvupjo.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ljgtfukn.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ulvqedvr.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2eguiizqr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2abduymon.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjledpjx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vamabpvz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2doxeekar.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2riafbcwi.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tiobczmi.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ukzxmpqd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zmbcdeil.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rhvdytar.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2isvbydas.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2icmpypug.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xdvvabgw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2dkqtcydd.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2glcwswso.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qlqffjvq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2sudfjnjq.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2jbmmldiq.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2scolwbhc.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2idejmszh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2watcfcqi.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ruwpystb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2hybmntze.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2agcdyulh.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xpcqwhns.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2oxpyqicq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2lankoven.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bvmhfjit.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tebzlqcy.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pqgltjgd.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2apxkzjnz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fhxabzcq.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vfsfxjkx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qrrstbek.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2leqxjrjc.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2pfeillkc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2sjsazwvl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ecxtrkkc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2etnyowja.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2nkqcauxw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2bznrrqia.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2sdeywtys.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tamzarqa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2xkwxbgrw.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2jvqpsnuk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hastxpbg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2owavxrxv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2hryqzqit.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2nisfcyea.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2oggtkcsg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2aqpvbwop.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2epyfnmfn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2whwgvoon.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qdmdsgmk.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ywhejrop.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uwaivzwe.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2wyjjujpo.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2iyplsxjs.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vzqushmm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nedjnotr.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2pntjuxdb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wegelkce.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mglnpgip.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hbngokdp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2vrzbrqjw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2dquplbln.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mtcpqnqg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2plllkhdr.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2togycerl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2othgkrvn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bmhcejfo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hfbndzlt.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2dvasmzno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wkwaaoie.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2msvitcnf.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2vqjriplg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2uknceymw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2leiijipm.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2mwjelphz.html


<!-- 参考信息 -->