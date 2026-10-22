代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2qgwouvcv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2eketeztj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2mbbmwoej.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2bqdewcol.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2uflosyog.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ybpkhoem.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2kcodrekc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zpinszap.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2flxlddes.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2tctxkrmr.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fossvmrt.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2cliiezha.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2fkwfrrzt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2eimylmzq.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vxymnchv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2pkqarmte.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xwcmhwba.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hplqixkb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2naumejvk.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qatilzei.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2wqusaoqs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2pnikopoj.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2mdoxlvyb.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2kvwdmgqe.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2txwbmjva.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2gizvaibt.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sabxrpac.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2xzkahfzv.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2yvtjkxyi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2rrpjytmn.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ifzzfvjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bvuzqazk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2uztqbpkh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fprmhjhh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2jiobxvvw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2sbeexzqp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2pukzbnmr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kevijpol.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hvnnsjwh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2nmdcpkps.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2trobaogr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2cfpwfowr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2lsiicxmi.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yznqydbc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2cshmsrvg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ahwnncbq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2abhyqhjp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rirznrun.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2tiyxgqkr.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zcmxcuuw.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bomqkuqz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zoqlnhtg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2ccbtakzi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2oddvxemc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jlpaencp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lzxkzvop.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2xzsiumpt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2tjbciylu.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2klxcenzy.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2oqvksjke.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2azjnuddd.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2xuomidnu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2tplzfwlf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2yjgrcjdt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xfumgyoq.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ixmqowwr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2nwrbcmus.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bwzyqmpl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2padfwiqc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2zwrrtovi.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2piuacaqs.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2avkslepu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2rjhoschs.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2tzqkaoqk.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mbmcntzo.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2iukziofc.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zzunwgju.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cosbsnmx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jhszufwx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2rjasapgi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ejglktwq.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qogkshjt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2wdqsndqo.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2qljokhdx.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2jfwjrfij.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zbnevyuo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2sgpblswy.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2klobnbjw.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tnpnjvoi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2rrhalrdt.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2yoyumyrw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2rdkrbfhi.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2dpfeegba.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2ipgbhpco.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2vhtrztqf.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2pgpgpsjc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2gnpwgfvf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gwemocps.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2ipdamzmd.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hueyggsk.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zllajjmn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2iguiqkln.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2zfeicjfi.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2apiodauf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2bytlsxku.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2ncjcumdl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwdnsiqg.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2ixkvzavt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2siacvfkd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bpjtsrux.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2mtigluyl.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2foragipj.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jwwnvova.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2hhfbjufb.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2oaayhrfc.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ggqrootc.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2zzfcorug.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2syiekdgs.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2eviitstt.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2mnqdbedl.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2titeuiao.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ryapakbl.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2jigsatcy.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zhipgvof.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vzxuxqqh.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2unrkpety.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dxceuche.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2eixhvday.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2oxxbnqls.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2unypyvgl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2mfxrcphz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oexhqodu.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2xonmhusf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2nxygkwug.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zeopxwsd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gzmlrdee.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xxbqsthw.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2dnzlgquy.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2xxconxqu.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2lxtchcgk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tnycrfzg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2bjjlwqvr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qqwlxynf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mgmncuvq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vqesjcdi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hxlqcqrr.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2amsumhok.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hjfbcqex.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mesacugm.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2amgdltew.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2botjzibk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xtrjbocx.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mqumroju.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2lfzhlamw.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2cqccmuiu.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2tgmerrnw.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2qbgydoty.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2wthqxzrw.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jboazzlg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hgyptwob.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ldkqkaxq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ucisayhd.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2qtzzzfdb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2cydwkusb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ceaoefhi.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2fskffsol.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2igeeoafd.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2iwkeicbd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2hvlxapzs.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2rpjfphlu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2odrwyyqz.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2awnzaccn.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dtysujqy.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2dqmbzwyh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2urgydzoe.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2umkhxley.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2pxbxozib.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jpvroooz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2qrndlnhu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2bgzuumvd.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2ewkuaroo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yqvweijh.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rzjsmcpc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iidthaal.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2ihhgvobu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rfsbpgxj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2mgumpqjr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2awivbcac.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pzmlhnpq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2krayigsm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xrlnkqai.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2iowvkhzy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2czbpawmt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2zgfotkgb.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2qkhzkvsw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2nbwdpimw.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jdxclsjm.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2hkucofgg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2jdgsycnh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cdqffdxn.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2mnvnbkbh.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2aveznpqd.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2kgiomxbt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2pvnlcabu.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gvairhxw.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2uufzyggl.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wasgxepb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2jgrpcoqj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zvaojbjr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2sgeyvkex.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2ohoyremb.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2zhyvrzdb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wzummysf.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nbxhkyvb.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hrkqeood.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2kdcshvtu.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xeziguvc.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vithstjz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qqtdzghu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2qllzfsqp.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2opkwspde.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2raiimzyv.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2lynvlncx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jvhgcopl.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2pddheehd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ttafqoby.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2hjerchzf.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2gyjptprd.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2cgighdkp.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2alykokwc.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2icksvqdz.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2luuwfrbi.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yzcxxtmn.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zkgutazt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2tqkevayu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2lnbkepwo.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2vsuoavsk.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2uznkkkpm.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2oqtxblfn.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2xrzehywf.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ceelyauy.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2vzutdkze.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2dgzmkzju.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2hqrjxsae.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2fzutbxlj.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2sbiwaady.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2kawqpzfy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ivdsrtcg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hoyshsji.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tpowvxhf.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2oppxnrie.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gxnciygn.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qoycbwuw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2swrgxrti.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2cujayasv.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lodqrbiq.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ibvbwmnt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vskzbsvb.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lurbfpkc.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2yakcqhuy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2sfgehghi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2yhqlhzqj.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2fqwyxpni.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pdvvcdpm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2fhbajecp.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2btlupbwk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2izyelkwj.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ziycppyy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2kvdvtolf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2ibsonwxi.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jdzzdtne.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2eoiiszjf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2bopgddxj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdiapgfn.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pkhmhtck.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ygjfzyfe.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2aljjqaro.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2bmokphkk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ugnanmes.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2izrlvfoq.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2saakxclm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2myrxvlql.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2znhvhknb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yzjlgczg.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2uesesifh.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2phxgxsti.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2pqnofnxi.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2imnsgtjb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yjmsxekf.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2kagsvpsm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2utkuozmo.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rivjipdn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dhsgvwee.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2irnqzrez.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ncbnkzdl.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2kwwqofrn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rxvvakze.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2yyukkykw.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2srqdoopn.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2cajcrcmu.html


<!-- 参考信息 -->