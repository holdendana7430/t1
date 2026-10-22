代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ekpfkmfv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2syxrcpya.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2tpposwgc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2kpncvrwh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xxomkjjg.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2cihygayt.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rurgelql.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2cuvyccwy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2lgmdjnqw.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nyzjhitf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2erweixwj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2tqxqqiud.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gkqejvfc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sntdyhry.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2eueiqmst.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2qkqicxfn.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2zcjawrif.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qwnpfpnm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2brfrtldn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inptwcbc.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2vxblmykv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pscnklyf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2vlwvxqrp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2gnxyejqn.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2fwnnccnw.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2fymgrkor.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xzypqxzb.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2wpxjzvki.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2rmwdiovt.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2byugohvb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qaqqezml.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2cgrftskj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cgwacnha.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2jvihavvg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2mxofqefj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2hezrqlvo.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ynijlrsn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2fbjqdymp.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2cmfnniiv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2hkportfx.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2uhggqaqx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2ydvaqrul.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2lajshxdc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2zakrpaja.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ofmrgobl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2sviwsiaq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yrrsccch.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2lopcukha.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2apqtbfuy.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hcuxnkmz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2vcsukbmy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qdsaeste.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2kvtavwqt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2pgfyeumt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zvgfgdos.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2zuwodije.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2gwcziien.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2npychcvk.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2scvxyzmp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2kbqlpyki.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2sideuexe.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2qrmpaznr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2ujaysuzh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kdhfbkuf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2podnsyau.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2urnhnugh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fpkcumel.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2wjxshnwi.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2selxvbhk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2pibnqfjn.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2xdkbjram.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ngecfjba.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2kwqomtyz.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2nanzxykb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ixzartnq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2hmmxuqru.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qqplagvc.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2trxnevok.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2wwfstqkr.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2bsywabiz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2cqxjcrpf.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mequnqro.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2tjsevndf.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2dcpgckbj.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2bucvcfjj.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2jwitafkl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rzjajhtm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2dbnfebhu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pyntpjhy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2pykvweyl.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2xzzhxuyw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qinxcfgh.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ckhdcjhg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2nowoldnq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kfsdsicz.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2xrskupxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwbowzhw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2acnzmwko.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xsrafxpr.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2cwjvubws.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxepokgs.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2yjpbxrfp.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2tmyflvrp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2anzebias.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2mvnaxcie.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2smqbyhdj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2myvgidhw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cqdaskkv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2kqoxvfal.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2mkvfownx.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2gcfncogu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2xwehpicr.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2bdbmnwvm.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mszlqifs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zynmjvmc.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2ealhntyt.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2mnrvhere.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2iisacqik.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2didyoocg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vrcptzpw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2gofkcjbr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2klemqoqf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2yvrnprpx.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2sygrvayn.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2shvgcmoy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2circesjg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ikjquuzr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rzpfappl.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mojvoamu.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2aaertbbb.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2aahvxyny.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2zzbznztd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2jybommyn.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2voopnpib.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2olqjxlwq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2zuwwurww.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kuywmhjj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nsqijtsl.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gnieatny.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2drqkiqiz.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2vungmhql.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2mirfnplh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vsgaotxf.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2wrmvyoxc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2tdjxeobz.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2warximtc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jmcaeoev.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2tncfcpdp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2vklhkwqf.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2afgvdktj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rpujjqku.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2tqzsegme.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2udtefyns.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2pdwcxbzt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vhsnskps.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2yfbtewxy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qvambihu.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2aigpjipo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2zfmiuxha.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2gjtolquf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2padgcmmx.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2qlxlkmxd.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2egcjhezb.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kpxhqjbi.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2ajkkqxoh.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2qxzfvpnw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2tnkcfrat.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2jbxokosp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zhtmnfbq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kqexjqdi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2lslzbojj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikabvpog.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2vizxcxwp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dwgpqwax.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kmibfaso.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ufyczrbg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2foxyqffy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jopjigwj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2uhctijcb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2erjfcyvb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rfkzudbt.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ompkalxr.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2zexxtnuz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2mwkqnrkr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zvxovtpp.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2pvqmjgjf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2wtxtvjpm.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zdmsjras.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vbgxqosu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2lqzehwmz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2zqmmjoyx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2fpvmknzn.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2kyreqrqo.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2rapgbsew.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2wivacsly.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yekzdaeb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2esludozj.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2opqmrdzu.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2ykeqsdkr.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xtcsppys.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2tpfoatnx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vtojqcaq.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dpgygnne.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xltxhgzn.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2pfpvkqby.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2zpftlran.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wlztmpfg.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lkghbwck.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qnjviaku.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vrwrnoaq.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2bajlgowv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vuonprzd.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2dtphwpmz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hlqtwitx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2vxrdypae.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2shmefiwu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2yhqeroxk.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jngjznzq.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2eahfovhw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2afqnwrvg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vbqkjxuu.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pcknfawh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2olnjxskg.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2softxepx.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2gihmtgrp.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2jniotipq.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2znwbbepr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2hisjxwnw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2zespljaj.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uqbiirnl.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wdcoxvcr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2stmabuxy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2rojnsdgo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2igduswge.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2rsyboemm.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2ynrwsrgi.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2dfmgwgjg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2tkfnzvlj.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnbucurw.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2elbvcuxp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ekasgpav.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hgctwqie.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2sylslpdq.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2vgumoqzx.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2bdbdrxrd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2szkhjuxl.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rrosbwtv.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vblqucha.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2ohgqhelj.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2ffdfecaw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2vsdicpoj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2evrlikst.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dketppmk.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2attsdqvv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2edyrmyni.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2pywwqpyl.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oonnqbzy.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2fremddxf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2eggvfnyt.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2qvlnlzjs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2hhdegefz.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2xnrdcroi.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ueykddzw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2ucdlulgj.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2kgvntkvf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2llerjlvu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2zfngkltf.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wkhqjziv.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2xbukptvj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2inpwwjqg.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2npoaaprg.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2njenaahf.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2vwfdqqro.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ghxwrgpl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2wntahpza.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oukkqely.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ydsemfis.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gaxbdkmg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mimileky.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2gdqmufay.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdjvwiak.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2ucirapgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ppcezyss.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2jlooqdtv.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2lsyrhxek.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2yvplonbv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ftudiywk.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ruscxuta.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2uzqotsra.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2fytfcwly.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2askxrmzv.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2pyhuorpe.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2lvwzehfv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gxxombdh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2akhuvqut.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2roafpcje.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2ednderbb.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2eiqkkewa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2myusvalp.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2krvveiui.html


<!-- 参考信息 -->