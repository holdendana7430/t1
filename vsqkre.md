代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wbtzgdpy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ccylhuet.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tpttasyp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2todzopik.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wmjchzjh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ankgalms.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2rnwbnehd.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2tazwfxjg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bbaqrpws.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ndaqheul.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ginldazh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2lpasvnjo.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2mqawsgga.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qvlfkbtp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2xirpvxpz.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gewqyzgw.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2aseeyyar.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jywnnjoo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2yxckdbhn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2mgezetaa.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2vytvzohc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2lopkrjwp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fwdvbdlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2izsufkli.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2lwxjedhc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kodfihvb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2lvdvomfj.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2tfwjznaw.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2ducknemg.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2letgwnwe.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2viqnntgu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ghcyrwgv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cllbatnj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vpdwubtc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dyrtkggs.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xzzsxbni.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gqbgzdqf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2cvmnfeur.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2aieuzmyk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2inujhvrk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2qnaqwxio.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2srsejadp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2qkbrruwh.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2iywzacam.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gfgjygdj.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2vjaxtoqs.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2wbjfgztr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2pvzimfkh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2adgttnlq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jltccofg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2dzpffgnb.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gqmdjnao.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2qdpxghgq.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2ifnnhcep.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2ghpbxfly.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vlabenuw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rpixvvar.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bwxhfpbm.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ejuyhpod.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2hbzxauye.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2egxcwzcn.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2jwhjbdpi.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mundhjbs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2dkzqayhf.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2lglaxlhx.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ocbejdys.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dbyquqhw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2fjzxtozd.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2ftcwlmtu.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2yrwxoaek.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jqohlfav.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hfnjduxl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qbznstgt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2lzkcrnyy.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2srsokchz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2obtgictq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2djkcxgcx.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2eldrhsws.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ugjvyaok.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2oznlqknw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2itajrxrz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fxnaazas.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2laqlbgjt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2vhwczail.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2nsilcjvz.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rhwpzmay.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2crgojgoq.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zwlfkptt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bqgyvdyg.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2wbhmdcsw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2miuphlqo.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2bzfisuxi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2tlrdarbn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2omzshrrl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2jocrkxgw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2cyggveff.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2xtkwwoji.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2asmfkktl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lknntoxm.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2mwxcsmne.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aedwqewg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vdygzlmw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2spibvoav.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mbmwyyzc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2bckpmvum.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqsqtxwq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2udguwftf.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tdhuvosx.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2epvycnaf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tgrsftuk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2ivyiviov.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2yxqbjuxt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2rsosdfxs.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2lifhpsjw.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2roepjlrn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ulawlfex.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2vwicitxf.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2htqjxmpu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hkbkamil.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2befvmhoh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2fcggxbat.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xzgpqiwh.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kqgoldhr.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ndwguchn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ttrdbtid.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ptrejvzy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2xcuqwqbb.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2fjgptwci.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2kjmrhiku.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pnblwrgk.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xmidwavv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lkvnbjet.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tqsbuiie.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2klkpjteo.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vpuyfvlx.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2fjyspcwh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2klpsclcx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2asguhbpv.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vlytekgv.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2ugfedioe.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yvfpzbsw.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bfxyyjwe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2udzrqnyo.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxhsdobw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2ebvxccny.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2kzkitwij.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ppeacovo.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2gqatvrnl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zmluoksx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nqqteilm.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lwlqunve.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ojgamnsi.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ncwwhcno.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qbuujvwq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2hcrznirc.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2azkvtwff.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ydwwkdxc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2wfkmvaio.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ixzkolih.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2mxexovlv.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qwditoxl.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2erqgkprn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2obiggvro.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2smkxmyin.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2bccbfzdi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2crwbtxri.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ipvnlocj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2kviiqhgh.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nmyqonxs.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2mpiptazl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2rlrtkixl.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xaialnvy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2xizgjprz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ioxbndog.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2chabyipa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hroklhor.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2dgeydlkx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xzwlcyeg.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ibvkarfa.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2siouiiyt.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jqmugyeh.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2mzaunecs.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohkdozzp.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2dlxtpwlu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tsnhdwgu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2qfoyysxc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2huzfscsu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bjklfgvw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2cvufenpw.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hefwcdte.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2zvfgrumu.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2onoxilgw.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gelnxvqn.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pqhzxujk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kupwdufb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2gioypboi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2ciusetgn.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2voqhgtsh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wrsffcyw.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2rxeisksr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zawoplvi.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2knbqbkwa.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nmrvveor.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xssyrjqg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2yofczhau.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2yrslqilf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2qivhxboo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xtlxedjw.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2obkunohu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2rpeihvml.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hfhxaheg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yunfkjcd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2rfxahgqk.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2aumuxavk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2mwsbmjiu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2muibobek.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2cvjycuvq.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2dpwsevgu.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2zgqajtog.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2ibxdjpra.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2gfnslhsr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yhoywbjq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fbtoqyts.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vwxxfqeq.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2omeaaeow.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvhjrynp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2ykhiajaq.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2txzttkqb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2tcztkxwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2crysjphd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2eqjfctlp.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vihkkqzn.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pgoumhcs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2afvgdsfa.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dgkcvszj.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2khphjjbm.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pczmedfs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ljxrroij.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mhsggciw.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2prytnqva.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2byhaqmvs.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2wmzygayg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2weppmdyh.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xandvtah.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pbxoebpv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2esmiqoeh.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ygrpizsf.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xconqyov.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cedejkbk.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ozgjpamu.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2wgoqiggb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2apjyottt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qpuywcpe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2gwdoekwz.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2vhvrwlsw.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2iypbjiry.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fvmhswpw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2puqohauj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ycycbsfr.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2mokejiid.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pzhxidxh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2bjvindiy.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2irowcelv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2xpmerqpf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fciexsrr.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2utwybtse.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ldsdwssm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gqsytohf.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2dwhreikl.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fvevcgxk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2vdnzzite.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2stwndzqd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2pzykizts.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2durgynyf.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zwrolkzn.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2wpihsygk.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2cxtbpeur.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2dvtxhmrq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2oxlmanws.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2kxecwppd.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tmzggtcv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2skqiilex.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ehjigaau.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2bkwajuor.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbnzoutj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2vvdkvmdv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ouiqdnpi.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2izosdqix.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2htrirlin.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2ybftkndc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2otdgflvz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2jibfytbe.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mdcckxco.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2bqqmyyhn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2dkutnrpg.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2yuapsywx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2iclqngqk.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2hffgdpct.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2rznvozen.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2xwpmubzw.html


<!-- 参考信息 -->