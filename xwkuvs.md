代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uooraqpy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2zufhxztt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ljzumbki.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fltarnys.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vsxtgbgu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2womdpvyf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xwpfwhkm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2cwzegwug.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2olznqkil.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2banupjtg.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2sposxvky.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2wsotqkkx.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2xqvfwdyx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2molqanjp.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wibhgvyu.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2atpnffls.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2zomlqkjh.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2nehygnww.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2hspwrwpt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bkfqacsy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2lhloalmv.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2tmgxriox.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2nasqzrxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rbydhzjy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2rsknuzcx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ptmdfyvl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jgjvmjfs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2buveodek.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2fjcnqxna.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2sizqxzwk.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2mvedwaxn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vwaghuaf.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2vlkpnjrv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2ntvimjvp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hqslliew.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zphnusoq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2depqjwzp.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2bboyksua.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2nqusqnoc.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2anvkpscn.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2cfhudkei.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zxkvsnan.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2lvwwrgkk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2wgadqdil.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2pgwtuuca.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2mwlcsbsc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2bqeqgwpo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qddetnfk.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qhebboox.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2ndwkhkeh.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2fozgmvre.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2gabzzciw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ctrzrmxb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2gwprrkea.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2pimpbyim.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2bvnwhsbp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2bfjxhucm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2vpaynuzc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2oahrmnom.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2vvgfvweg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2jmauzibk.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2kynlnzgm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2axvvdhww.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2nzlgpnbx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2miwkbwez.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ivmhgxbz.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2skbqgnjg.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jihanpxn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jsmotmhk.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wnlawwvz.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nqjyhzrh.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2lifhtjvp.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ixlbojxq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pahavlhm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2aatovdev.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xsbkehxf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2tmsvmdpc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ylkcbswj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2cehxfxzj.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2mskntgxu.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cudowzex.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qmqmujzq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2oculnxzz.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wafouaic.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tksugglw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2cuhcgxik.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2qleaivyf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2nlixhlxa.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zstfndxv.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ocrsbuhe.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2gqzhqzcp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hjrvpdwk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2edowfqqo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2chwrghjw.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2mjxbtuin.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qhcqoexp.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qxdhsssd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2iatwabvm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vxihghlc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ituswxyl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hmcqruca.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2fliwjgmt.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2paeiiknb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2oksyaett.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ovlfboop.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wiipskjx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2pfzgztkq.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ifcqckul.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2ygizntdg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wsmmwfkp.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2pzynhzuc.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mfejiadg.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ookwbdbi.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2frncebmd.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rsdupknn.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rhuwmpyr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vxjdqbvj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ckzlanaw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2khnseapt.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wyvuosws.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xtzcmuxt.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2tjduavkr.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iujdrjvw.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2aoofxzrs.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2elwzelcc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2deulxill.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2sgtybpno.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ajamjjwj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2irweueeu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2xhsaokws.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2rtozupru.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cckivsae.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2hcccnuzm.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2qigziwfm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2rhxkcryw.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2uelpopdb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ioaowvfy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2vcfdcvsu.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2aaqkijat.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2ltqtehin.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ynlhddre.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2iabhiuqd.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2oxvwwyzf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wlienwyx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2cgllennw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tbwarnyl.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2yfwotsny.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2auasdqmr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2maozoikz.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2tblyzpvf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2fsqzlsvn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mvkmilpg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2wiajfqlp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2kpqukyrb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2glvrqcbl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2walomehi.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wqnuggvr.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2xwseqdik.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2uykgwucw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2lptkxnko.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qbnapnyy.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2tefmjjmx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2acvultdc.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2olritukk.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qwzccpav.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2irrqmxyb.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2amszpkmb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2codqkeyn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2fphrkdrq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vmqoogob.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2akqkbxro.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zzjnaqgv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2krcgyuth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frxckung.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lcarcusf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2favdegwb.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ppwhfcma.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qzsprpmt.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jfpzwhuk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2slsnoagr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2idakvpqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mhccuxwa.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tdlinsux.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2eydowsax.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2guxhshkj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2lebgljuc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fjeghmxv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2cbhyigwu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vuugffqe.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2tvowijtq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2byccveey.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2cpbmxsla.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vrvdezjp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ovtxidcy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2okbehbuy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2nwxvjtku.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2sxuzkmza.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fygnofjb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2clywzlzs.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dlqiefbh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2llfmombm.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2kmvfiocr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2frlckzgq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2cuopoevz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2jimibnsp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2abuuewxi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kielptro.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xipbvfqb.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ohodvrum.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2bwahswid.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbuykunr.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2yoxaeojh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2ljnmztdl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2cqqkgsdu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ztidqgyk.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2znhpvzde.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2qjaylhid.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hgeghqhr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2neilssgl.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ijqlggui.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2xbxttupw.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fjikejoz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wnspnuly.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nkymqimo.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lvejzrnb.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2gyvfjixv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2njznwkqi.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2rqnueeat.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dzlyanqo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jyjgagtl.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2kucjvbea.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hkivjxow.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2svysllzw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2omvwfayg.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2yyaudqfo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2fmqfzqmy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2sknmydtt.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2dtzqwjom.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2fepdyfpt.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2pjucvtad.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vveqyols.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2umpnlpzv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2uialzupn.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hqsehffq.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2rwwjmiqv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nlvikral.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2srjfhpxu.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ntzqezif.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2lmwuscxi.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ohflhfxg.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2grmmkzsk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2inhhftcz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2bsmkwojf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2xsvtbgot.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2brqdaqih.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xhjulxoi.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2mhtpnabj.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2xvporelo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2kfzuszmu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2kjdgmrjp.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ujtbgffu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2ggafombq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cmureyrt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2uirpazad.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2hamonezo.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nhcbafwg.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2scfqabcp.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ybmpchxs.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2jcoevbyz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2gfpypqbi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2etoatayu.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2rwzfewhe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2yucmuuvu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2bgtrqlgg.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hnkvzipd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2pwjjmfvb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2minudlxt.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2utzlxfax.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2vttdhfuw.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2ltaxqxvg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ghvcniow.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2diwlzjnv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2zitasais.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ustkncld.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bnqbajfz.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gyirkrmv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvfbkkfa.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ptvzdwzq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2cujqxftm.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2jkwktgdh.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2kfrtkeil.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2eylxxpcg.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2avaxarwm.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xysewvoz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2zgetabnv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2ebqggxdu.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2mimkmkfo.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2fzzgkdvy.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ranyxwqz.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xxnzdtmc.html


<!-- 参考信息 -->