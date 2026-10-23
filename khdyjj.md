代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3ggkobaih.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3hsdarxvx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3dnroomnt.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3rqcxuwyv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3caumfhvq.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3uffzilqa.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3eikxdwou.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3uphyxppu.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3mzmysjaj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3vjnlbaad.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rxttnxuu.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mdldatvm.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zmsqvggn.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tevrijdb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3aflyqdzt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3ixrlcwzf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zbwfrscw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rbboixyt.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3wxpiqxtc.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3hssomxft.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xiwsamih.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3lolssdrc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3vkcqnmfw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3pojraenb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ukexeebf.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3nchpjvgl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3osbajzjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3koaxmlyl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3tpcntevr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dpraurbc.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3yydldgyb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3cnwvxagr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3mocuvbdp.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mxnuvndv.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3xyfszllm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3jmtkhobu.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3bmvigwgv.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3cviwofci.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vttxreak.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3tfwylgnm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3ymqqlapd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3dgjxcbmh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3rjlmkmcq.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ewdogklk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3omyrdgpx.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3gjuyplfs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3eyirbqds.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3sidpukxb.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3mwkdfdjk.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3bqpntgle.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3xfjgofwl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wajieftg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qhovpuqs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3zxvgkxet.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3nildwasq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3lvrrkulg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rzfjppcv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3fzckiojv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3qvtffnic.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3ahkclgdy.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rfpvrlbr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3gchjnhbg.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3jlnnzwrp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ytntqnod.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3mafdglod.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mwqiopdo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3fgrufysy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3tdqmyrqg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3zunecyxs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3bqkmpbkf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3yhxrsqgx.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3iyofnvvq.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxyboqzx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3vkflrint.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ngxydiod.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3wejosgmy.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3hwdntpoo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3dnprhrdt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3unnsvnsq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3uvvqpgop.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3pdrvhqul.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3fmnbjsar.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3mkedlycw.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ajcwdeie.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3yqkioehp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3hqxdclyx.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3adzeqkbv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3hhpdpnse.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ssquvruf.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zyscmuka.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ahqkezan.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3ieqrkico.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3geishftx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ekttvwkz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3kacstxlx.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3zjcwtfqa.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3kxktkvuk.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zntqpjhc.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3keagqhep.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3zrqombpq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uvituudw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3ssscywxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jaxriaqc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3zpfpyxnm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xojlbifj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3bmlbdson.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3wncmoibv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3dekrrvop.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3keuwkqrs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vujwqmux.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3bvllkwzb.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xaraeikp.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3gnabswcl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3pkgwodvk.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3nnqxsvjq.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3audupxqs.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3egwsiakx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wuvydcwl.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3gqqmcibh.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3dtkcerco.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xfkynrxf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3sjhrehyk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wbzaostv.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3buxuxrpd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3fhzfmllo.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3ynphpxih.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3uurfkizd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3rzgybtne.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3cgwxbmzq.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3pfisuksa.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3fespyubd.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3oopehzod.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3jefhaegn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3xzqggntq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3byoaqcxl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3wxzudbky.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3uxwlccsd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3sbuykmqn.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3uumbjzkj.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jxtoerdb.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3jsfrkcfs.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3qlvsujss.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ydbcmljx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3mptuekos.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rtrnygkz.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3qnjrhiiq.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qjnbwgma.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nnuaqmxz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3txjyotos.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3opibajbk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mknjjvoh.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3toiqewpp.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3ofbquejk.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3bcumybjn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jufhdwca.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ucvjauoo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3rviitwds.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3cqojmeeh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3exgkyycv.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rvyshkko.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3evaweotm.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3vthftnoa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bfmnpcnj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3crsxxdht.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qejoosib.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zelirglq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3sdygzdic.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3vtcxzaee.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3ujmnqmgx.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3qwxvehmu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3toxarcft.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3yplzrvee.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3igfmzogq.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3gwnyqqhu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3ehiyhrci.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3ssnrjwvq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3mixuatao.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xmljsjag.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3rzldfhxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jkifjxdh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3fqczdppe.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3zggtgldc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ssunyrke.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dnjzwnpd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yetpphmf.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ivqbxepo.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3coiaxopa.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3evsozcka.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3otcdqpiu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3eoizemjh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3viikndbn.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xqnzurur.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3szaqqdat.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ffugpkip.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3sgzfvmcb.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3irjptzns.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3wcpqyssa.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3javknoop.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3evhgyzyk.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3yulimemg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3dihtdfxo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3pfpjpvot.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3dtxbzegn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3jgqxykvl.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3jddclfrh.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3pomarqcm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3fyeolinx.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3oyzrrtez.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3pgjagdcy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3aucbraru.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3xtarnbnm.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3zszvzsvp.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3xobazzke.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3mtbkurqr.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3wfhscffj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pomkgyri.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3gyhwnjff.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pzwebuuu.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3oakqckxl.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3likbtfry.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3mxsquehe.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zswlwqad.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3ivbbhzyv.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bjstjvmu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fqlwavem.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3czleuzvd.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3ggfewegx.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xbrlagsz.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vxynsayw.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fdblczix.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3yizcwcui.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3btmcgmhl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3hhhnsvpx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cnjksejy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3rwgblbcs.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3zdngeiyr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3sukjtsrd.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3oigeroym.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3wdsrwgfb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3anyvpxpa.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3nzoafekr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3kclppcym.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3rwcaojsq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vpksstwp.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3axdqrpfn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3idjbxqvv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xfvausid.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ijesnfzn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3wxfbzgto.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3agyhsfkc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3vsywiiti.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3jvsqiyyb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3eznecdox.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3uemgimxf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3jyzpojys.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3oalbjlnd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3jjgreqpr.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rradcfzl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3hpahugke.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ozqzrgzx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3mbbypvwk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3peefyqzf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3nupngmqx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3vybbygsn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3bmnmapkj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mmhmhrlc.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3mjaggszf.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3piumnzrm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3fsdnuxaj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3fbhfqudp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3ounjvmsv.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3gvzxsvhh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3ycbmrmun.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3uhaqebme.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3muxllrwh.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fphzaiho.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ijatgojo.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3uahlurvg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3elyyxcum.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3nutcrrrw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3jsdqatns.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3tbmfhpmv.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3szxdbylb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3tixlmfdj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3shzpgovk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3ujtmkrui.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3ebbhgrua.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3qnpvhkpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfjgpxkk.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3fkxbuxhn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfcikhhy.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3iaxcpuox.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3dqmxzber.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3uoocnpgq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3hrscqaaz.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3hcwpnwoc.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3omfbmeyc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3lhktxouz.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3jahwmmfw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wdifkqrn.html


<!-- 参考信息 -->