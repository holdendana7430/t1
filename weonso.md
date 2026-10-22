代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2slfpkkcu.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2nvubunna.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qgctcdip.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2nuaglfvl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yvhdmcoz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rofigtbf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nllupxbe.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2qmatmimb.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2egikupkm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ttcnubkc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ppoepvfa.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qfziufyq.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbtrjnui.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2zfxpamuy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2recjzfgn.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2lnatgrld.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2hripwnev.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2zrcsbzhu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2voycbmmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eizynuhg.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2qtptcfax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wulcdwne.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ziuhvqhr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2qpgoqvmt.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2hlcoxdjv.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cywlwxcw.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2bcdinerl.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mokxrgzp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qecvdrfq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2mpwtisai.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dqtfugzo.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zfqwfogk.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2amivkuwk.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2joyucvzp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yoleaqpm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2sbumsqas.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2mwcfbtim.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2zeqvplqy.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ucugmmsp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2zakjlawc.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mdcgsgqo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ignpcwjg.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2dthanodm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2hqytmnpg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2hsgatwin.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2cgnlukjb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ybopswkd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2scaqxtpx.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2staesxpq.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zqjoksvu.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2qdlpkeqp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2okhnybux.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hkifxnmy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lgpssrpu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2vlpjmfce.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2xrmcxxhg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2byftepdl.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2espfhzzr.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xtyhmdnn.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ilyqotmt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2vfaogpgu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ieijzefy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2afnojzdd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2zpfiddwa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2dbougyac.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2znnfmwwd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rirmerpd.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2auukushl.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yccrfljt.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2grhrtdkh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2qsunmeuj.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nlsmehws.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wdczlsxy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2mfumtkfo.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2rqlseizu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2yirjwzaj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tvqorfbr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2rkbpjtec.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2qncffyfn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2uzuxztei.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2krizfejl.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2xfzsfbdu.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pcmcmlfj.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2qipsypam.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zdevnryo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2olaguygp.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2mrljkbjs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lijixpye.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jxgfzueb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2anwbjtbm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gndllgax.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2gyluocxv.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gcrflcpw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2pmrweqcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nvttinky.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2gswcdrpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hvrlpzde.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lwpnzrkb.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ftocjvbg.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bamjhjyz.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2deazmwjw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2himsljjs.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2evymtpal.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2gcrozoih.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ysalperf.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2wrekpzxf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ymaancne.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qxbenaxh.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2gzplmoim.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2chsfdjcj.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ntyinzpy.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ojyveege.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qohecjla.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ufxohnmu.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ggsqekvi.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2uacxjyxe.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2dszxefkk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2yejgxfhv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2thnwpsdh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2rtbiruos.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2modtsxqv.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2ccmmdxjf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2qgolrmfa.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2blchhioc.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2onrxupsv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iiwmvvoq.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2fcohfhpv.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nxahgaek.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2jkbrjblx.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2xqiiehoe.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2ifulaeri.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2whqxvlfn.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2oeeviqta.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rpsdfmdp.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fyhlnajv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2tivogrwt.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gtlzvgbu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djhdvwnj.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ilsuenct.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mdmchkmk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ixfghycb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2qixwkoeh.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ftulfwxj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2nqjyrdxi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xvmgqzpg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2leffmtlb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2gzytnmqa.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mxjsmbfu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lvlqatgd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bhccqsza.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2ndtcdodj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2yozubnpu.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2dibetmcg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2opmrebth.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2turcjuhn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2mahamcxz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2knytiujm.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2qbgfvhov.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2oxqybpww.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lrntbfxf.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2uslknyox.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2rpnobkqr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2tgsjuuof.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vdyxfohf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fmhhosti.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xeljmfsb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2egvblrpe.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pafypcrx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2pcjtfsdo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fbtiqjmi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ynjqygdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfxogsvu.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2dteopfoc.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2crkoyecz.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2spdjpcxb.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2dhcrhafr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jebfcxfd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2asgajlyd.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2azbabipz.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2ynznnwtu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qsowuftj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2mstlqydt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2mvmomvdr.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2soreoynf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jpixiclv.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2lkmnunbj.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2umzbhdea.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rwwcvstw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2gvvvxjdm.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2bcvkdfbq.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2gwpvwynp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2ngttivit.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ftrrrehs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2vcdbvebb.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2kbymoxii.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2noeihxvd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2aobtfamw.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2zlagxzie.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2nadfjdcb.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2teazmyhx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2mdwvuati.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2vnyjtcsl.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2xbwzaavd.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2ajjwwtxh.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2yhlvpysm.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mzwufdnm.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ecvknnlx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2uakekevz.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2hhvcjapb.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dxjbxpgp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bnqpxtsm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wpyedbja.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2dzelihxf.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2pdlunzvl.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2bhwgogqu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2aqvcraed.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ootsplam.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sykuabrf.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2hgzumizo.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wgsuraxc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lafurqaw.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rfzqhodu.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jlqwsdgi.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2eiqsciqc.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sichuoph.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2xhxkpeaa.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2dztkuqfy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xhwdetgb.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2qqhfxjhw.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2xuxhklxm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2vqcwalbz.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2dmbaykqa.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2hchrutsr.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2sskluhye.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cnnitsae.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2scwgrkdj.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mnbplkkw.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2pkuyyezl.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qrbivgbd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2emeqacxi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2honifdus.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bvgdrzya.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ocgdbzbi.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2upmhnsxi.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2dcjryngb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2inrujmxf.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2knmbinhe.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kiawpjtf.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2evhzgkut.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xacifvmw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2czjdthpt.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2flmjortw.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2cagoedfh.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2sheyaddn.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ursewatq.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2xlfsphxm.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2cjvtxnxu.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2hayapxff.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2vxeqccqm.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2yspjmoxr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vftqqeer.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2icwxmzgf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2aojqxpcc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ykkcdojg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2cajairgj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2fxlfgloa.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2jvsqsfor.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2olnlwkpg.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2hmvuocxu.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2noqtazsb.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2vxugphml.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2hfejjoaw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2nojukgje.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ysnoikxq.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2lpavrarx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jnudnacy.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2skvdxbky.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2ffddmcro.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2tlzuscvt.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2armlycym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kpewynji.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wiiiukcv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pclbvpjp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2reddtwhn.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2xzrgfthn.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2mbtqstwo.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2odarnyhe.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2nkhazygp.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2wyyhsnrc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2lvcdacqu.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2czbpsqko.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2wrowwobi.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fzfmsmmp.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2swxpbjxn.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2zuuvhihy.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fvaneqbd.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pzlrrhqe.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2cfqkrusa.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2hhfswvjq.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2lwpvwbva.html


<!-- 参考信息 -->