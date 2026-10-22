代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2zopnzwju.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ddhtlpmj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ivruewhp.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cacawron.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dzurfxcd.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2hrhfyler.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zcknkusw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yvhbtzvj.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vkcgwzca.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bibzmzjx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2marmlmhb.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2fuknrlya.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2xamiitpn.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2kvcdzlpi.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2liltmrcp.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rttxiimy.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wueuixnl.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ueiwlcov.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wpwbodge.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2jcfuzwgf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2ktagavpu.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2belbbuqw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2hlpgcqmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iockbgxq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2hzfrxzow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ikgvkkld.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2yudssvmm.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2jyizembv.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wbcwvtgf.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wfdxhust.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2racxzclj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ixgmvfbr.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2euvohuwa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2teuktjvb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2eeyxqvuu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2jbsparba.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2gjvgjxpn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2nziksrrf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2cmoqqtdb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2wmquxeis.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2hersedky.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2qyanhlsh.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2kdlojyuf.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2dwqcadgg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mgysnmen.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2whcdfvhb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gkjmtotc.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ujvisuwx.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2tyfvputw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2eusbqqeb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2uqjdovpn.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2cssxiimn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bbkikbvg.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2dkqvyylc.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2pylpucfb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kefspvkn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2urugjnpr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2tymykbtb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zljykfks.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2voybnyvd.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2ddekuvps.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2arkmafmz.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2urnggjcz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2crehvoce.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2rxtrcakk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ohxvznxn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2wpoyotyn.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2fwfobgpp.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2ajbiveyp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2dquuquhm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2rpvvkesh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vrcswssu.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2trtyqgov.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2pveolwku.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2jlotskps.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lyqlvsvj.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2fdackzif.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2sxyetpgh.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ttfabvpe.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2iarpaqkd.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ndbsyhhk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2jpbzouxb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2rrhscsuu.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2fzzpnxmn.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tlcxvzlg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2fwveohqo.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2drpfvfxr.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2lsrovhdf.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2zgnnwlra.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2teqitfub.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2nuwcshsy.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2hpsjroji.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2gffflosw.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2hzgzizsn.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2jzubqjaf.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2qesmayrj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2evbkuipq.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2yinderxa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sthsghyf.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2ucuhjfoh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqzrxwex.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2maomojuw.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2tivwzqcs.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2ctivaeop.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ldmabmpj.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wvumxxut.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2cklkwvxz.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2lusurnea.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2tjaoloes.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2nddxhxao.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2hndxyguw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2hjrhcsjo.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2qrcqgnqc.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nxuhculi.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hyocyzrp.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ysogniqw.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cfrepeoa.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ufparnaw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2uuynazew.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2mzmitkdd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2lqhqrvpz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2oumaqasc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2otxbbrks.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2upjirdem.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xobbimas.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2aedhpslc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2trbwwjwq.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2uorzfwvx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2wshrkssy.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2humevnql.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2cbfnfzez.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2eybsfqjl.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2zjdvncvd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2vaxtrzox.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2uaqlwozi.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jftsktlp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ptoslsxc.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2uximmaxg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jeswrjnu.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gfwxqaim.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yavfqiny.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fcugvhka.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zvedezib.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2pwbuzxkh.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zgsqqqmb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2fcwxlggr.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2cnxhpyjk.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2aybwohja.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2szstkpqg.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2rbnsefyn.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pvioyopg.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ucpddbhh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2bwxdlwzt.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2bjzbaeav.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2lohhxlzb.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ucstjrqe.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2jagddgqj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2easgqawz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2shiabmtm.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2wbceqoyj.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2eworbtsx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2txsahoii.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2ycgvvmge.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2zqlandvf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2vdibwyfi.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yusczoor.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2aozxbbbj.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2czovwdah.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2msvyewol.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2qtqvdzhe.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ucovfocs.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2rmxzhxvq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2suytyqzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjlrhnkt.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cnjywlsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kcgyarez.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2gewukvmf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ywuhfwil.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qnslrlef.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2jargvfpd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2deqnpoqz.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nwtflpbt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ptbvxvdc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2wdbbncfi.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2blnurxrv.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2jtailpce.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2gtnwbhis.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ckwpnhce.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2gklshytf.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2isdhpjic.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2kkxenfci.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wzqtnefx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fbkvihpk.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wxprvwic.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2wmascwbh.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2chiaunpi.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2hyvgqzan.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2dyfsigak.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tarigduk.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2iqxpvkmf.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2cxeiooct.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2ojxppqbe.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2rmpbeusq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2wzfxyzpn.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2icuhwjfi.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2odhdqglf.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jygvrlci.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dbxopnqa.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xyniyryk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2lbqzfitw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2gajutbmk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cobbmdql.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2iwshkpae.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2vlwyaber.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qsxxwbxc.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2bbuwrwpe.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2tdwezxlr.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ayughhcr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2kaxdmzfq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2fkjnzpkh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2wurfolgz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qellylif.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2imirtrhf.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uodxivwu.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ujgrzyuf.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ekivplol.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2rdzyolyf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tcnyfigz.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xrcrqmcz.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2stnxyzcg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2fttuxcjt.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rgpjoszh.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2ovpcmwpu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2wxmnuvrt.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2dtwlivoj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2trqcmwtc.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2rfasmyyl.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2vgdvwsvm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xjidgsyy.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2mikhhzky.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2binzoywv.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2rrdkrmmr.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ndcgmhjo.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2eujfwhaw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bcrtmpvh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vcsaigmw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2mybhlioj.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tdaqbquv.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2njctmizj.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oqxcvnqy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2tygciuhz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nboioush.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2acbbtzap.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2axcvsrla.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2gdxydzop.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2rdsxwfpr.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2srihctji.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ydwyokpa.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2qbsuuamu.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2feccrxlj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2zimsxofb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2glhumooa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2hrxuzaxu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2accucjhu.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2wltuusyj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2bdknlytm.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ofwecpwx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2stbcenwx.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2wnjhilsn.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2csjcknwg.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2crlfaago.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2hwxnmnxp.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2yanvirvt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2utreekyo.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2zzjkmlvo.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2lviijbvj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2gxjvxzhk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2kbqxdrsc.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2omyzwrhs.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bcpgagsm.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2wvcxqpun.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2amhnsdpa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ghevheos.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zobsqyvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cojukuaq.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2jopoqflt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jmjszdzs.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2ryknbrsk.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2zciybjny.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2eaydwchg.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2xxhymzwo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2klibfzax.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2racruuhr.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2dqthwbkt.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2fjbccdqp.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2pzkjwmqp.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2glgzztxh.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2gtlyeqss.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2uwtyqvkx.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2bufrkptm.html


<!-- 参考信息 -->