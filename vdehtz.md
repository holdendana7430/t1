代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ujqrrsbh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3eljmqzpk.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3zwuiyrwo.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3seuaudwc.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3bipwpxwq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3fgavwpvm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3aydiqwrw.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3fijarnsh.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3blbcezgg.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3eegwqbth.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3aqklijhi.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ghslezrr.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3haicfqir.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3sndbvylg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3yryirhml.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3umpseijb.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3iymntwcj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3trvkgzmf.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3kieuaqxe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ionelkhh.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3yutnvyyd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vaeqvkyi.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3secplmzz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt3dnrihpuo.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3wkgbbumr.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3xftanhqa.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3kpqfxalo.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3vqmfagqp.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3tmjygtsg.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3qyxgwpsq.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rdnycuug.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pvlvnqga.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3uazmdvyw.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3ygtxnqiv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uegbdjoo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3pjxizksy.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3dthpnxgg.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ichgbqjk.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3ulgqntrt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3jnjvckrd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3fylylcez.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3vnllxvvk.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3mrycdolk.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3bxlmhdto.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3jfazzugw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mcyxiyke.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3vcjedmhw.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3nrowosvh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3lbzaiecd.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3xhecnnzy.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3bywvpubm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3ipdtumys.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3bdflqnqy.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3ijsojejv.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3gbvasdbm.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3zrkdquji.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt3rxlshzqz.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3mftsvdxq.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3khnabbwf.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lmziyqvn.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3quekesmz.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3trsquher.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3mekwfbbl.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3zdplvysx.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3uxnwgxnb.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3buyvkpcj.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gjpenrwy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3whhdrlnd.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3jongtsqn.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fsvgffwz.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ssuntiaz.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3zuamvxhq.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3mckykybh.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3uvuytxhy.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3rvqjkrnl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3xgaxcdqq.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qmqogmlw.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3mhcpjkzf.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3oruoklgb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ffvvgsxi.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3mbjuvptn.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3amkfbhla.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3jfiffrmi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3nguriofm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3nurmwjbj.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3ruqkqjop.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mascxbvs.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3wrobjuil.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3vopxizyn.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3qhsuempa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3bswokrkv.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3viinejdl.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3uqqaqumr.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt3pkzohxid.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yylmewtz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3zdrwhsxf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rgekckak.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qxpejnfk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3pymyhktc.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3ukzjcfyb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3givqcsri.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3afklybyx.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3duuwgvko.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3brnyklom.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lbjvglvs.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3jruyvooz.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3uyjyviau.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3trrotyoj.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zjnbbnnu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3rmdmadjm.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3apwqizie.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3gkoizccy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3aapbumvy.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3wkzhhspp.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3hliliqxg.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3txzmsjyi.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3dbjtjnlq.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3xjrgomph.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3zbaridmv.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ovtikzdy.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3vwmqsors.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3momkmxov.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3vhyzirsl.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3pgiycxsc.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gqdrvqee.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3pkvducvk.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3lfoudcwa.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3blxwzqll.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dpjivzsf.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3xgtyubyv.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt3bzreripn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3tngtrnya.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3urfftyga.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3yeqfxyab.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3zbqcoqga.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3zhllgfye.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgojsvj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3rvptjput.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3edudhhfy.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3iyatyihy.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3fjethbst.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3heesxvsf.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3mswvfxvf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3ezhafjnk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pqrdswsw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3syupqhok.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3tnothgpz.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3emnuzjsa.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3zrjmjbcd.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3bmapueqo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xtfpxkuy.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3fmbeqtjq.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3gnbwnxsp.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3uornjsim.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xfaenwug.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3xknixhvg.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3gftrkruf.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3nmgwkbgh.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3lbfeillt.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3kvbwdmyw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3iaqnwbnf.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3kuhjpzvu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3bfjaxvvd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3wvvdlmys.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3ggxaptbv.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3zshferqu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fhyxwlga.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3jdcoczvo.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3jqqzunic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jwgugimz.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3cixjells.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qymtfhuc.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3gzoiwlcs.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3woggejhu.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3foodnaug.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3zvjyamsd.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3kzqynsar.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3uocgwvbx.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3mlmciqzt.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3pucocgxx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qxhdhjpc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt3ncqcrdco.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3fzwpbntz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3iaurwsfh.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3yjjdjwbj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3taizsphy.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3gxwcdwzj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt3vgfpvzhk.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3oabyezap.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt3opnefojr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3dyhqclqm.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3ezlgxvtv.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3grjevehs.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3jjsjszpf.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3gypsmbbl.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt3ribwpvgh.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt3civwqjey.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt3cpanptlx.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt3cfedrgwd.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt3nuamrhea.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3yhctynfg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3bxailqeg.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3lpamshzo.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3jhfardzx.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3kkjbudbe.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3varatvky.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ppbfcqrv.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3vfomdvga.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3fikalcwj.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3rqtvvgvg.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fulibuqm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3pbgtvlpb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3uubcjxgw.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt3uhtboyth.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3uiewqmpx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3yucfogvx.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3xeviubif.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3lbfklalh.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3hbwcjcii.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hmuzxpgc.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zjkewens.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bachvhne.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3mybknpaz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3egpkxuzj.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qsymgfrl.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3jyiimvip.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3myjsuhjf.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3vjceoufm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3iljrbpgm.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt3ljdlcfow.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3chkxcyoc.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3oydedufy.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt3xnninszg.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3uhwdfwuk.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3ctrpnfyx.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3vknkevrl.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3okanguuw.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3mywtpqlv.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3kmhjsqou.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3ngcjvvib.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hadmuuey.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3msbvvfmp.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3cixodnfo.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3blbdpnqw.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3vjneeszf.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3wxyhbdab.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3caksdezy.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3cikcvbvn.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3rssbguez.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt3rzxftvld.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3gnjovjth.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3cqyrfglb.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt3pzxdeooy.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt3ltjgrnnv.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3fnacnzqf.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3hkirknlv.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt3nqwmqoee.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3mdpiyocf.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zeztcwqp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3uhlakzmi.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ygtagxhn.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt3mzvpoqfc.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3sbwpnhev.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3yibalace.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt3smjgkklj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3wqpbhxjb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3xnswgvli.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3bgutxige.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3wqlkqcjn.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3jrqgngkz.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qbujyabm.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3gcbkblya.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3ghozxpaf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt3oyapsbfg.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3thsfwnze.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3neitecoz.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3wwestqtc.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3qscyvvwl.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3gezrduhe.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yerbpoad.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pdxyzmly.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3wqvpvnyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3abgtvhlb.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3tnrmjcme.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3nudwnovt.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3tjfxohvj.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt3ywerzkxk.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt3edrlbhvj.html

Java: new Thread(() -> f()).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ujwnwflc.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt3bgcmcyav.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt3itmstsje.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt3rgkpwcbx.html

[O02] 使用线程池
来源：http://www.52xcode.cn/Article/details/gt3avcqwgcu.html

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.52xcode.cn/Article/details/gt3pfrldlkb.html

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://www.52xcode.cn/Article/details/gt3gcmliljg.html

JS:   // worker_threads 线程池
来源：http://www.ydjk.org.cn/Article/details/gt3bnjtenql.html

TS:   // worker_threads 线程池
来源：http://www.52xcode.cn/Article/details/gt3uirrkhvp.html

Java: Executors.newFixedThreadPool(4)
来源：http://www.52xcode.cn/Article/details/gt3vkolmkro.html

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.ydjk.org.cn/Article/details/gt3upocixem.html

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://www.ydjk.org.cn/Article/details/gt3mqpgjqzg.html


<!-- 参考信息 -->