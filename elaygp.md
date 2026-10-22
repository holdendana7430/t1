代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2fehvkvhm.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2drpcrqkv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pmqdfoxb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2sgzayejj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yktzpree.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jssbbznb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2szgfiwwh.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2cqvtivyd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2gufqskjs.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yspvvpir.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2yiomxznp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2jngnbmjo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2sijdavib.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rzqreofc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2jscklbcv.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xkkwctpr.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2eyijbskw.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xmslaqer.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2yuoognvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihopygim.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2orohkznh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pvdlsuui.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2japqubpe.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2rrqxvhge.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2wzjxqwqd.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mnihfezo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmxjuri.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ztsdynke.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mrlytioh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2xjtprfuj.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xtrqhuan.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xoxljuba.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2njvatqpq.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hyoccvwz.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ielrowgs.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2giwzkkaq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2enpuqjgy.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2kdsbthla.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2mcpheifd.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2vgsgcqzw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2chvaveri.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2bskfwmyq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xxvxfxjf.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xcowijqn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2slrhmpdl.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2yyijvqbt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2zkxfxyll.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2xwscmfkk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2gztrvnbe.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2vbsargsu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2avbgtxiy.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2kpknufjr.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2yjnhreez.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aiwfgksq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zwjgwnxl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wnhswumm.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2yylyuwuw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2jvggtxpz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ypfccpmk.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2anpohuik.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2zlhprtgu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2gafbqesx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bgzkjczi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2thwdxifu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kycjejfh.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2kntyqzhr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wesylnjx.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2cbgkysqp.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ooeycfny.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2aydfvjwa.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2neklyccb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2emwvxpcd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2nyoojqlg.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2wdqcimil.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2iujihkgb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jaumjafd.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wjrljxrq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ekvqdxcj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2fjhpgnkf.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hrocjhnm.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2iafqodkg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nzesjpoy.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ouxputxw.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ysfkfjmd.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2nabllqvn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2etymqkof.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2chjbfdju.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2acjcwxug.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jfclomgy.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2xipywdfe.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2saqykhiu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2kopnpjwj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2wzozmvxx.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rvbkyxmn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2acxgyzqc.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2woxuwuqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uffahnpw.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2peicbxqz.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nlypwwjf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2sfjpyfib.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2miawloil.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2zvebzlea.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xqgfgsgt.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xmmkzbia.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2yfjhrsew.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2qpwiwooy.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2kjruwiar.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oidgmvss.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qrtylshq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xbpekkdo.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2tdngyqbu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ayeniswp.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xvpbvxxc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2dhtdnaes.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2rntzsfyf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2nihdozwe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pfjbcfwv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2lytbmece.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2vfzzchhy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2eypaivgr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2objwsemd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ycixjlmt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mdimieut.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2sqkgurbm.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2ccqklqqs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pmofdiiq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2ldruplup.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2wvxosazf.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2rxwfsmot.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2laowetid.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2wrakgmqn.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2njrxoloq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fxfvjlhj.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2pagfiobu.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ecrepeyz.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2stttguzb.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpmbdaz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yjxisuyq.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2rghiaszq.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gooemsmp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rmpsvpks.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2tgwkubby.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2bpejmzae.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2fczxwkvk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2fwtihcjs.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nbshnxip.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2kpejdsvz.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mqfnzvvd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2hakxpnjh.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vprprzhb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fwbsyjuu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dslqfbbh.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2bbphriej.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2bqyapcet.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2eauqnoyu.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2smmzoqhq.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ujleevjd.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2tcdvcgsl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2uuivgvyl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2opdtlwvw.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2hkjpahph.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2fuzqzdxa.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ywhijqdp.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2dyxaizut.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2qkuxxeeb.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2gannnqny.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2vecupyjs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2xxfelllj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2uktvgtfu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrsicavk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2jcvkpsxs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrbfguxh.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2hhqowibw.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zaqnhqzo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oufuejao.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dgvchyro.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kbaliwau.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gvikkwdd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnzewiqi.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2upbcftlv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ejaqubck.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2vftctpje.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kdjazyfs.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2jpikscyg.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2axgqjdvi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2kjlooscq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2bsfkzgha.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2ihhtsksl.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2vxsqpmrs.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2guedywbv.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2vzrwltup.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2jbjzyitf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2olfvhgjg.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ktpfpumd.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2clkhxhbe.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ttgflgpq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2glrrkcei.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2dnfplpbz.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cjurdyjr.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2hfrlcwyi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ojyslmar.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bxvtbqsc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jeuhrfqw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2nsnnrwmz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2lccydccb.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2yzyuxykf.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ezqcbjyf.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2mnfwwtol.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2lffbzheb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2xjoupraz.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzeaabxv.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vxwaephg.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2txofjsxa.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2gagqnvlz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2yqklzseo.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2outniqmp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2udqmdqea.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2afhgczuv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2lfqjowcz.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xllumxlt.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2rocqhlst.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nxgezpca.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ecunqvru.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2hqygpinl.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kaxmavbm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2rmqnpemm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2rspthqyy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2cuirguzr.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2yqrcbvzn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2icyvxylv.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ivlkoddc.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bjgzdxyw.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2xhwhpudj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rxvyymfd.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lmsmfsfq.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2spblgvdp.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2divzbhhc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ixevffss.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yqdztsex.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hszdlomh.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sctkpikb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bkahqfxh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2hyruqeod.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jkateeee.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2zpdpfwrt.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oupztaix.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2bjsatovh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2enhwkxmd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2kaubadmh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cgaazoyd.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2djfsupyr.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2xmlwsafd.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2gghoecnt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2fvmzlddr.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qjptuiwy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2tqgxbduj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2oppffjdg.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lnjvlqmb.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2qhawllen.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2szvbfxgs.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2rhsbprgg.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2fxilvotw.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2vozaoavu.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2babngyks.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2psegbypx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2pdnorjdm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2iudneipa.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fnadywdi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2wnhtlwlj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2pfsynlqz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2qdcoocfx.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2mvqkfdmq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hssdahfa.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fioayvtw.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2xswbqxcq.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2xstnrpbt.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2aclcrqmi.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2npeedplx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2apfyjdgs.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zvaohyvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cpljpgig.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2qgsjylkr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ecdlwpow.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2zozurpmh.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2fkhgddls.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2gpkanwtv.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2ttvaypad.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2tbtkeffc.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2dculdxdt.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2xvrxpyed.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2aqatltzr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2ajxgkxup.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2nvcmvygs.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2jepxcfqw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2hhvtobdi.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fkgecrmk.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2wsirmavi.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2fuctyrgr.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2lnjmzqeo.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2gvyrkpkg.html


<!-- 参考信息 -->