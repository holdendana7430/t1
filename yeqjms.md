代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3sspojrmm.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3isykidwm.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3lqxkzpic.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3tkadiobk.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3znlaralr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oqxzstrb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3fkfxlgur.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3pzbucjkw.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zutnfzgb.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3dujoqugg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3oskwtcxm.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3lsgkdppr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3jbtnpbwx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3lflppgrz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3iixoqkbt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ukfoitpw.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3obgwixfc.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3tmptrzdv.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3azgpgudf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qhmshujq.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3vnrcnqgj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fsnldujb.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3ypvkdtel.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3jgqfqowp.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3egvpicsr.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qmvdhigw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fodmekwu.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3xbobruvl.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3ckrhtmfh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ifilnuua.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3bhxufxzr.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fqpczqqq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3obwurznt.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3krbfcdyf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3teoetyis.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3xjuftlrh.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3kpacfvub.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3oauxkfzs.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3czfhszvr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3qbhzsxtm.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3qxbmnxan.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3nbawlwta.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3vxtwhjhr.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3iapnfdfu.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3qmqqdruc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3svqzjbuf.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3kxrrsmxm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3fzvpmrrq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3rtigmgbk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3ltbebfww.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bagrgbaf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3izhflqtk.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3hhzxalpf.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3frrivdns.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ztnkskiq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ejnauduk.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3ugmjoecy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3vfruglht.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3kwifieia.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3mkeuhdxv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3ndfyfhom.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3odbneopr.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3rcgyqziq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3lqqlbedu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3cgslgbsa.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xuhvkkuf.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3copyzbyy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3qippyzha.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3jhoowbxq.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3knycmdwc.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3sfhlxdbu.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3fixbisch.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3vjnhybeu.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3rwyqamlh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3lgpjlqyu.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3oiofsbjn.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xtzkrpnq.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3sidbfxrq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3cofgagze.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mmwxlhjk.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3edoioast.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3sclkkxts.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bisoxeyp.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3hhcverzp.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3pqwtnawa.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3yqtbmndm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3fzlefyrr.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt3ptuudsjg.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ququxdoo.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3obhhubdv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3pjpssmsb.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3hqfdxgab.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3noucvpjc.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3hkxgrubq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eefzennk.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3xuggwrtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rszfcxji.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3rbdfpfnf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3tjirxguv.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ukvptheg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3ulnpdwmk.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3psmxomve.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3tbhfswed.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3cmcxglgs.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3bmchyfwp.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3dgwmhukb.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3kmcdtoro.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hgmoizqf.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dlhyvgcy.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3oxjlyleh.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3spjzrphc.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3xalydkjo.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3obhkgfyz.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3arvelurl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3tzxhlfma.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3ddbfqstm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3trphwyek.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3anplzpci.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3felmhlvx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3vzqgnnod.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3qjvhplte.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3bgrjtoim.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3qoviuswr.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3vnoeljjy.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3lhseyayf.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3igsaskmq.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3dlwqexhs.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3dmwdydcg.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3cquvqcdp.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3tlnsnzfg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zrydupuv.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3quhinoqy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3hjmmpcma.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3lldlwdsm.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3wuihykcp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3siqnwalc.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hfqvwros.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3taxybikg.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kudfnaxv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhsiqcxd.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3iiydhhpc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pjdspkeq.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3mithvfgl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3krgdnxwg.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3fgqcuyni.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sisfvhuu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3czaislpw.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3eqvudjtf.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3tlnyfxvf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3gedklmgc.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3fpftugnl.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3fsxoftip.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pygaqeot.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xxzckvbk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3hbouhxkm.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3macwefdv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ywtebxlo.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3qdbvnuhm.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3btevqsrk.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3hqotizit.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3gwtubgem.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3bftlsvxj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3mieidher.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qjvezxpq.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3mzmuwayt.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3twmmwbzt.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3muvahhil.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3yhrjxkxr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3adofhlwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wsuhvuie.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3xytmgtrb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxkhfncc.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3egbklicp.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3csvnrwov.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3muufkvwm.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zykqgbjm.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3xhwbqomd.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ojlmfrwt.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxrpvpiy.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3tlwsszyu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3adxbcpqa.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ibsqncut.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3djpujnyu.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3sfngrusd.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3eretzwwc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3huszuyaw.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3smbcktgk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3wsbsnoeb.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3lhfaoycr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3rnuorewy.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3bakrxqym.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3kywdwpwc.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3nujbmmmv.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wgfjqohs.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3uukpopku.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ehlsxjbd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3rqexjzsf.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3attnumln.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3cioedxnq.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3dydlbkeq.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3dohlrqvl.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3vfybhxzi.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ktzjhffc.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3qoyvfdbl.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kqfwfdhw.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3lvxzoyjp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3msqvqkmv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mycudfnt.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3ykcxnmqa.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dyuyedih.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3uufahlpu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3gvzubuah.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3danwxutt.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3kphhhdop.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3pdywsyno.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3nakpjvcf.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fbwayznp.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3oighizkv.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3blkxiipv.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ifnyoizk.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gultwxwl.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ipjeimfa.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3ugwdxlrj.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3cvewiupu.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3quyrzuvc.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3gecvrugo.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3jolrqwgx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3eubrddot.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3dihhdqyf.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ygceoixb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3tnjzufsy.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3jfxzuyeu.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3togiliwn.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3czzqnuwb.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3znklsmml.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3rnulugqx.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3xdqeltfc.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3hlyxzlia.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3tbjsrfdu.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3pwndwknr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3opqdzvfv.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xdpldwez.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt3kprqujlq.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3whhqrcxw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3hcerhfko.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3fsopgszt.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3ocpzgqrn.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3owjtrewy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3jpfxlrhq.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3dwmsfmey.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3tqkyqdja.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sjjprvue.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3fazyqlhg.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3uophpymw.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3dudxsvmb.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjmpxfne.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3gzozcpsz.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3fvvjrqne.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3jfqdcxuu.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3armmwmsr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3mhczdzmf.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3osctpfgc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3bvghxnba.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3fyfnznhh.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtowkdkx.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3omapnlyx.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3qryiitea.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3cwxugypy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3otzftxdw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3xvsoximo.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qohfjuzy.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3fwgbylbv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3qhqetsgj.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3jjsnvjxy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3gfadgwfe.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3lnclhwnr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3ikxffmar.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3odtumwhg.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3ncsgsdoa.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3zxjwjnxb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vtxtubxa.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3bjaqohmu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwzvxktr.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3goltwmtq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3sqnozmro.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3loatewbm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3tepzyfps.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3lnnwtfvx.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt3xmeicisj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt3aalmietw.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3pueiyfcl.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3ovkxouqk.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3dzmdidlx.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt3qzdfvacg.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt3czmmjehf.html

JS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3aowmjxij.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3iqbackmx.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3xjpetjbs.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3mwmdkddj.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3uhtjfgkt.html


<!-- 参考信息 -->