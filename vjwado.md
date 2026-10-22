代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2hlfrbiti.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zpgylynn.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2vpewmdne.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2slvpxgmn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wrzqojae.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2dyqhenpm.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2evprmgno.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2bnddcqwh.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2dndnbfez.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2juegquse.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2hpdhfgnr.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2jjvvdfhl.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ikrtjxwk.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xvwmzrns.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rtytmkex.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2enjmyojs.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ivmdrllh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qlgmgjdq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wphapkyw.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pqvyotek.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oruggadm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2virnftlx.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tfzipfkd.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2nygttnhy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2igonkrff.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2migpxsay.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2vhzkixez.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dyxfkjpo.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jozkqodz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2apmybblg.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2txnustel.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xhzpcfaf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bijzovns.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nwqhxcij.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2crpsavpu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2mixtqybq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2xymisfum.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2mfouxxzp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2urghxark.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2muuwwqhf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2rfomanld.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2zrjkkbgg.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2qnqwfamf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2aalxoipb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jcsxjaou.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2iqnbjsyk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sitsgeju.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2jmatrnbt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2jbxpoyhq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2eggcvzsl.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jihaiacp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2iwrmnwht.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ridmtjhd.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2ofnlqize.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2loermuav.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2tyyxcqov.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2bczjsifx.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2amicbopv.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dbwaksvd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2jliusaks.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2oyskjvor.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ceyrpzxo.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2tgoykasu.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2mjqowbbc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2rsuveawr.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2mqqeqmgk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2zniqoyqi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2enwssald.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2fafmloby.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2lgsygjqs.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2rlkixbvh.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tansvldv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2gcfkolfm.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2zmgpjybb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2suxlknuc.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2vflbqxrv.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lkglsmxr.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pwaraoeh.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wbthvrlu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ulryuznh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2ulbkaedk.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2sldngllg.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2fxhlrhma.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2xciixcim.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yeklcnnu.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2cddeckgs.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2zkgobjay.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lplnopes.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2pidpsyww.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jxlqhjiw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2eiceoxsi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2irimyohn.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xhoagabi.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2jckgblwb.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2jfxngony.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jyvnmnws.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2zxxdwxqi.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2kqsvnsqr.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gcrlzruv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2hksucscb.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2gosplpzv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2vdogzfaf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aoqblrfr.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2uxhurbzf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esakbhze.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2xayrmwjg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2hodmclxy.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2feyvkwky.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2wdjpcsys.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2qpbnkwmq.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ksrgbbic.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2iwjwymcs.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hhorpxfj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ifencjdr.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mxrbhjxy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2byzvysdx.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2jekzbaus.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2hdvypkcr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hhtvrbdf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2iiisiykl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lzhfyzdq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jieibzta.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2otpfacxh.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2wlynbgxx.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2bshzkrjk.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2rtzvfxmz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2cdjxbcnh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2azinlbat.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ejoxqoxc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2gahyfctw.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2dfwdvasf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2rrsryojz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2xbamxmsz.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yenldkzx.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2mabdxrzw.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2frzazpwi.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hfmsznhe.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2ubarkmib.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2reeiqjmq.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2aloiorgh.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2wqkttggk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2wmiruaak.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2mogyqzdy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2xkjjmfty.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2fnaormmx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cxzmywwe.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lzvemqjh.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zcrodwoi.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2avbtlqra.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jzmqznkf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2uxibotou.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rvpsbqmi.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2pegbqkwg.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2pqfzsodz.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2mzjoanhp.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2mcmxzyap.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fiaqympp.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2rjpoazpj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2wthxubmg.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2vmwbzqre.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2tpqbjvne.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2hnrogvcj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kwhptxyb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2akuskyra.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ejgpcnol.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2pvtalsjg.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2whmgvmpm.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2dektuuoq.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2pzyaujsn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2trqhzpqo.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lyeelriw.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ptewsrjv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2acpfsnch.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2nroigekx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2hohxsekt.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hxozyqqx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2gftpdvbx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nqrjisfi.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2uxsbmyzd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kozfpztb.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2erkcdpxg.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jalnpain.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zdlterpx.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2nwqcusjj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2msngpcbm.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oqcxllho.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vmrkmuen.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2ggluxmfe.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kcdwmcvd.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2qwschxgl.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2fpbxdfqd.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2whmujhwa.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2iwrqnhvc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cfnctwrx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2vbserscw.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xdebcsoi.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2xekvdebf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kuxyarna.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ibolvzvm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2sgzxnzmb.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ygvhaygl.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2jakhinrq.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qadktpbf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zzjkmdtu.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ohevqczr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gqpcjspy.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2kooxuram.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2vowejcdk.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2nuaznuvx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2nvhdavol.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2pfgkuyfo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yqfzxokv.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2vfocsiqp.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2wlnlydmj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2qtvutrxc.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xcutoznl.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2danoftiv.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zhibsijs.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2chrxmmek.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2vaaidzjm.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vuexhbug.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2fvyindge.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xyxswhml.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2xctfowvy.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mfqzbegd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ciminans.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cssjafdy.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ymejcxhm.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lqwwoanz.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nklbwqbt.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2sxavdnye.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vuvflndw.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kspvhpnf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2egrwjtjb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wlfodifw.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2yverrsps.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wmechnca.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2khcpmhdk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2dqyjuuzt.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2rtaofxua.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2hmuwjxev.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2nexwcppp.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ntpxxrgc.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vrpdlypu.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2farytjly.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2btepuyss.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uautyimy.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jaohngzp.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ymcgyzzb.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2yzhaamfi.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2tnygijie.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jnzavfzj.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2grqyygay.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ypmlbwgk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vkwotzyl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2vdtrrwyd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2fvbzgvao.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2twfvjrmw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2waugszvc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2agvwtkhz.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2yswflwhl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2dzcezwqi.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2uypardjg.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mosmslxj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2emfqazwe.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2nayvzgpf.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2oppcsahb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2bfripbqf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2quiauvve.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ynrzeths.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2poenvvrz.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2yqddmpuq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2mfcpvdpk.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tcbwgmat.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2xhuhjnlr.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2mwpwtqnn.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xbirlywp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2raanrqxo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fzywfiwl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2iurxwqyb.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2klolprxq.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2ymoourew.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2mayusfrl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2knzzatbs.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2zjifdyba.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2zqrqjczu.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2abyhbund.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ocduzylo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jootmssf.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bfuqrlxq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnadlapz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2kzsfwffr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ylzhbdco.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2glhljlxb.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2cychyend.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2uleqkhxt.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2rqsbiamv.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2wuthapar.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2idacxqjh.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2oalalzvf.html


<!-- 参考信息 -->