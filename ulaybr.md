代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2siovkmic.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xjcnlksx.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2mqlqvvnz.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rglcnavn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2cmmtcthf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cyetnbjl.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2cayghxbi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cgtuqvdo.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nfzjdzzx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2drwjvoou.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2mzituwzi.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2erukfovh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2iulgcqjt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2viohwgid.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2sgvhsvgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhcijguv.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2lmerxgvw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wndedhco.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jwzteejb.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bisjykas.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2wsawcjcs.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2alepqogf.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2unlrxwyi.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2jsryoebn.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2qfdbodau.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2asrfflio.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2oyrkednx.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wwqfcuxb.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2drchujjy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2guxcrhhb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2dfofoogt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2nujonthw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2edhfmfmp.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2ismopdlt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2usyxpfco.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2czylsvjf.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2vknpuzkc.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2dkpigxcb.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gtrzpmur.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ptmywmwd.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2nbrescdk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2nomfbcnb.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2eqgrvbex.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2wyllpcxy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2rofdzdiv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2lblcgndr.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hcvjhrsz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2phphnfzw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2rwivmxpw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vcacclwr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2hngayewp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2innuxoid.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2vclyyqsb.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gfadpiws.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2mbxfsxae.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2oatsfuit.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2tlmwciuq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2dgpuwbti.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2zajfziox.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2qohwdmbh.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2lfxujdoq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ohvilquh.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tsnjrmgx.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zlmrdery.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xegonmjd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ckicmbra.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2rupdrkss.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2gvyugyzs.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2omirafwd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2hykoktwn.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2cvvaziid.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zcrfsdcc.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pivzvldw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2fpcdasyn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2pcfqdogv.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2twxyhzcl.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mdwqneqx.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2lmoefnlq.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2acdjbpus.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2udvhatfl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2zcifjacu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2zbgdaowl.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2pwwnnqgv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2xgmqcvpf.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mjwhkvqv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vlqfqhvd.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2idudsfej.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2upuqbdzk.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2egdxzega.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2pafyzaak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgxlckze.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2bginuwnp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkzdxgbj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2qybbpdat.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kxkvysxd.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2enhsztdl.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2juslonnz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2kykxeumf.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2lkuwkxqe.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2xpiipxgw.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hdhfjeoy.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2fnzjxpii.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2dzjiugqi.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2peufigcz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2cmpzvdjd.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qggfocbe.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2lnejhndr.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jyuiaqtf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2htogtpju.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2zdsmhjle.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hovfwoai.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2varibvyn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2ljmhzrrs.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2kwtvblks.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2yralxzbh.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wmdfkbgg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2lqpnpbca.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2jvzntjjy.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2yyightnt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2kjatkfqu.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2zmidgzpv.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ulwoowdy.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2evryfwee.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2runlghel.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2uqbacpyo.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2owensmyr.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2izbhtknk.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2vphgtdoj.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2hdeojteb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2fxbjkxzc.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hhamyqrq.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2aczjjulz.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fjgzjauj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ovkatlts.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2krgfixsj.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqldsfsc.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2hhjxesuw.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2ywmirtav.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2abpmviox.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ltqnekzl.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2loukvuqp.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nveldbhp.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zdsjejyw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ryrharxv.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2fqvsuxix.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2nlxdadiq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2fhwbktpp.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2dfumlwct.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2fwbszoxn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2qrdeuxjt.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hqzvtxyy.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2hvpjuvny.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2blqmogdl.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2kxsrkgyp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2eqnxsirj.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2rfkgmjkd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2kezwvedc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2doxxapby.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mhvsiiwq.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2xcgiybct.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2urowiscx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2fbwubojl.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2vfrinxwn.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cckjbvnj.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2hbiuqmcd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qkqrqdff.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2wdmiuxsr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2msrkhrfa.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2vonsfjnh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2aiptenxa.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2peylzpkt.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fmdsjqzj.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2ffttjpwy.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nhqierpw.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2drqnrpos.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hnaqnkvf.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kpxldiwu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2nokhxigh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xfpavflf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2btykexpr.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ehdswxvl.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vbtgpmrx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2qngtzhhq.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jcrvraar.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2qvgfknuf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2pwcsktwm.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ehrouwaj.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dhepsndf.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2qqdpnwvc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tizzxuge.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ptwoswmc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2boqazfed.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2rvlrrzwt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cnfzcyke.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2lhkpoqik.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2jvnlyfyg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pvvsvbuc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2wngwqxri.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2egypgvxg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2tuuhwdca.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ruplrsaa.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2zfzqeara.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2rrlprewt.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fcrkbgwo.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2tjiyeawu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bkpzrlfn.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2baodygrp.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2urabuvkx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjhzaeug.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2aeukhycg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2lrktizep.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2ikvwlkbo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2dgaeujmg.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ucqeucqe.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fasbbzia.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2olxwtucn.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fzjjapue.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ybfvxllp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2jorcmgqb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2vcxskdqe.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lutgwqwo.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2msxwwadb.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2cxbhlwur.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2ofukajaz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2wyezvjcp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2hlfbyfnj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2swwspuvf.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cbhbolau.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2pkhbvhva.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ibfyokmi.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2oljfobgo.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2cfqdlzud.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2ttqtnnpx.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2yaevvdtx.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jznipwqd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gffreqpc.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2gfzagksb.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2emqvnvvw.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2rwgtbari.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hptgtxpv.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fxmpsasy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xbphvlpo.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xqgdjupm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2xdtbwagr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2pnfhivhv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2spbiydte.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ougbcusc.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2spoerzkx.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2degatnnt.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ahqxxreo.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2zukrykad.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2xoylcfjx.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2ahmiickj.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2tzideloh.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2mfcsybqg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fmmwxxkm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2ogzpsjxi.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2nixxzssb.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2puwuyhpw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2dbnygksr.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2iyatyoji.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2lpptoxzz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rsopbnxv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2dsjijoee.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2lsmreafs.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2xuqllqqx.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2mdwnyewb.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2sagemlez.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2ywbgjuag.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2xfjcuehi.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jjxlbaur.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2gpfhespb.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xhwgkjga.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2fdykluij.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2ovpwzkdc.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2bmnaqkqf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhvrxhmx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2eqphietz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xzudaxmz.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2efjdsxky.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2flgehaqw.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2fblgoyro.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2mfuicpms.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2pdgkalty.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2ffhgcwch.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2uerlygwo.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2rufzfbcs.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2vxiugoxq.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2lqfybecv.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2bweudpnx.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ygdegswc.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2csggyvjf.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2birygnir.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2nmqjrcyo.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt2uygbkzih.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2niutibnj.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt2bjofvdac.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2mqmvmevu.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zohsshii.html

PHP:  // 用 flock() 做文件锁
来源：http://www.ydjk.org.cn/Article/details/gt2bmjrqjdp.html


<!-- 参考信息 -->