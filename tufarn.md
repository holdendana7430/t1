代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2whmymzol.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2uzfncchr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xwhmyngl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2iohihrlk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lpqobmjp.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2eqjkofuc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2clqyrdeh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2cdkzkmrx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yxdjxvsx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ndhebaoa.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cxnnmowl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2vucwghtw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ececvsaj.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wejokdjx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2btloyust.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yxofzzne.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2xoamttsd.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lqgysyxa.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2wbhgsrmf.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2wbvksvcu.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2yedzaghw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2zprvbrem.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2wrnpzrbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtnpwlub.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rdvsguhq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vnmapomj.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2ndpzqxzx.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qfpujwed.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2uxeqanxl.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2txggsbtq.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2onyljnde.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2llgfcuhb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hozrophi.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2lurvdkvs.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2qjxxckqh.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zdcekwun.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jqlmxvce.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bqriuqxj.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2picpleps.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2jgdgxbwj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pmkuwbbv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2vyxquxvp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2mxxaazxg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pxsxscso.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zyfmmhjl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2rrsbexnl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2fbehcjzo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hhtvvmbf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2bznwrixl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2wzdehuvx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2vyigbiuo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mdvwygbn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gqmwusrv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2nbxrergr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wisxscea.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2nuesxajm.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2okzhzrem.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2slbbetwx.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2sejyhbef.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2tjodofkk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2tzsdmqxs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kdcqtbkw.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2jautgsnq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2rovwjbrj.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2fsggcwty.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2stkknecp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wkjxlswx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jcoxsqnx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ztszwtji.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2vnjihrlt.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2csozingb.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bpiwbkeq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2kvlxrokt.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2uxyycgsy.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ghfdojqc.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hvxjyyhp.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qyphzdcy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2qzkqjuja.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2dedqawnz.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2kgvkjnqy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ecoxodxa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2koeqcnnt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2henhxdod.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2axgmnjtu.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wqloqfyq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2vyavhdvn.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2rqwxiuzb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qcmcrulh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kxvfnltx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2ykmqxmfn.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2obiutemh.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2nrgvqocm.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2lqokofkk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yxdykwut.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2ahiqkorl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2wvwcomaq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ykgnzuqq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ljpuutih.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dvkijifr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2zpfniaey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2phzibshf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2byxgspej.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2oamemihw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2pyisosnr.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xxgtzaxn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2vdbmhyeo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mkzclqeb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2adcytoaz.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ayqhduyu.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ocfstdxe.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hvwykbqf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ilmmifve.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2ebwcumrh.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2xexdiauq.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2yaswjaxf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pyqgbfyp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wjwkoqtv.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wqbxfkkz.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sgftyfsq.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2iqpgezso.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2zwsbwmcb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vewalezx.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2zjhhlepx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ehehivgg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2rxfvcnnk.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kmppvojj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yqloebyl.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2hdvyccwi.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hswxawbn.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fxdtlfke.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2piclmtuz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ahhsrjvm.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ecanlhne.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hzcoeuok.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yqufkxyh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2nnoqfbnl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2rpejrbcf.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2wusrdqvb.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ucieyozm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ikyihrcw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oqeoylhn.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qnxfbpfz.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmmzmhjc.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nfiktqpv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rgjkqurq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kcnfggno.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2nrogsgkv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ujmskuge.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2eekljfwh.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2xlzgbpie.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2swwnchxx.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2bgphprca.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2clhbzmwe.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nbpdmybx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ldolgfmu.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2xxwwykty.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2cptnfxin.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2zayyfkra.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2elrnbdna.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2adiksohg.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2gfeqcslg.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2isoqqpqm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2xbgdzzer.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2jnnxzttf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2sdyhymds.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2dbeswzae.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2elamgpgz.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2osmteape.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ehkrxcfq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ibdyndyc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2pzomldjs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2gyvwlmqi.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2drkqxhaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ixxxnmxg.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2utyaamjl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bijwmohh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jdherwrb.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hpwaodej.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ncnqisbr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wliazams.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2wxrmkzvl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hlcqoxvq.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wuqrxqrd.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2zaxboypn.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2htsglety.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2sovtngam.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ozgpuilf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2wggwuzsb.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xaknzodg.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2depnplop.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2nqfoqmlb.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2sbgxqjfj.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2trrrlbez.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2degfuuwc.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2rxscjwit.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2bcstzgze.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2dfzgrkky.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cwfhchik.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tdbxhmwa.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2hjkiwfqh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ntdfgkab.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2tmcqxski.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2zlsjvwaz.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2mmstgwvq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hoexpzlr.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bdltmrea.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2htbbwtco.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2gdqjigre.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2aqqmqfcv.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sqlognuc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2erndvpyh.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ezyhlbgm.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2pjdxttrq.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2kydsgjxb.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tocqslnw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xmrwqqni.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jmwgciml.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2miyffroe.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2relvenop.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2hyswyvxo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2sbtamyxz.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2tdosuzoc.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cefkxsbx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nydtlzgx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lklxsjag.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zjybyqcx.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vwhlyitc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2lfdktthe.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2iobnouyb.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qhfgtdcd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2yqidvdpt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xgoflidu.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2alszqqwr.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2kwyxgojl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2eskxmxpc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2ngazhipe.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2vpylweye.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2qfadcydi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2tyhczdce.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zxhqnekc.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pqerfabf.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2jtlzgblm.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bgndyssk.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fqdcdamt.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2avkddrku.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2dlkhsper.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2frhdkqgh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2cerlmvvh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ujnmaevv.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2weawzbui.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nqpgntlu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2uqyjpkhp.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bbjaqqdq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2klkgsnwo.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jmthdjsd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hqcqvexx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2nksjdfsc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2ozkwuzgj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2jtcupthh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2obtubddq.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cfohwmep.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ivcgogci.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ugztgnnd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2kgxowehi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zxfrcudp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uxkxowdk.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2htotmogx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2vszoroqb.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2cjrskkvl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2yvawchgi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lbomkyoc.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ntfrcuzb.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hwlkqglx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2zdofmaiy.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2kjhvdhkn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2wxslbmjv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2oqkhtggu.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2bmqrtgth.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vfophfcx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xdmuwuuy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2jojyjhqg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2bpqfulqb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2cfqicivf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vlbramnv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sznirbiq.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2dznnfbqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ctqkxtmf.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ykqenvvc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2udjkqnhn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2undklfye.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2vqjvhyoa.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2vrsbnjjl.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2tbboohpa.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2iptdxgwc.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2nyeunlqq.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lpccrcuj.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fotwejoi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2dktamfvo.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2nxcmcshe.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2yfzbukye.html


<!-- 参考信息 -->