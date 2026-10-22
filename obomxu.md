代发 wailian999

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2lougupxg.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2ssmivkyb.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hqtsupkl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zgbfwuoe.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2tdzsyssr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2wuimalwy.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2sjrrrylv.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2xbfaxfdp.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ktywcjsd.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2ksearxam.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2entzageu.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gtqvzmnn.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2tzqpyilz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2teuqpvqr.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2yaeqzfeb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2apwfmtdr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2oddfqsqc.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2ojtyvsnv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2yegqreba.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2hpyusoob.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2tbqlorfm.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cfbzahnp.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ljjmnisv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rjrljspv.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2lzivmyvg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uvmezmbd.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rvhicwnq.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2mmncsqsd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2iusyubir.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xxywvajw.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2pizdkmpa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2fjwmmutq.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ghwatelh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2nxwldsjg.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2uimryvfc.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tlkuqlxa.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2znxxkqtn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2vzlagpzw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2ufkchfjl.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2efkjnpfz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2dkvfjzqt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wiasplgj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2vqkiybyo.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2ikjvdhpt.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2djvxpykb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2wrturvpp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oywxsmyo.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2pxhbnjgf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ljafmleu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2xewwfndo.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2kkscvlmo.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2gfgqmwfh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fqchtijk.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2zfnnijtx.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2dmvwaaoa.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2wqbdncsj.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2svhftouu.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2uhhmlrht.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2zowtnppw.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ezruoncr.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ycnitsoy.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2etpysgsa.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2gepjsthp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2vhonirsc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2cyyjcgtj.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2hnokyder.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2jrpysapd.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2lqnjucmw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xpebnnrl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2xetlkflo.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ilvliewf.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2yzpxqhwt.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2svlphbum.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2clofevnk.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2faknuptr.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2yzygcttk.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2qochsany.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2dqmixtyt.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2guzqgbeg.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2zlgercfz.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yndgqthg.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2elzrwpja.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2mpjmfage.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2szjgowhh.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zyqphcij.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2tscuczko.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2aecgxucz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2pkznzhgl.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2iisnkigo.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2tooenxnc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2xgxsobzo.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2lktfqwak.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2akfleobl.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mpjhwhjm.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2aosglmto.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ujhdhrhy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2ibqkbqje.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2kxrgsrly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ayljoqpc.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2mxjmurmj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nfnsigao.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vuxgkhsg.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2kejckmdm.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2hbrumtgk.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2wyswyunn.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2okcjlwia.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2exfmfgav.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2yopxnyxv.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dsthypyg.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ujascxvr.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2jcftymvb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2vjqsctxc.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2yilyvffa.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2mkjrmnab.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2rmbqwdxo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jadcyuqu.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ymlrvgya.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2odsnzerw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hseavwrw.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2uildsyrn.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2szkwdcca.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2aoifblua.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ljijslhn.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2dovabwbi.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2mjuizikp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2kiysrgzp.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2yfimzlsd.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2lryvwyzm.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2wgncjwvp.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iueubhhf.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2wpsuayek.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rzocewxk.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bhllmgyn.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2vupeeolm.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hbslurfh.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2hjxlzcon.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2etjbyzqq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2pmtidgcs.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2qaiknbqm.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2hfwxwfpp.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rkrsyphq.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpzbbxkc.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2dalmqugu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2helddsxp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2qckkvkkh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2akxjzeou.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2tovfuiro.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2ivkggttr.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2twxlqfel.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ehzryenc.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ygkiuooh.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2hyssmxcb.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ykdupmym.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2spsfzouj.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2bjgbybul.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2mfakricd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2oarpznbs.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2byzabdsn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2zmwwgbdn.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2iimaeeuz.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2aermaduj.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wjcgtttc.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2thyyejcv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ydfrxnut.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2lqqxxfgh.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2rodpgwrw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2leahypau.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2mhyyodrs.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2yfjloifo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2jbapupsw.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2nqoezaem.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2inbioerg.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ixpyvxrv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rmjwqzsa.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2ejepocto.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2syqpabyj.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2fdnydgfz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2lpzxhlyo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2osataxwy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rusdwweh.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hqvezhwl.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wthenlxi.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2kilzvvnl.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2mdimbney.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2nxqtxpxz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2skzqultt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wdncittp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2cfozruhm.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2zarengkn.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2guugnqph.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2gfbpwqhx.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vuxxluhq.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2exsbfdww.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2upopayja.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2squmllvi.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2tkystowa.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2xrkuenlx.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qcyluymk.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2tfollikf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2stozusmi.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2kgqoavne.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2hhowdyrs.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yrbpgtbc.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2ugiqtosl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2degswevw.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2hzjfaeoc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2bkxamvuo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2hyiifewj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2rqgvhaig.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2xxjpknwq.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2cfjukava.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2rlrtzvog.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2qinwrvut.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2syyfnxxp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2jzqujfmz.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2vphrenjx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2gqkztfdp.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2cddwqqzk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2oewoofvq.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2cfcpokyh.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ehgnzjjd.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xzrwttdz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ulariafv.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kvouztpu.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jbxuzopq.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2caynkkcv.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2hweczoft.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2zhmchfcy.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2juwqrsqu.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qeykqwnn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hftrxbpx.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2pxogivkw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2txucjsqs.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2irmqdzbe.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2fnrnewxo.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2alxdskrx.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2ndnmqtky.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2ohgsvlgm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2xkxksxdy.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2patutzap.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2sddgupaq.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2sdhqrltu.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2qbcyimkr.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jntyjumr.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ossxcznh.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bcscvzoo.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2iobiemdy.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2onsqqxbj.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2owrwduei.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kxknbgwn.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pfaqjnze.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mkpeings.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2ttgtwxmh.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2cmlqolxu.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2lmgjxmid.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nmgdhcsk.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2saakkzbk.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2hujwyxhh.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2bungjauy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2okdcbciy.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vlgtxmxk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2pudoyyxn.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qlsnmvmg.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2ebujaehd.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2cfihwzut.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2kvwiqnlk.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2gyafxjks.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2stphelki.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2ezslydan.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2dcqncayu.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2tbnuemnz.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wtrkavzm.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2bltcsozt.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2qsxcbgyv.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ixdrvmao.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2eeopnwha.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2odvxnusd.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2nboqfimt.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2arbdsynm.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2yqrgwosa.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2xrvrrbyk.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2vctyabaa.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2hsmhnfkn.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2vglivoml.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftjogovi.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2wtenucjr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zolylwbj.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2nodpolct.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2qhjwuulc.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2iavmgjnm.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2defywvse.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2qakpyccw.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt2ypbkxchv.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2edrnswii.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2glvsejmr.html

C#:   Task.Run(() => F());
来源：http://www.ydjk.org.cn/Article/details/gt2lehwodra.html

[O02] 使用线程池
来源：http://www.ydjk.org.cn/Article/details/gt2xezhuxkn.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.ydjk.org.cn/Article/details/gt2nhiaivvm.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt2ovagpxga.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt2tccrqwze.html


<!-- 参考信息 -->