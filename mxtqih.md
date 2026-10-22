代发 wailian999

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kpprgfjv.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dpitydew.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2rmxeltym.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2djopklgv.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qsgexqol.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2qmlzkgdp.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2unrkyido.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2ngfxjsol.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2awzkgvvr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2rihbvaii.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2elrefiyu.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2lovtcprs.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2xdykmnfw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vzlgcchd.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2holzygwz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2iqbkeroa.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zwrjllqx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2prvafatd.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vnijmnli.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2gfzetkam.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2kvejwiey.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2cxmfswwo.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rswrnfcj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2wjnkzhed.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qkkcitsp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bbyljbyx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2thaxhbgj.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lrcrglka.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2pnrambki.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2izjojxcd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2zddxqasm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2bkxiqqod.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sdsfrvxp.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wjishrtd.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jfeezvdv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2msqwehab.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2znzgsjux.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2aprubctk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2dhcwagis.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zqvvmycy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rprkojct.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vuxqefzo.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2xsneghsy.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2gpkrlvrv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2oaejqrlb.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zmlpmcgy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ptxvzihm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2llkwwcao.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2psmljpvu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2hgssibxc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rhytokqq.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2onaknszp.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zehyocmy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hordhygu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2sdpkcoyo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mljbzwyx.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2yaxjtjee.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xgmchuox.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2fqikogup.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2pluhrtgh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2zdavjmpx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2aiefbugk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hodrpgyb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2dakedtqe.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hcxoihzl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2rtgbmuiu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2pomqscjz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hzvneosg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2vqjztugn.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bbftrnhz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2hhovwsgz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tychoymd.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2anxzwhef.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kkhbvkvj.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zvazpmwl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mlffwutr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2tpuvvidj.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2lpbbftko.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2jikgohpy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ijwzjecc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2ktyrreaz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2hujchxvd.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bletcmia.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2zibqxgax.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gdqgpabr.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kvcfkjww.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oysvuwzy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vobulmkx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cmhydnig.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2rstdkvxc.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rbghigeo.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rmpxwhzz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ltvippyr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2iakyjhio.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ksnhggfj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2mpolcdik.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cwpwavve.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2obpivbcp.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2oaldkhxd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jlgcjnnr.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uwaglqgh.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gvcorwmk.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2cfeorosf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2yuejwaae.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jekstkti.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2pgxrdsrf.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2kubxdhke.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nqdshdfi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zpuagfbd.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ovmudqgj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bwuaolfj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2tzsvtqfe.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2lxoccojh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2fiopoaee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ntbrirnw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2wkwzbpxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhtudold.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2llhihted.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2sspjimcy.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wppdefxj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ikhcbwfm.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2fauecpem.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wrgjpxlr.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pmkmzarz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ejoszaow.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2fybyavar.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2thuahxzc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tcsmoqwb.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ylvervzn.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2sqxlpxxc.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wwwjdtrv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lkdxmzxh.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2yunjsocm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2yxjtfboj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bjzgiqkz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2cxvnhwuh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2tipcluqn.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2osrmpwyf.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qttxtxkk.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qtsizjua.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2dafxmubs.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2kfimmknp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tljdtyzo.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ydutyxvw.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2opcomwwm.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2netpsdoy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2eliirinj.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yjripftg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2oygeduhx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2eezqyaqs.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yufsxuvn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2odewzmix.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2kultlykq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hgifczzk.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hmrrywsj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2fhqmeuae.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ugeupnjq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hicrauaw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrbobvyu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2wqatcsvs.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2evokyrla.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2dbzqbtyh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2uadawcaj.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2eenprioc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qfomparu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2cwzsgbwn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wfosgirv.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2olrytoxj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2nejlcjyl.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dckuzbao.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bvrdtcmt.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2nwmuzqey.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lgedtiqu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pmullvjl.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kipzpwux.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dpaqtkfz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2urxvhyqb.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2vhianlls.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2jgvrziko.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2znlhgpeo.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bfasasnq.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2hrccqrbe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2jqgvhbap.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tahcavlb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kwokxzqv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2rxioxzdx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2huordzbk.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2nvyvbwuo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2buzlkbny.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xpephnvc.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wonbhwtk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvgdefki.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2glvkpanr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2stovnmei.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lkabzwhp.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2cbqkixdv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gaxrsfkf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rmbplkeu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sevbdfvz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hueytyjf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2sztezkzp.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2dexfzrwj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2hyovczbx.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2izkryfuk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ufnuqdgr.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2gznkmjqh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2yxlctjno.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2glansocf.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2owljexin.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2lfdvbmvp.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2qrnqfklo.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tlyiygnl.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2tblvpjgd.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2mxvyvtal.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pkilsfzt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ldhvqmko.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xqgsroqc.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2qpjphuje.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qytifchd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2kxggehsn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2jwoftzag.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hfnyldsp.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2indhuipg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fywotufp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jzqdovnx.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sakpoeer.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2fuxnledx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nfhrjwud.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cnaopbvt.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2knllaksp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2uddvtwjk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2wnolzwcr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2immpigta.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hhhrmzah.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2nmkmepvp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2nlrtfslr.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xrazdfmm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bbubjgzv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ibuotitu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eqbujsir.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mcgkiett.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hapbatxc.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2liwmplyt.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2upjrekhm.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ewbwanmq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ppibylkw.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2nazxrxuo.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xgmothbe.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dtlfyuph.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2clwhmdnw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ptjbjjbk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2chzrclaj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hnplarny.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2sibgpyov.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mksqetyg.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2bwwvipba.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vyzylgko.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ddgyfsaf.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qnufotij.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2mvkrzzji.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yuboiqeg.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2brlyudvn.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2brmzqhzq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2xnteexvm.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yxeejldc.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vzjbikgw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dxyqghpe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ekkqbaai.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2owzkrffm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2hikveoci.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2oncjiupq.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2kmtawmpe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2bexabhdr.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2itbigebs.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2gygqzjzb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2faoequmh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2eyimmrzj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2euwsdoqd.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qewzsvjq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2gneomfti.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2avyzdsic.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2aenegtgr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vaqrcgdh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2lxhumliu.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2akehqjyb.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bpjpbwrp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2yukhhshl.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ghpoussb.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hzbraxkc.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2jlhdlzsm.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wexfsklr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pcxjpfgi.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2maglnryu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rvrrntvg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2zwsfvvuk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yjzmizbs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2unjuhmha.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ozdtgarq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2vrkxwtvr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2pvhwwpno.html


<!-- 参考信息 -->