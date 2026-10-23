代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3xuhgcniw.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3iujzfcks.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3dcdmkfos.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fxiweyom.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3laswtutf.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3zjlanwan.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3vvniozbd.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3rohhllgj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3arnjzyvk.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3xlwyqmll.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3jzgstlwj.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3lkghhdqs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3avjbofiq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3pxtueouq.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tuaqkvca.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3rutouftf.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3qmvaohkm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3rgmoarlr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3spmnnwzv.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xcmcwter.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3avpypqmx.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3aywbuooo.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3zdfbpdzz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3iywolazu.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3pxncooeg.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3xvgozdtb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3oamrqzzr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cusibvtl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3hbujrsim.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqhuzoxz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3fhzeamic.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3mjjkhvqi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3armllnvg.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3vrxkrphu.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3nyzkqhhm.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3axzpzbza.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kpzhfbyj.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3etzkgsjw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bqklgwpu.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3izveendh.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jxngthua.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3eegwkbgx.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pqbtgmiu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3smoshsxq.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3tdewdixt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3zghheuuj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3uayquhav.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ksrzqpxg.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3brvokyvx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3pgnncyce.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3pkxhlryj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3zpbocicg.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3luhhlkfc.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3wuoucgij.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3qwrvgkmk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3yzvfkknv.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3trxelqdf.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3qiuskimz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3iduhphyc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3gpfcngsl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3htrqzwpp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3byolkqmw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3fooqxfrx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zipiozgx.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3jvlxytpo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3clsxsyii.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3ragonxxw.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zbvcaqxe.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3osymyldb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3dmvpfoed.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3iaquscrj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3ahqpeygn.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3fldpxbho.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3whmkmynw.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iiyjtnpu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3olqreowk.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3njscfhbo.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3knqslkpg.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3liomgfno.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3etnazfit.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3reajifzv.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3vcfezpaj.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt3sedybcoh.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3xnixqusl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3lcncigez.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ipheoumk.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3zsjhmhyt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3cakronhf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ohmcxbvq.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3juppeckg.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qwuvczoa.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3takkpapy.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3vacfpjhd.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3xgkrsggs.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3uuxrpzss.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mmnsghrr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3bvyclgsg.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vsuandnk.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3xbvyauoj.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3kmedcmmc.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3llhdpwad.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3nyriwkeg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fpufldez.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3yrlnuoan.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqdjtvry.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3iyaltzww.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3srtrindn.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3jrcmshhe.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3gdgpyqcz.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lohxqjvk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3xmjrhifu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3bmjxouvc.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3tiwrehzi.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hiumfpnh.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xxvqkwta.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vswrxbqj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3daoqdolt.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3zxkcfcng.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3xkufmzxl.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3xuxtindm.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vbwzrney.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3gdlpobws.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3geqekhdr.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3hmjaxxqc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3tswwznho.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hkmpmupz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jxjewama.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xlnukfnn.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3cebewspw.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3dartlsrl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3hwjdzvzi.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3dhyxuhlf.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3khltercy.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3upybiirx.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3axsnztrc.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3gomzpsap.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3akeprhwj.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xslikjym.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3cfawfmkv.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3amlkirsw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zgvfentf.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3xrftgvuf.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3btnpoboy.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3ejxtsozn.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fvfuircb.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3femmdsls.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wcwvbdkt.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zywlfvyv.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3xccwwnah.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3mvjpdewu.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3ayqppmce.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3fevqmkpd.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3grwrxxio.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3szxdonaf.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3hlncomld.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gjqbcykt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3yhelozeh.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mhvkipsn.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3sorpcttq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3sbhmqmhj.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3wtddijyn.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3xtteymef.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rosbbwuv.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3sryneqds.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3nsuavzrn.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3rtkzgyov.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3nuayewht.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3ljzphtnj.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3nbnmzuyg.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3mqnapikz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3rivmmsfo.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3yzwrbciy.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3demvyphz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3lyyspigi.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3rdqmoiij.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3iznduvhc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3rfzzdpfw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oddbkeoz.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3ztzpwhsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zqjeutsn.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt3amxhpfsv.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3iikluotc.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tlxvslyh.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3dxomzyvu.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3glzuwnze.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eminokcp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3bgdqqfea.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt3suseesuv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyavfhwl.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3nhenoeci.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3tarkfhqy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3nsofhuvh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3kkwfyqxd.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3toqqzvwx.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3xugnyzvh.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rhohzqdp.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3qfrjkveg.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3yenducib.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3lyorlxob.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt3nprjufrp.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3pcfqcgpz.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3hyupnach.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3wrrwppmi.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ecuzcsfj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3nztyytyn.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3jozfijmr.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3jcwyjmqv.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3fmljjwie.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ugskzfda.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3teffeymn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3yzffpykr.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3kwtoenyq.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3zuropoun.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3nfoisrob.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bovxzpee.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vpvuefuh.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt3umvixvdw.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pljjtqvk.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3gvavndqs.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3zvssjlkq.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3csrlnfmu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3ommgykrx.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3yvvqzcjm.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3yxpfdmzp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt3fnophaae.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3gbkhskyj.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3wgocwfid.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jfjgywvx.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kgocxkwh.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3qbpkmbcq.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt3dnrivbii.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3wnufkdcu.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bvfabybf.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kmhdfrgd.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt3drqtbmem.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt3syiedbkv.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3pkwyixav.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3bfirkzrt.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3gvhhttjv.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3mscxjuaz.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3nesvitxy.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3ztcpuxss.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3xorroqzz.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3mcpwzgof.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3rrdargfk.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3ngxodrjd.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xfitwjmt.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3lcwxikaf.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3rzxiiiws.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3xwuakhvz.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3iwsuusge.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3pvqgsacm.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3fwnmpsfy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3hojfjwlk.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3nxwyptcl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3tjkqmscz.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3fskrfrmk.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3rbbzedzi.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3uthfozcj.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3mqispjzc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3jrjyllvl.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3oolzbbyh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt3andfsdgs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3iwfsclla.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3wtebsyje.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt3zmbfchcm.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt3irqvdyxb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3aapdrdmm.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3zylijlkj.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3uwjoujhj.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yarskfyq.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3aumwyyjq.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3fhjkhere.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3aoqjylas.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3ymotbkkv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3mojevzoy.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3gewcbjbw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3hbxcaznq.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bbwerzad.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3znktldiv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3cptbragr.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3pqxvwpme.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3lusiqujo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3teswglkj.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3lbyqlqvb.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3alhpylwv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3khzwymin.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3kqghpzyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acunnbxc.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt3wxsazdet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3upxlxgkj.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3fsncllfe.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt3aflgfrkq.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3ewjpnbdj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3stgcrjia.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3gugpndfz.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3cxoeftme.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bfsewzqw.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt3dzboporu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3wvuhjbwk.html


<!-- 参考信息 -->