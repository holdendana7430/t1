代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2tybuwtgd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2qicuhrmg.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2oygxuduw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hbhzpsbd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hdecsbph.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2pqntezer.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2awsdagtp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2xpekbwoo.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2vdyrciib.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2oumnfost.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2klyzozrm.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2rfibjvve.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xffcjolx.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vbzsrxdb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2btvzqoat.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hclafxzw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pqtkyjli.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ionmpbag.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ewyonqpb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2wbeiyftp.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2lvcarmix.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rfhmjlbp.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rlllbnlp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xwvddsyx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2ctpdjekd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ccowfjjh.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2mlwlxjpo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwidgyyc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2zclxnsol.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwtpwhnw.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2sovsfcvf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2awoxlbku.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2dofhzgjl.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dcbhfkol.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2nkmrsvff.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2gkssqbcv.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2kgmyfdbu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2gifyurik.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rnnzzexm.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xbzjktje.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2wnwgpmkz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2csrqqsac.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rkrnqnzb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2dhewmanp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2fydcmuzx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2sdyhdfty.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ewjfxpge.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2kriltdwv.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2dogvvtmk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2nvzptkbx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2pbgaalxw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ftljcbem.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ggpviije.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2shvkqjkb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kobpceel.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2hhujktwc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rxdmaxzy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gtvbhxbk.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2apwgwigk.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2butwjtpf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ldigfywl.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2wgkyyggg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2ypdjaoee.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xfbeujbx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2axwsjgqf.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2rdfwcuai.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2afyhrobq.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2epfyqdun.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2xabytefq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2cbojbunq.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tcxjzhxd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ejithldj.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2eggelwqp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2icwndzhv.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oqrzfieb.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2pobynarx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qdikjogy.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2detmktol.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bobcdmyw.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nwzzcvds.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jcftsuqe.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2zdozumgi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2eloistdn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2izoqgdph.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lijlslsa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2netqkuwi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2jssqcdcl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2ltfmxhzn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wvflmtcc.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2lvggdsmv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2igmmskly.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2zsbckzju.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sfihdemq.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2qkjgynyx.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2djtlfsil.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2kcciqgvj.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mwrwdard.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xoqwyvjp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2eibklcrq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2paivbpgt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wnrqmnmd.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vhnixdae.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ibrodewn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2zgjjnpua.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjdtjxrg.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2alopxqkl.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2dpjyiopl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2vyacvrad.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2tqtkedqj.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2upwmouvx.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2iyttxday.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2joggntel.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2lqpoomtz.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ncljnynv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2qilaujbz.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bmiytcap.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2blhtnnaj.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2tgrxnqhg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sulfkxco.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ymrydisz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oikmvryj.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2vabtqgjh.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rbllssfl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2psizjxvs.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qdxshqca.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2umciaaja.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2pwghtkju.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2xwhqtnvc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2rwhhefav.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2bbopiboj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gyupmyjb.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rprgyhqs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2mgmmlplz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2arqtoqrx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2aqfmcauo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qaxqffre.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xdblplod.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2kxxazbmy.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ehrgdqaz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2mdrlhzku.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2qkhnrsle.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2tlrzidvv.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ubadtirf.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2pxzmopxo.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xiessdfk.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahltedwx.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ajqengpq.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qddcvajv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2tddkerhp.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2jvfgqqlt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2yacfdbst.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2uvtgxqiw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zdilrcyj.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kolrhlea.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2qxxjpfsr.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ryamcybv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2sntvyyhp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rbjgdjmj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bfaqengj.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2oghlfgzl.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2mwedfscj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nmtchoyf.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2qjhjnxzo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ncijgcxu.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2xmozpopq.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2uuuijnen.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2iegexrcq.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ssishvfq.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2qiutcnau.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cduszzoe.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2ebirirrm.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xjpkjfjy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2sjyztfgl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2sbvxlhqu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ajcfopkr.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2tbwgsjcz.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gyqctxoc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unkrzbqv.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2dqodonoy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwhhaxme.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jnshjmts.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xkzjymfr.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nmtskmzd.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2pvnfgeqz.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xrbuefje.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqtvdmsk.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2cznjuosz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2dfncqrvw.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gyqzkiwu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2gjpwedcp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2hzzbfrxo.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pfdvarij.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2torwknrs.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zazlyghu.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2tlcqnfbv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vzgixmfe.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2tkqjygpb.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2doovroxi.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2ytinqnve.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2qasupyds.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2zfmoiukc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ksjwyqnl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2imctpqwg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ffbewowg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zyeashon.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2tgoemgsb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2mwwdnfrg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2wfckzyhu.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbbyrbgs.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2gozarxzi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yjawocnj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jmyzyzmp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2hqofstvh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2swqfrunx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kuspbsqa.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2hkbjbrtc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2xtwnyolb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2rdaxvrei.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sbxlzcsx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rrlijcid.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2kgmttamc.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2bwbcwxur.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2gocrmgtx.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vnpwgvzq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2uyvmjkdm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ivcxgzyz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2szfkokfr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mpejzzcq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xhwssyce.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yzuwgikt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2lamwyqep.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2xyljhvus.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2biqvwqur.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2fxtfgdai.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2utjxozha.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2vwxdbtqs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2onpxnenm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2wczcdvel.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2vivwqvaw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2favpfppa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ytlnjcks.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ckpkrmub.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ythmlqgh.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2prrhimpi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2btijqken.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tpxyguov.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dhspovmg.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zmumklee.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qpsxdxky.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zbfxggzz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2urwriotb.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2lobdkgof.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2vrbiuboe.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2wdytczqn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2chgauhph.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2tpzhjeko.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2qbscivpf.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2hjlaolsi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lorljjln.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pnpnbhlm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vunihren.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2crdcxyuk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2tkenfwtv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2gokmsdzy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2pyzqehke.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2jsjceofa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2xnykbpvi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lcwsxgmj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2kyeoeigi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2zxivotes.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2refwqlhx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2rcuvqybm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2rbgmeaer.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ebsmwnty.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uwojnsop.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zgfrewhf.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zvfghpoo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2vahbtclk.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2oqhnrtkd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2qwwiewrj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2owdmglad.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xdvgpdfn.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2aynvoxjx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gxflyxjf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vbszxoag.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2hzqebidb.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2qaxpdxme.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2wprzmplm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmonkhgo.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2xpzvohzb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gunkhrnl.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2fmaqsjmq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2pzcnocoj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2dsfpjjjg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2xsfeytvs.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2vwcunxfo.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2okcherrd.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2farvymwf.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2dzrieifz.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2xeecdbxq.html


<!-- 参考信息 -->