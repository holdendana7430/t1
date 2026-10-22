代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2lqqayroc.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2baoksjpl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xdigfnwn.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2hptppqri.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2lxqxaxkz.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nvuwsvng.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jlfswlae.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2mhptqvxh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2wwsotoxl.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ntzdgfft.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ffjxbmif.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ocmojdmc.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2fgmuwmmr.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2keenaskq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2xksfvqvp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2lahqdtpk.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2yknhmdjj.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2yoowfldl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2tfpjkuwg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zdygxqfs.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2xoeuigur.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fsgzfzaw.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mvbcurzq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2nxjzeyqo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2upphesdp.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2cqiruyca.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2khnypdqh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2idyicdaj.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qnokgnxk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nwkjzght.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2zuazasnu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2swsgjxdt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yojbdpeb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2vqjkylzh.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2grmesriz.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2rulbcajh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2gcjyjnvv.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2cmdsudpr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2yqkaanlm.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2nyxsvlgh.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2zwhxscsw.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2anbhvubz.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2lnvzkqxe.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2sxcujzmh.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ctvzdjvm.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ttfwpebv.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xosfjezq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2phgcxnxb.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2djmxekzj.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2hhhhynwb.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2cjzhferh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2qfyrjgwa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2fmgmqibt.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2ypilgzpa.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2aolebaeu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ikipvvlo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2xnhvilpg.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2pniprrwb.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2ybbofipd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2icymyjjt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2uozegyyk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2blzyhicf.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bgnblycm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2jcmcxpmt.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2orthbako.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2yezivjma.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2okbxjlks.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fkyqgkhh.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2dyiqgdnr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2qqrfbnya.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cvclhnun.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ywogcrtd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2xamsmclj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2cxnevhlb.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2uyjtmwbq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2wzxkmiac.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2djkynhbv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2mnlkauci.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2swlbetsr.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2dedlnvby.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ngeuuqmz.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2amrmwptr.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2apihjsxp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2oowintox.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iajfaxvz.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2wmhljovw.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2segaljwi.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2rpgqyzfg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dfignnxq.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vozdbogh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2dvelctmr.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2xjsmuxza.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2fxfngzfi.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2aakpqzdy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xnjpnikp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2dmdbhzvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gsrcyuma.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cmmhktaj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pmshwqhk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2jssiljgb.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gksfjjch.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2snkbpfgu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2uhqhwrnn.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2brplfhdn.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2udlccpra.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2chlexpvw.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jscakrdw.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vbgzefjt.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2emveqtao.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2woolulvb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2dfisbnbc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ptqciuvv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2oajdadxu.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jbklchlj.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2kpstaaup.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2umagrzge.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2gbrpwghd.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2fmgyrcma.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tasqdjhh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wqyfadvj.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2wfpregxg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2mlkangjm.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2tuhctdax.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2bgnkjzja.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2atxrhcvk.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2fgpcncfx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2mfnawlrr.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rjfvnehz.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2dszxakkp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2qnqxcdso.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2dkinsbae.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jcxrufxa.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2xkacuivn.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rrscmhqs.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2leauxlrx.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2wvwrexwo.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2byczwprq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mhakmvbt.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fthqeuyp.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mpgnpufp.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2uqqkmmth.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2rjijnfsx.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2lvsfsrsg.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2imjcnsxm.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2letjtxle.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jfjqgtoi.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2esksjqog.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pgdptilc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2jnfzuvls.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2moqjkfnr.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2apcqdvvn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2jcsxodbz.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2lzvitlio.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2damflble.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qonkfyts.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2gzbyygbc.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2durrszyy.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2inaioxya.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2owtpwjqv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2atotjowl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2obxysmwf.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2zzglijtu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2jvkrjvwj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2glarevgk.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2onazarqy.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2xevdpilc.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wlbdvlpq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2ivgsxvvv.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2lqwcwyjn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rgyppuup.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2fhwgzubl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fwhqiowa.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2zotzhoil.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wywsuxfc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xpkgljoz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2csnodlon.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xoatjhnw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uauzhukp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rxkmktcg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2febtbotd.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2yijebcuv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2rhwquuxl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2yeytilnd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2cyijdvqf.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2upqqfdsj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2yrnxtppp.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2rwaxwxxw.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2kryeitwy.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yigiykoe.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2rqyahyyi.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ixlworpt.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2mbwnqboy.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bsfmmysb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2quhrtqfc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2bzqchgzo.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2olmkcgjo.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2txivaqnb.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2edojtbkq.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2vbdqotyz.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ktdpjkna.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wmwhnvqz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2otddcabt.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pkgqkwmi.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hzfyslpx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2bgrjthyu.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2karqhplx.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2meeydifi.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2spqejwbe.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2ytejrnjv.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2mpztqpai.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2rsliwemo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ikwwgrqv.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2puwnhemj.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2sbcstlqz.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2rwwqthuw.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2vdqyjhyu.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2dhibrggm.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rnhdonnx.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2wnuivtye.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2xuzzkcnm.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ibxafoql.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vcenwlio.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2oyvdqksy.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2nkdxhsqn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2efgjuytj.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2kaftkxej.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2jxnujbds.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2anfojzgj.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2kwtyfebs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uzqbshbc.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ujotcyhl.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2jyoscrau.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2guhwyidc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2totsizfz.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2xnhwttpw.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2cvhzqnqd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dzcsmhie.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2sylpcgxz.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2zctgbnve.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2cljqdpis.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wbqtgrot.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xwujttrh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2qqsqidnp.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2wxiyazxz.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2amqrqmth.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2hiwowxdh.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2rxcdtniu.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ylvyzuvu.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2bubzzvan.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mxxoeyim.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2iidvgjvc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hsmjnwqr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2ecahuham.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2nhxdsgmp.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2thiehwna.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkegzlzn.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ejgcmhjv.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2mtdcieod.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdnfdhjg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2ynbcktbf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2pdmtcglb.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sdwwkfyf.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2qkdfotbh.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ljoqrhlw.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2iogmkdzf.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2qypigrpm.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2varosmix.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2bawkkped.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mesniyqt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2znloajti.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2vvfuyilm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2pkqhxelz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dffbalxp.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2noadsccb.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2tqdjgdqg.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vbopekck.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2sobcuqpc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2gyrvcgpx.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2biuubiqr.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2arggzsix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hhjjbwpg.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2seppegho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2quzyojtg.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2stamyvwd.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2lzyeumuf.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ycwgvtfa.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2fklwymaw.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2rvwhvhzu.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2yeblsujp.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dlylrjze.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2ywkykttw.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2csohxbnn.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2wpsgagal.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2ogsnmmbw.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2gpoeheuk.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lwfbhxee.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2nptawomv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2kasilido.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2gyfsoqxk.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2yzwhenrb.html


<!-- 参考信息 -->