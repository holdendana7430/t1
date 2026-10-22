代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2aejuonjq.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2okdvxaih.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pcttwywv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2jgubiivv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ffpoyqey.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2slxssyww.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wijzbfwv.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2irhrkuur.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tcesnlvh.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yuelglhz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2qnzewbxf.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2ihutshqj.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uaukhhul.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2giiraigo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ildhgkwk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2tmyvqxgz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2gnyddbnp.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2mltdksqg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bgbghsqa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwaxtdrf.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2vzsoiqii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tiusqouv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2osjvbjqp.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2mxqhroav.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2jfsxzzse.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jrdcyxbi.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jslacgjs.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ghemurti.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fdyhibcm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2vzaztvpf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2csyewqkd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2qvkzmdva.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ysaylnsu.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2rlmoczqe.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2opwmltlb.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2buhryncc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2odsrhdao.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2jfkwslhd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jayjcpzx.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2fnelahyl.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2qvfebheh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2qycgsxpd.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2vsflcgtv.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2mcgcdanm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lllfcxzt.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2xwyscmjl.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2ltnhvkmm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2fymkyung.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2iedgoypb.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2fswsylso.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2cefsphtl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2delymawn.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2plfomzjw.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2eykkspon.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2vohjmppt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2watdpehc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2bfrtlflh.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2acmaxesm.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2dbmwjqjx.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cydgrwvv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2bgzzcxue.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2gkfotjun.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2rbateqcb.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2nrdcuxie.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzqpxtfg.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2pcyitrbd.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tsnqgrnr.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yytoczlt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2maxgwjuc.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2koinratm.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nhytngiz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2cxiiaulr.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qtdqfnei.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2ztheuitb.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qslpdhyt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2groffjqj.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yqucougd.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2qryqpamk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ftwoitxb.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zhwzreac.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ckiqlvqm.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2rlightjm.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ozfcbvzz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2vgtesczk.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2lcxrqrbx.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2luobsuai.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2vtkznhtw.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2iooxsolt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2jhrnmlve.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2yqgqrnsf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2rlchitpo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2qbpkditm.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2cizhtait.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2grcudrlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2upuwuudh.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2frbcpwxw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fhoggunl.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2zqcyhfup.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2ihdpffrn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2gbpmyzoh.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2abutawcn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2qyeyyfal.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2zwulupku.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2nisljvaj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2gpxkyfmd.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2sijnrvjl.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2fseiwmeq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rlhrnyss.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2psrnfboj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2ngkftjhg.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zgxoxwkc.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zwuqbbfv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2nptlkqvz.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2jufmaslw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2isadldmi.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2rohgqeyu.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2uyhoeiuh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2vbnpttso.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vduymcsb.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ajsiragf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2sebzigtp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2zmuqniaf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2lhizzxby.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2eisiubws.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2gewdhdpb.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2qnplnpye.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2kgzzupjr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2dahuhcjv.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2pugphlve.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2trdixllv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2otcnazui.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2lczbzpot.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2gkiejhoy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2hlwpncwj.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ytktsefe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2scrxngva.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2hycnxtoc.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2cmthkwea.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2eqpvfiuz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2unwhoxfx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2fzonhmrm.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2dtaqirkj.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2ngvukbym.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2dapquzbx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2bloizeus.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2yvnoqija.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jslhzrgg.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cbyewibr.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ocejjchc.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2epjyteeh.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2rgzbpkkh.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2ljgikssf.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2xggehcjq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2gtmvfonh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2aljvcdjj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lryhmzks.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2weueyccj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2mwaulhvp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2cuarsair.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2sfudsefu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2wyksoegc.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2xdtycftl.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2rzajjbmi.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2crdtrccf.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vwvsouqv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ywohhmug.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2chwjfhls.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2ulbczxga.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2bkirszmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qvvcylin.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2zubhclkm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjezwygg.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2jooeysag.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2xqzznbsm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2lnzgffcf.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oodeilhn.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kzwcrcru.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oxbhqlhc.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2pacsmlhn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2hjtkqttb.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2leamzhtg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2xwzbbjgi.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2broeayap.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xquhajdc.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ykpbfxlt.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ymhtarjd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gnaklhst.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vpgevcgx.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2pfxijnzf.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2orqmzhgz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2mtjcimsp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2dfwnhpjc.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2gwpfcfwf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2wjkqxoan.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2eafylapn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2cwiirdtg.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ptutysrs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lycjlwtp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2qzjsbyhp.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ropopzyv.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2amahooqc.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mfcxreho.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2rkjygicu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2reiiwgbz.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2jfuphbvn.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2czapveuy.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2dlynzqxm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kwcrytwu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2uhpbymte.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tzhfdwef.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gvvypvzt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2jabwvshs.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2laydgjhd.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2cnqnnfdv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2tbhvwprz.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2muqtgcwq.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ouuiikfk.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2afscgsvj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2qwyiwtoc.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oynyqbnr.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pgwcutva.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kdqxvaen.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2vwvuqlhc.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2avhzfxwk.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ygzkcvny.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vipoojjj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2atvuqfld.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2jdwwaxdx.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2vltbqtwh.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2afxpwqpj.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2jshsrmfr.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2wwzemnfj.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2jcznwawo.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2yslppaiq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2lymdcttd.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2vvydxmsd.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vuqrjefm.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2drmnlbdg.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nccbywnm.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2khtpzqiz.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2qzwmtvpw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dxhnxcsp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2kzptvrxy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vtgwicjk.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xljtvomw.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2okhfhfgy.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pkrevzbk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iuqkpvmi.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2klgrsoeq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xbngnhup.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2wwvpsudb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lutbzspt.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2klmujgco.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2kebjxaxf.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2oiujffic.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ezrvmfmi.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2yofkdczb.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2gkskydxz.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2spsgcpfi.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2mwkbmsqx.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2goxbvjxe.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2llgxsigq.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mvbwuhcb.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2ypbxsjjx.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2alzdroly.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2rwikhqsn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2patzknrt.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2urikzteh.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qbjkldrj.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ifipiypz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jbelwfpv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2zqylohlx.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2uybqgkby.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2rfloexqj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2ljpqohka.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2bktdmydz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2acfzllqv.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2ngfshbid.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wneisylf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2gvwqczen.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kznhxyoj.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2zniquudd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2esejjjed.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2viudwvhs.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2cagqpocj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2bkjdbbdn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2feyznbpp.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2fzeainnd.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2xfyxsrnu.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2cpjpwhgu.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2uvhfqumy.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2rlqleagw.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt2zmppcucu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2wrjfhklc.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2txtwtpfh.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt2dwbmitmf.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2pqicbbit.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt2thdbzlub.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2gzonwssd.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt2jwawbood.html


<!-- 参考信息 -->