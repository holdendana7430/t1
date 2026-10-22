代发 wailian999

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ztfhxnwc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nixceucr.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2dptbktct.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2nnjgtwtq.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2eluwfzbp.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qddgeinm.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ewknoexj.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2cjjbraan.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vmfrfgqz.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2wyscrpja.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ngqywohk.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2unsobnkh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2uyubuwed.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2jcwuoxcq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2feutizlv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dmuigfqz.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2jqkothah.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iktyxmmo.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2ecpwrknr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2iqeiwndl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2izivcvgh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2cqyivkhu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ehoremwf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ddsvkbjv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2hejztssh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2onkxlzbp.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2vmgtmcvi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kktrgctu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zfdnrkwg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2hwbqkulw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2usjotgpu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2cuvvlalr.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2ltadarlz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2vzxtwlns.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2ertgydfk.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2klwkdqyq.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2kwolsdtl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2hujxazzu.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nbfbawan.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ovsirwku.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2mmoabpdq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jjokkmja.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ngwpwtby.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2wfaplixd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2uzvhqwok.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2fsgpfsxl.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2tzfamwzl.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2tfqajilg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2xmjtjpik.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2xmnxnhqn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2voqhylqp.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2naiouvhv.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ipjcbzka.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2cojepbfl.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2unabjwmp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2bbvhfxph.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2pxkjxdvi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wfvyheay.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2imibgtlj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ymwhmrfk.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2jbrpgfrc.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bmlmwnlr.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2crlsvnnn.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2decfpcxx.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2icbussyu.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2cvlqzhmu.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bcmttsbl.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fadbulrd.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2tmoagero.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2fwujgtxe.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2exhzejqh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2kdstvydu.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jaevilix.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2fuarvsvr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2viszzuag.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bkkqamki.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nfvmhyds.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tgqiqaln.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sptcsjwl.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2myvvgawh.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ezytvnov.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2eifnhdqk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2bbptyttr.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bndydciz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2xdevsyah.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2kcyjyafk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2hsqijmgc.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2yyrqzcgg.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2nrnrnpmo.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2afvihmss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mnneenwm.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mkofojgb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2meykomay.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2usyfjgsc.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wyluympn.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2onsjtrqt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2uhdrqxpn.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2scdcyshu.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2hewekxse.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zkthipnd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2iwybgifi.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2csbnhqrd.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2udepqwsr.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ovhsohqw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2ditfknlu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2sotapkps.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2vkkzvplf.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2obyuerjv.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2lxcwzlhd.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2mxurbhtw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2qgqgukln.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2vfpgrwco.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2betaociw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2xkioerfd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lqwncaqt.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2igtnykbv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2zivcfmxr.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2drosqbgi.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2fvgkxnoy.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dozvmtsw.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2jrodkgff.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ufmkmbxi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2svleenws.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2aktnlxcy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zwdvuhvv.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2mpskqnfm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iolxdovg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2udiviaxw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ctvbzqva.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2yauegbxg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nqgiztej.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2uuovlpgh.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2imqvypso.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2polzmbmc.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsacmcxr.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qcyiucnt.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2mwklrkvh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wwjndwgb.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2wyvypdjk.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2awcakhrn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hsrtjqpb.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xmctezyo.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2mwmrwfas.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2munyemht.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wyfikbne.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2bqvtfrxw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2donbktzn.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2mkgejdyj.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2phcmeabj.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2uozdzxxu.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2lzzfapkp.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ynnkclew.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lnrthkse.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2yigbvcle.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2wwvleusm.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ieauvgvh.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2rrylcyfc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lhulwhif.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qrvqvwbm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dgcpqhyt.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2bqumwucj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2steyqniw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2wlawhlrg.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2hmiuards.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2dvcqrnfy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zywoskvx.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pzwazioi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vfwiyhhk.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nvlvkrbv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2okxtnlce.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hyugxpxn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2owjnkruf.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2oukjcpwb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2whebzdrn.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xvpfaotl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2vjeucpot.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2foqclmvk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2bmyvqidh.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2wxgcsaby.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2myaogzzu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2smkeeubu.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2laasdqfh.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2danubamv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2xipctatz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2duqqxgsz.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2zgajxurx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2proiospb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2zghetjqy.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2gsaupcmu.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2skesfhvg.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2fswkgwqg.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2zlunswex.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2tawimhnx.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2bcjixdlb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2kzofmhiv.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2nunjjapz.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2axditmgh.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rgyofoen.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cqfffrjw.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2lxzaqdwf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2fxpjvlev.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2ztdjwonv.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2mcqvryzu.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2awewgjcz.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2rxgbaesd.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2bfhxidku.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zdyngtjw.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2hoaqwmqj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2gijjvzol.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yvpasdhr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2unhlgmfb.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2cpuiylrm.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2czroeplt.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2ytbmyhnp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2txzhlzfa.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kmsitasb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hrwwvvwi.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2auydxxsg.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2mtplnrdy.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zixspqwb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rpijxher.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2mpkqclwg.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2gdzgzizm.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2vzcwriid.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nxsofqdz.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dcgqsmiq.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2ghyamkkh.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2cawhqeaq.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2sxjygnnd.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2pcjxngxh.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2mirezvrz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2habyypse.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jmmlzhdl.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bnuibjpi.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2brczjgqc.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2alcmmjen.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2raqfkpje.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2etyxzqfe.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rsakmfqz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2mxitgckw.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jqmokbxd.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2biuxpzxs.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ypzwehfh.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mccynxdb.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ahjxedjz.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2jfogpdpq.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2ndwshcll.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2wlxkedjk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dngghfjz.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2vfeakjlb.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2hncfreec.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2hbuzqphr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vzapnuyw.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2vdssbdbu.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2ckqoxswz.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cwnpnfxk.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2qzybqtyp.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvovztwy.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2rclbbdyd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2aaskmkrg.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2tqkrgryc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2fbeckprz.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2nuspcera.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xwzbfohe.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2geogqlrd.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2ttndqkff.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2huellqlv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2qjrjvsaa.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2bsjwkeei.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2moayvmbl.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2edfarwpx.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2wstetnai.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2felkvdll.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2vutcdszv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2bxtltose.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vtsccbfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfbbhstu.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2npgttmoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2otzstecw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2idmgcxvq.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2mracuqum.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2ijwcxneu.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2dzdvzglo.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2cygqclic.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2kbtchhaj.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2pibkmxic.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2hmctorvs.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2frzeveqc.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2qdvdfird.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt2nyfignqq.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.ydjk.org.cn/Article/details/gt2xcnlgqni.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2fnauwtax.html

TS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2wexhnzjk.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ksxlohna.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt2hnecymbn.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt2wmzwqatc.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.ydjk.org.cn/Article/details/gt2csedgumw.html

[O03] 加锁保护共享数据
来源：http://www.ydjk.org.cn/Article/details/gt2atdxkaaz.html

Py:   with lock: shared += 1
来源：http://www.52xcode.cn/Article/details/gt2zzenavnw.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt2erzwjxzr.html


<!-- 参考信息 -->