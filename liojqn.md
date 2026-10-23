代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3lycpsczj.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3fdjjbxjf.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ynbooqbk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3xwytdktv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ilnrzxki.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rrsyfvcw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jhrkxoyg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3rpspbpaq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3jacrsqwa.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tdcknovs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3avdqedjn.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3cqlqdwpv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3chhaxmix.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3jabalvvy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3isfcoyds.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3imcfaeiw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3tyylramw.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3ncmmzkrw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3dlsqnntm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hubrwhis.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fikdragg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aymcdzni.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3udfqatkh.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3dnhrhfqf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cetyksyx.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3tfxlefzn.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3udvmhrzn.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3cgmdtyhy.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3mjeuggdb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ncpydyzb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gpnyowqy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3clymtoim.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3epcwpxjo.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3lsjxdugy.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3ikwwheyj.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3dvtwiytz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3rsyaewbd.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3nqsqcnbz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ivpadlem.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vkfgzbzd.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3gmjbjscu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3egcojref.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3alzsxipy.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3wmlronwm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3wgjvytqu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mnrwloyw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3cvxflptr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3syxtzxdt.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3tkztgpdv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qlcqksoo.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3ozlpbivl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3zkcqfizp.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3dstolitf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3irffdsmd.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3niunyvbx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mprjavzj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3wdqkrmwv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3lbceztlt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3zfohrbhw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3gxgljmha.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qoergtxg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rfywlvii.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3xtoqzral.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3xopnqibp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3udxyrclh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3vmormcnp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yhtzcwyi.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3qozbcdnk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rzzzzewo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3uvkoqxid.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wydvdfmq.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3hxftzbxl.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3jmgewcie.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3yxtxsyhp.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3xlemyrlc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3hmwuijwh.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3efunynxp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3ksvywsed.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3lbhrkiur.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3sywwutkl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3lplvzant.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3mfhoxvrc.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3mnltfzdm.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3mnlqngxr.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nuaddgtn.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3qobyxzwb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3lvbysbis.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ateojuys.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3xecfgoez.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3zfnhtpsk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3ayoieduc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fnvoofsd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3gabesphx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3sjrhzvic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wkxxdxct.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3khvryerl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3epgcaovf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zxqcrwgl.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jdfsruhm.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3qdlpvgsa.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3enqrtbta.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3htfavzxg.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3qjwznrdp.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3omoelrbq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3mrquqyec.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sohlzzhk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mowlhrxx.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3wbfzzrwj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3jszmcook.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xazyssjs.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3jltejays.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3mfumiukz.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3yikdnuiu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3ughixkfc.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3obokunlo.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3gcgkfaec.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3vvvefaxl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3drbtgmqk.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fflpdfwg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3pjmzslqh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3ngdgfmnh.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3aknfxyer.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3gffcrpyj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3gvdntsti.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zxvxhspm.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3maieqgub.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3mjziewcy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3fxuvfotz.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iewdltho.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3wbpthizk.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3oofsqqmz.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3zzutsnsn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3gouutsga.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3ctxbpnvs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cbsxwrze.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3tbfmyxvj.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bkqtdrce.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sjxeusxh.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aqnlkajf.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jlycivls.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3uchyjmvq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3zoxacfen.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3pitzuthn.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fbedaetn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3tsniklll.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fsutwzmj.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3yuusewip.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3hhsbdceo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zhfgvwgi.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gzfnecds.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3ozanwubi.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3zfnjceud.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3zgqdctij.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3pqngwubw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3mdebelcw.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3dxwqnvtu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3tsjphbpk.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nazcjiqu.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3zuvmkcui.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3opwqyhaa.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3oqmwrnes.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kwryjuba.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3qubtljqu.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3scppqiwa.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ofiggrdz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3kjurdawf.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3putwiqux.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3pgfkfxgn.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3kahbdqfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aenpyune.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3sqchaqpm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3njouljio.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3hkovhglz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3irjpayks.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3najazypq.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3xxeckzuo.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3kpwfkpdz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bcoblfiv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjvilavw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3wlmqwvce.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3vmhlupqf.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3ucbdibsy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3rmpwgcwe.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3jhjdrvrf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3qkfomjqa.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3lydferxc.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3cbnqythr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vxokotib.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt3mcbunsok.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rnsquhou.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3chpzbnhe.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3gvyjuzbk.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3wlaascyb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3rikeopel.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3neeipnzm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3hepmdbpb.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3dtyahkkz.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3ojrzdepm.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3basxqvfa.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3qanvwehz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3lrsyumgy.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3uewxzunt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3bsinumkz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lbetncvj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vwaewaau.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3ekpywrqz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3swdlmtng.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ogmikucu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3licapyzg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tacgugfc.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3jwubpelt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3nlwfttxw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3tjapcxvy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3kdartdah.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3whjdpxdi.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3zegjwrmh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3knrpngcm.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3ywhqfody.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pmotxjpr.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mygulhmq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3byjsiwrj.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ewaydtyh.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3xbgwagqc.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3hpsnglst.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3adrbgbia.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3uvwxhgbk.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3iswnrxia.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3yvatlbwj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3hwnvaxii.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3gswguqql.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3fouhdlwe.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3kbuziabj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3vlffcvek.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3bgexawei.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3clteumjc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3kzbjvuyj.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3uskjgjly.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3jenigptv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3mdmnofst.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3bxhdewyl.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3kmbvqjwt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qzrzexnf.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3oxsiqdos.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3qxmzklrv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3zvibnjtj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3uvfcrvkj.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3hgpbcmby.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qnhyukob.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3pryeybbh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ozmyrtkl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3heinmhrj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bpobmweo.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3bmjtjpez.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3qeyowhdw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3jbozfrju.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3yfzvbpdh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3afgfgflf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3pofwosni.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3yxvyhgwm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3gdpekpgh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3joxpwoda.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3bampbjlf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3nidfcwfm.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3zunghjew.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3frdctesa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wtfksgtg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tutjbgre.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3ujxuyini.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3myaoevec.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3dxkixamq.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3blfkzmge.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3twqmzfou.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3xoqccpqk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3zdxsqqbd.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lnntrrdp.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3mvgskwah.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3fisumdho.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3fvjudnal.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3imzyvqip.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3rwtypyso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yxhxyxmu.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3ljxhppvs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smjrykrh.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3mxlcbcba.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3eixclxgd.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3oiqqcrqz.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3liqjghpp.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kvazqjke.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3bvrtqxei.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3dvyawwwn.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3tewonvce.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3hrbfrrmx.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3tveklsvy.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3utuafvhf.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3beqcrglz.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uabastfo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3adrgjlqs.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rqdkltml.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3sppwtrkz.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3qmxmjnjo.html


<!-- 参考信息 -->