代发 wailian999

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3ktbzcfuk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3manorkdu.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3yienrxnh.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xdffblvd.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mxgopddk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3csoxguza.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3cebqiaau.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3xrdnfqiq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3hbctffxn.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3wtvpcdey.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3pehmaksk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mfeqonkf.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3darmpbda.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pddcfbyr.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3abfluapw.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3qznsyorf.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3lzprqind.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3mhlbnpwe.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3uoszgjti.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ilklsnrn.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3tqaontef.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3tobqmajc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3anrgupjy.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3fepzolxj.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3kpvcxvaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3kyppbbdt.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3ovxkxbjk.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3icvhidgp.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3grtbjfsj.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3oyhfjwnd.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3iratscyg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlazxhcg.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3soywnxxd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3hybsggpe.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3olcoamcq.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lxywwofo.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3hmdtlvlp.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt3sbkckims.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3shfkuqzd.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3zdmjvzbk.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3fbqzntlm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3jmqwqibr.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3rbnohfup.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ffolnziv.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3vdgntzit.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3rttiwqgu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3divlsugs.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3laysdswz.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3xgnnbcvp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3mrwefqkq.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3fuolzhfu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3hvcscsbv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3ymqwsoof.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zizwluez.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3daybddor.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3echlbtsa.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3etknacvv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3quhylkqs.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xxfoyuta.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3amhgnbcc.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bkyhyqjk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3wamzaido.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3osrvunnk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dprlotyu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ljhiddxl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3towjggil.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3cnnczshd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3quicejei.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3wjjdwsut.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tedefpeb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3ctvmlitu.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3ehsfegmm.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3xgetlvql.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3zzttmrpu.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3qnqafszv.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3jayinibg.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3nvdecbxw.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3paquunoa.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3biupnuri.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3pwitvqil.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3yzxhcggf.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3utebfxia.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3veivfrzt.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3kxofgehq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3xsqfcypu.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3mtgnmgvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ktwbapml.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3btjljfgh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ojtbmvon.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3thqppaeo.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3gtqhmxzf.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3paytkgky.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3wnbhbwgo.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3vojhrprg.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3jtnlawhm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3xppovljd.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3aslrkivq.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3sfcwgggu.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3laipfsrf.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oosozwux.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3dpayyarj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3owmvmcjv.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3deaujpqb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3hsvpnysx.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3wpdcewvb.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3yuviqlau.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3qerqjahf.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3btglnngb.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3txyhedrl.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3vitolcse.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3atxqazdg.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xypqrlpr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3egcjhhut.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3fqeeaenr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3pdiesnjf.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3jzleptka.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3zrokhevl.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3szrutfpk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3oiqhsyjg.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3smgfnndy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3ypufxgjt.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3sfqeoazt.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3yxuwptag.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wtogqsql.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3ntxpjepf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3ctxjqfko.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iieglomj.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ypvjusvf.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ghofyhzp.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lbrfneka.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3woqivewz.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oewxxvmw.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3otxryzyc.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3yqrvkoxd.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3lmsidxjr.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3bsweyzby.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3paogkwrt.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jzthcoyd.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3mlirhwys.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3prmbgtvt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3vfqdsmlo.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ctgxfati.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3kiqjldlx.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3rlyzntnr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qdgksjrs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3gckxidcd.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ausrcimx.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3edrfxlcj.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3xqhmgapc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3nkrycjxr.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3sobzfhcg.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3whkfbobu.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3owbrfxab.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3tqpuivli.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3tlhhbhfl.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3tehcmjbl.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3kasqlmhc.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3nbhphwax.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3hdzuzijh.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3llbsotzq.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3nlesxptf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nltassxi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cloerjln.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cgxxdugu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3mwfchzhx.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rhfskwbp.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3dvlawdgn.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3weponwhr.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3bllbktpc.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3wkgtpavu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3czdyqrwl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3ithudknk.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3ywpqdnar.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3yuplkqcc.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt3fnkqtygt.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3sksjjmxu.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3ynjigpds.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3wzwrrwsf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3utloizar.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3xzbbyzil.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3owcltrag.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3tpcwlvvm.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3siyimvhb.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3atjuamrg.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3qocyrgsx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3ysgujrrh.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3asrhdgyb.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3vsffmqbr.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3mbjundfp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3rmqeywyi.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3zkhazdkc.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3pniasqtg.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3jhhallpv.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3vogvefpy.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3jdjjnnar.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3aaszihme.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3ttabggqg.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt3nbjxfttc.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3fdxsvjww.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3mxjguxzq.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kfvadrnb.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dmkqajch.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3ivfslbwx.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3sgdqjupc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3rpcjpntz.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3uwnzdsdw.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3gjevkxix.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3xiicnkmo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3jrwgntay.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mfeikszh.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3cpolqetb.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3rgvawuwb.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fdqhgkci.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3shkeebbp.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3etddvkwb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt3fmqhfeom.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gydsveoq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jpwnihuz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3lahitrnr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3pfdvafcs.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3ywryrrio.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3pzccmqbz.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xaxxvcfj.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3rtdccxtn.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3klcrbfvc.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3xxtbvjdq.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3hxpsigwz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3ltvcjfoi.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3mjlfnkvn.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt3dbvssytj.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3chmydpdx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3jxbbypsw.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ytdrembk.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3xvsqyocx.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3orqzlako.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3awywmfvh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3ubrinbkm.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3sqlnmzwi.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tgbgnmtf.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3htnfxquo.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt3mstdccei.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3awzthdes.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3qrbdaybd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cpwcmdpg.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xpidpppt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3inwycmqk.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3asmyoier.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3gjftuicf.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3nlcwkgji.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3rbueviyl.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3nlbnymif.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt3djyhjwbh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt3qjritbvl.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3nrpaqgkt.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3gspxvlxx.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3mysegman.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3llkvctiv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3nxsfbwfs.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3tksdddhe.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3wwwbfifj.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3yrutsuen.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3lawhxhfr.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ldukfsyv.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ckcxlkkv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3klhueiei.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3ehcessze.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3cixstmve.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3rvwbybdf.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3wcxfwkfg.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3kfkeoszf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3sjqeufjv.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3sbyrvoeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vergpxgf.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3spvmvbic.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qzwstfjk.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3mhapggtb.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3pzmwbfna.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tpgnifls.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ookyazla.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3vyznzpjw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3xoojmmth.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3wnbpngbh.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3hxmatqkm.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt3sbegtgii.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt3wkskqole.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3qanopwwh.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3zsbrwuik.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3rjekdzjo.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3zrejhtkv.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3tdcupbif.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.52xcode.cn/Article/details/gt3yjcshwer.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.52xcode.cn/Article/details/gt3cffuxcdd.html

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://www.52xcode.cn/Article/details/gt3mwtqnflx.html

[O03] 加锁保护共享数据
来源：http://www.52xcode.cn/Article/details/gt3rhmrgmzc.html

Py:   with lock: shared += 1
来源：http://www.ydjk.org.cn/Article/details/gt3mevjsdaf.html

PHP:  // 用 flock() 做文件锁
来源：http://www.52xcode.cn/Article/details/gt3szfpmxje.html

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.ydjk.org.cn/Article/details/gt3lggimobv.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3kpfunnsr.html

Java: synchronized (this) { shared++; }
来源：http://www.52xcode.cn/Article/details/gt3ezxivyyd.html

Go:   mu.Lock();  defer mu.Unlock()
来源：http://www.ydjk.org.cn/Article/details/gt3acwedyaj.html


<!-- 参考信息 -->