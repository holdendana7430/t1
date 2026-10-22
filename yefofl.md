代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2bqwdsexs.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2porsqroi.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2eszdmudc.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2gldtwkcx.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2hhawbzmj.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2pizuyhlt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lkwcqrkn.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wdhfswkg.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2mvrjbxyr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2kkhsjwks.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2nnkykppl.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2ucsxvejf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2iuqlfrci.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mxjgvcbl.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2fraiubxm.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2ejgzlsix.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2alcofjts.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wzsewawc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pccgtiuk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mgrxommm.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2euvacdbs.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2risguldw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2awcwjvjx.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2popnbcrs.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2mifqmcfi.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ygcioltb.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2zidbobqi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nnmhqzok.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2lurgycmj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qnhxniah.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2flnvcqgr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2wsmingbe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2trryawhm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2axfwdnjs.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2wvpvfitf.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cgoaqwwh.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2lfzbvfkz.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ajccdplk.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2utbnrgpn.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2aefvflmn.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2uplvvvyl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2zxwvpjxk.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2vdgetpqt.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2trqmpwlv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2jafudjov.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2uvrxegbm.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jgpaibnl.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2cxcoovcz.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2knykxosx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ihruyhei.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ytucbmvl.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2lahyfbhz.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2xjdynkak.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2yoitomes.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wrhqphmu.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ekzewlip.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2janlmrdz.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2tqcbhmwz.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2rpviljzz.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2dsmwfiir.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ietmdgan.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zzruzjbl.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2rlnjkilt.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2bojljdpa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2yubbctjp.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fypbcfjp.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2rbgunfdg.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2adbxhdbr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ugpidwxk.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2letwpspn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2kcjkehqq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2afwqnxpg.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2adsjopms.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2uukardwg.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mizvmttg.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2fxrmxpah.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2xzhukbci.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qudwnbdt.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2nklkvfmm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2bzqxqzsm.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2repailwj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2aslncfnq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2ctfkebtv.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2olunzwqa.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jyrzhdwr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2yfpbxzsu.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nnjwgfgt.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2lqaddbze.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2doilmstd.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2hcnsyzjv.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kmybcevz.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2unihigkc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xaprmtie.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2eaxodxgt.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2xbzmuybn.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ovoxyufw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2oliajtts.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ecdygvlj.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2irkbqjcl.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2pdxvsnnt.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hriksmwt.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2sqvvzpfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dvhmwggf.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cdegqvyu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nhexwmwd.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2feznjvie.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2husgkmdv.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bimhdvvj.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2csqeqveq.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2yyxxchci.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2bqnbbmsr.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2zneboisi.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ybztrspt.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2snxuxyko.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2evyodhit.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sabepsti.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2rohsbill.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2qjomggyg.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2raicruqj.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2pyffdnkl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zizgwafc.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2vyppucaq.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cqanntda.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2qpiecker.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2yzppzsnv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2bfdzkgom.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2lnksjfda.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2jxnurqze.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dnapdvll.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2fhpzhiqh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2ctlrcars.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2qmbbrcbs.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2hfopbxgs.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vohydnlh.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2rjveufdy.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2vkyryfps.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2haabmwqc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2nrqgxjog.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2xlmaftmi.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2lckkitvy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2dqrdzfok.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2lsoosldg.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2siwglagk.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2aztuflak.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2txdsxgex.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2tfeoxdma.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vhlvztgz.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2slrkfkgl.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2xoppicho.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2wycazrqt.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2vivdrtts.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2rvmliuil.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ichoqyps.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2jlrmjrgf.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pibsygeq.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cooughll.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2llerucnz.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2kxczzrsb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2fjvroyhs.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2gsouybgo.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2azutmjgc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2ojmxywlx.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2hixvpldl.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2kwmzyvik.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2dukshegh.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2nralxfug.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2rijpccvk.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2svpzuevw.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ilhbulbo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wktdrodk.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2ynratymd.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kysmxdji.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2sdaclyip.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2zmftrygx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2qxxocsfj.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2cwyfxkcx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2cdwkhzcf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dappyxnd.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wrstluph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gnhramav.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2qxfkvoty.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2gcwkpslx.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2yezwohdz.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2vkfmqtvb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uvuurvub.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2asshddea.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2tbidfrzb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2yeivzoni.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2bzunzwvu.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2ntvkpoel.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2grmciobz.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2sxmdhzel.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2owjlrjti.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2cppiauus.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2kogtcfcj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2upvskwqn.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2uxcccoiq.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2iolvvkrl.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2pykwtdsx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2kqwptvnm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2rfmeubza.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2grfyshcn.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2ufdpnfpu.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2fcpxlvmt.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2xoyryzjt.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gztlsnmh.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hniapucp.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2cfrkjrqx.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2cyoeehvz.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2apbletfn.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2zonahbyq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2gwypssub.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2nlymlzfz.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2mbmjuvxb.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2lxoxnkxm.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2jikqlpmf.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2cxqlutwf.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ngmepfvm.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qnppxxyq.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2tqedgpcc.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2awdlnrqy.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2yllxrkmv.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2mdezonbp.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tyscmyib.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2ncapzadi.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ziysthrs.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2gnmympxh.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rwtdsvak.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pyxewtmm.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qyfdamlw.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ezudiwqf.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2zsbnjxnb.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lajrepmd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2strquqwd.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2zaxhlktr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2bwhfizah.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2izjgrjbn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2vgyxwqdm.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2hwfsxrqb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2bqaomcym.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2njgrhmqk.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2vuktpqqm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2eqdfxznb.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fskwbbnb.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aytgizhg.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qqyubsrp.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2uynfwnpi.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vhvwpftd.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2keeeqblt.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nzpctehr.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2utmtkffw.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2snqvwhoh.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2accclyms.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2pejgvfij.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2qkkrngww.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pndivfnr.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2gsmrfjll.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2redhiqbb.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2jcahfxco.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2cuycbbqa.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2lewgcbyp.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2frliwfnu.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2ehmpenjc.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2iweamsgr.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2ifkfnrih.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2lpdzksck.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqlfddzp.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2pgcverwh.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2vuoyxetk.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2sgbmcong.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2ajnckshd.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2rcgnwfuz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2jbbhsssa.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2beiuktck.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2uioomaaw.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ssznesvg.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2fmjvryxw.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2aoomhzpi.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2afkbjlbz.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2sbijevtq.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2jismvqzf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2rscdprhy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2vqsxmaju.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2uxpvszqe.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2butmpnde.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2btcvobbj.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2kqgiuxiz.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2rtmoxrrx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hrasfheh.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2omkpwnru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agdfebzm.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2cpojjmxc.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2nuswoqzl.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kygjgqpq.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2lyuugyuj.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2aymkqwrb.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2mnoydgcw.html

Go:   go f()
来源：http://www.52xcode.cn/Article/details/gt2idlixulr.html

Ruby: Thread.new { f }
来源：http://www.52xcode.cn/Article/details/gt2axkzmwpu.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2fdcjwzbk.html


<!-- 参考信息 -->