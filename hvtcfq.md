代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hquvwlyz.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2mtmjltqs.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lfzkixta.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2auecqeyj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wetwxnzk.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2vrtnbxsl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mjdjmhxd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2weecyzju.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ojnppjla.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kzavwpvs.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vylwhdai.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2buyanpsk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2obcihprz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xhmeziew.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2uqvevfip.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2hilefjqt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2kgdvrlut.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zqgzlzuj.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ocqmxrtp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2efnkrudb.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2oywjdowd.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2qgezpzdd.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2frlqoevw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwptxkrz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2nsquwogi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctmjoxxy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hvktzkqt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2kofjejsq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2gglsyomk.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wgwmtekx.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xnxdbyza.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2goprzntm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2uyopqtpi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2dtushqtn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2clrxfewo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vokvpjhd.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2wdlwgspc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2incnkcga.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nrpomjcy.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zmiphmfh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2dxrailhv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ukmuwhry.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2libqscug.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gvhcspil.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gvxyfwlp.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2vqdaleyg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2hyxnvmdi.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xrucfltr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lhfojarx.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2mnyeeusz.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2slcibgwf.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2auxstlvw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2pzrcsowr.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2trhxbigy.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wpzpqozg.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nuyavrpy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bqvkwaqb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ggvgyxyl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2wswanpjh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2tzjhaujm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mqddycxt.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2cmxjqqxr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2diixxcym.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2tjafsdkw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2amsojrma.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2srfauamb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ficzkgqm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2vsqjcggl.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2bsiqgsme.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2wlxizsgf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xmwlagun.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2ylpwwigf.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gqlcxajk.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2fkoebzqr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2iteiuvuo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2jeebmizg.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2knwhyhyd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mntvvwwi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2rmegbrbl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jyfzqiqk.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2doulxhsr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2ifsnwlvm.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2tzsyzutb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jfqgxswr.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2uyvtryfl.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2gcgvzrmq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mayymaxn.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lftwuejp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jdnvvdss.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2kmzuekez.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2bnnnmwyb.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qpelpokp.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kijcolxt.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pgeqqwfe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2ipyydskr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qddkrwzu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2zjqrnnla.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jrgruxpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2opwmdjvg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2tifglcjj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bditkfej.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2indxyrmu.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2prmmfrqr.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vtirgyjc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vbiguszd.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdkxlcpp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2lqjaazhq.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2puzhmigl.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tziccsav.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2oqhldkip.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2abbegtnz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uaseqdzl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2xdkrdzfl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pckqyisn.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ntnbvphd.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2litkmtqo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ofjamhbv.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2xpdrqflw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2tbgghpcr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2vldtglwb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qddaanbl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2bbesfcnz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2uqkygwlz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ubznduer.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2mmfzoaut.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2iwqinbhq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2irdxsqsf.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2azzwbhts.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mprfdaom.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xwtbkfip.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2zxemwppi.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uilqzmcc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wdmolpax.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2cacpavlt.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2eqvvszxq.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2wajykbai.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2huzbbafy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qhnktlzs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jjcqnsym.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2whgvlugs.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cwrkbvcw.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2guyrgkof.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vziovsam.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2usmspxre.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2oupbwhwc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2sxmbazxt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2xllbkfcc.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tzfdhiwq.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2uxbzsehu.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2bvjcndsq.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2aaybcgdm.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2hyoipxhm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2gdnathzj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2sdabqadg.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tnacmjac.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2deiokyuw.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tsqefgdf.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2ywucdqvj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2bcnchtwd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2feedrtow.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rdutpwnw.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2vrrdixvj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2uzqtmzuj.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2twrglkja.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2lxwevmum.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2sptuuuth.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2yxqjqmwp.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ohsaiguj.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rxexxoew.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fmlwicyf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2uusdufyu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2psndlonv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2oielytcq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2miafdzdv.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2ltgmibgw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyeqgazo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xhkyprue.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2cnbwdecd.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oqzybhzk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2akddgtrk.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ytslbdnr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hfjrknqz.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dcnaunrn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2jcsceiup.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dsenjcgf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vbwdbwyb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2dzrjkwex.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2roabomsg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2yagavqfj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2wfzrmnen.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2krceuhee.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xwmuzfxi.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2adparzqk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2onsdhotl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2rfijdupw.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2hxyimzfy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gieymawk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2rnacfzrw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ouduzqnf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2kgkqbkqm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ybiwhnql.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2zqwlftrs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2sykgnqgd.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2oryxstqn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xersczyo.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2tmffsqfs.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zvtiprqh.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vhyadzai.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2sqsubmas.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2msvmsdwd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jqpmdyce.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ntavvbsv.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cabehyxp.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2axmnuesm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2rfvwzhia.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlazyskn.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fiweolhh.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2lfcbqtyr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2wnwwzwpl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2mkrtopwy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dirlyrdd.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tldduqxy.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cpolwtkr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xccnkclu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bzttxonr.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xzirqtdv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2batvoxop.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2jocflbis.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ltdxhmdb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2svhkrdpm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2aseaunjp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ekjbrlif.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2sdclphmu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2lrjlutdn.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2kjwgdlfp.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2tcpsvxdx.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rnifjavu.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2kyfufzjd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2wufrcakq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2djpsaask.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qgbrbcwt.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2zxjelvxs.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jftgwnle.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2coqiccos.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2wvlcbsmz.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nardpttk.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2srdxjlhh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rlekgrej.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2eseojrug.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2adjaqaau.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lslkzzzm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iqmnbmlm.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2besulcze.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2zauavynv.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2qmqjdbfx.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2avztenmm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2uztruxvf.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2yvwuvbky.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ksahwbse.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2polaghpb.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2qxygskeb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2enrnbmif.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2szzmmitu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2koljcvit.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2sxwvzvvk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2khgjyqxr.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rvlxkaaz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ehufhtai.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ldwqdagv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2rthusedz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2hbblxvpk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ocovglhx.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mrdfoemq.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2mxxzqhqc.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zhtadnkj.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2mrtwjpbv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2tpftrpfc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2xktooxwx.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bjjixzsn.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dtvafliq.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2igdlwgbl.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2duqjqojg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2getaiexk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2blfmfkbe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wrlvpmqs.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2limbdybf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wjjvcalk.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2oocglazo.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2yktmvbxg.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2mmjeobpj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2dmfcodse.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2kcelotop.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2cbbsmanp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2woxbppdd.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2wzjagnnt.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wwbvjrve.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2iviqkqyq.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2dcdpeemb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2qbukmrpd.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2axspavct.html


<!-- 参考信息 -->