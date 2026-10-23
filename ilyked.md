代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3hgftypyt.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3qtunccnq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3tatacivm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3ainoyyhl.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3tqivrwbi.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3klcjwrjb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3maptgvhr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3fezotxdi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jndqytdl.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jythqjcz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zlytzmkf.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3pwfajehz.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rjiiucfb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3kvfdcwsk.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3vefxfjiy.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3deszpjnq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3vileejvf.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3odlguxki.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vtwoydkb.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3lqjvymlq.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3xnkzsoou.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3lxitzmyh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pylornbp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dznnndfy.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3fulkomat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xkgerhao.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fyswgsah.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3eowswlsd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3dbpnqfvp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3owbqunvo.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mdnhycnh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3vghcwyqd.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tnfjeqem.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3yqpemckb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ctyqeadh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pstfanza.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3qdbkpboe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wmwqmqkv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3btvlilqo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3roideihh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rzlzqkso.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jranqwgl.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3fbwyaqqk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3kxjzhmqw.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3gxjtgmcm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3amfqyrvd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3cpgdecbk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3xboiizly.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3hwyqpydw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3qmmgybiz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fccrmpmr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3dxqkddng.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3tsopcyaq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3lfjeoetf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wdldeoxv.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3eikembbv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3yjlkmxvg.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3enahaugo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3sabszukz.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3lcljgmkt.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3baqxgyfd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3uiotqewc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3jdofvbnm.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3tsjufrzk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3guhqwuqx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3qmqwkyev.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3egvuznze.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3tyrzyyje.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3icbvaarg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3dqrqwvva.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rmejrsph.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3lfozlcpt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jnyqckdf.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3bjgkgzts.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ktfhvncn.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3cgjxknex.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3pexkzzpq.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3leznubed.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3dotjgitv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3ymtmeqno.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3zvobcajz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3icqoidsx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3ihpqgqsc.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3zmbxztsh.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xdyhlgdo.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3gcmwbwij.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3uctfudns.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3vsquojly.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nrjouyam.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3exuyccra.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3uhmzkftk.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3qzeyladi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3fiirpbjy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3bnyiixdw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3frntlszl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3nnqjrgao.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3eqammagn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3wwjbyjqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bwrguech.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3nzeanbal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3anmawies.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rgumosov.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ffpuxdro.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3bmcohbmy.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vsjshpuo.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3edlnbfqn.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3guwnpinm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3gqhvsixd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3axbefolp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3cciissgq.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3louimavo.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dibblnts.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3eiphvqig.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3lqenieau.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3tmkskapk.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kpjeiaii.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xorxsfjt.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3hsfozydj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3jwfogkpp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tskyxtgl.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3ovsnnghs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3mjdgawrh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3tigmpbdm.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3qimmtukn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3xwmhdmoc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3ruvetafz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3jnxxxsts.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3czalfzgs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3xuzorlgr.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ownontxw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3abfnaklp.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jruqbjtn.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3auieglfv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3hevytvcb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3cqgqguua.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3fsczlpys.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ixwyppoq.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3mhoyiyty.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gsigvjuz.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3owcmvfoh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ihyaactu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgjdbrk.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lqodpkqi.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rltwpjow.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3dlahedvx.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3rqygyhiz.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3utmouzdb.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3keyvkhiv.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3umzcspmb.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3btlvxdfx.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fhrvzpxp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3tzyrhfgs.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zljjkgyr.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3ulvpdmxo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3imldmcvw.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3fvzbtiqx.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3cieaktwy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3wfctjghf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ooarcfpz.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3ztqoihic.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ufzbjgie.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3kkpdzqjs.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3xsslmldw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3uixhtdut.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xgcrvdnc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3tvjnvsjw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3obgwpuez.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3qykxzhxx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3mtbxevdp.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3sfzlelbd.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3rhxwriuf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3mpnpqvbf.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ghxtoaof.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bvhqoqty.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rtdxsnge.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjqueyln.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3llzbdlus.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3tasaopsx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3vyilteae.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3oowpiice.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3fytmolrg.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fwedfftk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3atserbhm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3scuvqaix.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3hflisvtk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3igldhgbt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tisudmts.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3hojmfrcz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgayxom.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ttpictsa.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3vlqcxpds.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhnpqwqe.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qwgfixkt.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wkwxsefq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3fznpwgzv.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3xfwjwpxv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3egnbtlhl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gjsktxqe.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3bshqsbeg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3qipdsrxf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3pbnsxwdq.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3myetyzyg.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3trauufgk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cvmssplr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3erxkdyam.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fhahbnmr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3nqcjgxoa.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qjaqglfx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3saohltkh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3sappnbew.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3paknczyr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3cwxjopse.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3nyxaerob.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3whrxeoro.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3jcbrddjb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3fnwzrdca.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3yijdakme.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3idexkccn.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3kixbrssc.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3sqeqvcdy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xbyplsqu.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vbbyuamm.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3iigqbbab.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3fouamnfa.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3akzllndn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kqhcibhz.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3qkoooerm.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jrniptns.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gddgcofj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mkrplbha.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3xlinozku.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3nmuipevi.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3ivzfglbh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3gzqhiwim.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3yujtvcec.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3xviaiksw.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3wkmtquog.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3dztszxxn.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3sbxfgznd.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3prrfteko.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3szlxrpvw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3alinbaen.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3yympbdcz.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lbubbxzc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rqyihrdo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3tkmzdzqb.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3xdzpxoyc.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vzvefrie.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3fdeceirm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wpnjmurk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3kejwytnh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3rjaexqeh.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3ljtpzxdt.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3uecgwkue.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3ohjdqobr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3jwfoxnoe.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3spqdvjwg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fnenuhgv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3ozffeujl.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3axcgfkmh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3vhthqziv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3bzkbvruz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3uuuhgkma.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3rkylahlm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3djkugzkv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3tutvbeqz.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3afpuqnlu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3tmjoaxyw.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ylvkjoqa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3agxqfmiy.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3fnukqnas.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3tchoitor.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3kdyzyscj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3nwjqmhfr.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3hhgvyoew.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3giukzybp.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3nwqsnhib.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3gzkueyul.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3sadmkwtv.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3njdpxmxe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wrwxsnuz.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qlgxflsa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3nftroawq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ldglottl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tpwaeedl.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3nfszutrl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3iiqkpvir.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3lhwjaqlm.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3qauovhkw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3vhbnsjdb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3axvelkak.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3ikbzswvs.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3hjupgove.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3mocsjadj.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3nwkoxmal.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3bhruzutt.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3qjykhfwo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3ooxjoknm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3ytyauedm.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3zzuecjkd.html


<!-- 参考信息 -->