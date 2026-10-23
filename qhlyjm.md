代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3yyxqgzoj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3qtgbsbwm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dkdhutsw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lwdpuqus.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3cokhxjjy.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3mwbuelyw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xyjxruvx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3amstlrgk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3fcdipmgm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3adzjeagm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3jkmistkv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cgwrglss.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fcdqbrhi.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3egjtesaq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3mipkprky.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3bkpegcuy.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3wqcezmsm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3bmxxihjv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yprjbtum.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xhdluuxk.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3wjlmeszq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dpgfacnc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3fivevcid.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3drdczepq.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3nhnzuofj.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3wirwgdwf.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kucbkxwg.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3hkpwgomh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3yfrkjuco.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3tbkfrvew.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3vpmdfbzo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3oqycuwnr.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xhpnxuhi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3ytnsayan.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3epoxdetp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3hnvvcpyk.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ofowwqrs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3jyurdyzs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3pukdrewm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3hmmqdysg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3vlxzswoi.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3dxpokovt.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3rmgdqpwj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jdrfnmqb.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3oqdszdnr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3vduywrgp.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qqtydqoz.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3ovqyfpww.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fjmzdkly.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3bknhtoqh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3wifsxpyy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3turbytki.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3uexmkkik.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ypqtdfqi.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3jteqtrqo.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3mmzgjatu.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3tnfuwest.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3vaalgixf.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3msqiuuca.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3cucngsvh.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jbqjfxer.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3ayzzlorp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3dnuizhup.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3xjohwmow.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3dkssluph.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3hzmnwhap.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3coeyogsy.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3oryevfwn.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3xqmpzxde.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3hvogsnvr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rruswgfs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3iulppyeh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3fupnvmti.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3gqngwsvy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3roszcaew.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dsryokan.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cdekjzoa.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3dsndevxz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3swafclmi.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3qdfodeui.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3aetqjmkc.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3wenzkhau.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3ehmeqqjj.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jqzcgwyc.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3hwgowunf.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3crvtxlkv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3bnwiqfgq.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3oyrgplho.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3poefqtei.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3lyhrbawm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ypgdpsky.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3frzbqfjq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3vrovfnzo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3suvpwqvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihtyowap.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3txbyzrwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlaqezkm.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3pytvmjnj.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3flumtdjz.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uyyuideg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3bvbuppbx.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3isvrgjhz.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3oecvpyqm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3jmbrjswt.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3lfkrfwjq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3ljqhogvd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3crsmbtnd.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt3ewpgrhda.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3pajfawox.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3qsewzljb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3plonsomf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3umsfwjhg.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3onobidxz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3lywrazhw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qkgpefbx.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3onmastir.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3emqbqpyb.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3vykkoygw.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3eqalsqmz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lxaubcmz.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3wgevngum.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3nbmvscuh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vikmhtpn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3noehojbb.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3niicoazu.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3pzmptneb.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3hyfdkrfo.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3jdkauybw.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yzuluhyb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3jpcvampm.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3dypukibv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3ddojtiar.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3urkhwwju.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3aprobqwf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbehxsoo.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3gfbxewwo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3gwaiasgc.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kilvloed.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cwrbwdzs.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rofdyloh.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3jdogeati.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3bsqznvqc.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jqxrlksd.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3rkwsqknb.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gqfiyvtj.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3rlkhfnzg.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bnrronzz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3cnezpaza.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zzsmvptj.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3galzjxly.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cflomkua.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3twvzexlr.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3yywnclcc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3xudpsrql.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vbsgaarx.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3dicqzgvf.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3zhzktgmw.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3rsprasrf.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3pkicbgnp.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3lrhfxnqh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3jodzgedm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3enubvrmr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3pdmshjaa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ehjxmjlv.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3iggnowja.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3ycfgioad.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3zuybtraa.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3qomdonoo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3ecqclria.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jbgnrzzd.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3fycdmoqd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ulqupbpa.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3onijgmeu.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eiehlznw.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mnuzseob.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3jjnufqkp.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3fdelzyzr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3pbroeclv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3hbdwiklm.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3olospmfy.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mbmvjyyh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3hbjmmwsp.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3izjpbvun.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3anifeekc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ofzewgua.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3lfrhvyiy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3cwawswdj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3bcqgtqyo.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3byrktkef.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rdekzyez.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3merijzpp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3fmqglaqb.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3regqkieh.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3fakdqtng.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wlsgdayy.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3fyesujvw.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3giqfutlt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3ymjcjzjd.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3axudwqql.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3dvqigfyb.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ghuxcmib.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyxpjkiv.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3eekffdmy.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3alcixpiy.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3rbrvmmcy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3fmlvrzth.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bejeaywz.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ahvacugc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3iyxeclzp.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3xudqktes.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3cyndsyzb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3ibbjnbgz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vozunihr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3mkxqnmqb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3jueeuenm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3sfkmdrbl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3ljacxrij.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3sejtwkiq.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3solklzyu.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mumlvrti.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3yfacoznq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3nprhfsfl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3skcctaik.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3jbclwbfl.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3avsqmnyv.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3ojacziqj.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3kmsqkjdt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3cgahzjtl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3yykzedvh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3yuyjjchw.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xmkjhqvk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3exvefhga.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3djxujrzi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3uxvbuovv.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3aeqyrsks.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3jydhhpjd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fthhxudn.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3rrbpiyoi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3zibyhswb.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3hnhykcxz.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xqxtfsbo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lrerijgb.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3wonhiavw.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3glxotakj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3vdlivtet.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3lfaguswf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3mpiuwgyp.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wtjrblti.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3omvmmquw.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rrzrqggl.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uquttkok.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3zcxcffdg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3mjcyenzn.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3fmvatztn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ryltkrvc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3psnomigw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3cgmvwjvh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3mzcfdwwk.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3ddygdunh.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3xeofizgq.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3xkcusxwj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3lowrdigb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3tbhtdrcx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3xbnoscfr.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ancvcduq.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3iztxairp.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3tajijalc.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3qchosynq.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3xbsigidl.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3fsubseot.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3znkmbczr.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3zifjgbaa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3unczthcd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3xyuudytu.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3agnqfleo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3agjxbvjw.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yqthpiwp.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3manktmbm.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3uvbuctih.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3kgbnbrkx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3prdiarkw.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3nenfstag.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cjtxowpv.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3bypkvcuy.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3wukqieks.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3pplczxfs.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3bjlnuaag.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kycazhue.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3mngvubjk.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3vntbomdf.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3qwzcwmqt.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3acexslww.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3mgqqcvqi.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3iautmbeb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3hrtfhqhx.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3vvbxjjpz.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3kncnvrty.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3rtmiplnl.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3obpdtziu.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3rzrsxjfw.html


<!-- 参考信息 -->