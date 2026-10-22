代发 wailian999

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2hdbzququ.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2ewntkypv.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xrtcbgpj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ebnadltf.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2cfdjpowp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2xslhwogu.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ubssrdmc.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2qvfowiev.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uuouwbyr.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2ppqshyjl.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2vbdrhslb.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2atgewvft.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zwmtgkul.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gyajbzyd.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2jaswrgym.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2hwcqdjuy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2vqblwxye.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qalmmwvg.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2wawquids.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mqlpclvv.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2oygtxoho.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rvyamqlq.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2iyonkwvp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2mclvtecy.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2lmhynprd.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wnxurjhk.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2doqjflut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpgbqsvh.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2mgunsrvv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vrkxcdaf.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2mqdxjjxd.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2nbthwsab.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2kdonuemq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2yhezwuwl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2lbojajrk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2ylwfbuwt.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2mviovdsb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2vpshkazc.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kdlohatu.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lteurvwu.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2lpotajhy.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2rrpbkdfs.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2zarhlczr.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2yyzfqkxe.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2iwhpuvxn.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2mknodpne.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2dwrmvdkg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qchdagpd.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2jszkjexa.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2xuebxyqh.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2xjflbums.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2cvblmldl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2kmashgoy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2iqrmzyzx.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2jnykxngq.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2tmgrqfic.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2iggvygzh.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2xfnwgkih.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2bzxqitby.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lvzmjpls.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2zucgfieb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ecxdtdnz.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ovizdzjg.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2kgaxosix.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2lyuqzppu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2qmgdbxev.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yafmsjeu.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2khmpeuaz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2ixozlnok.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2mkfqjbjh.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2xoclaqqw.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ikfuiuey.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2zxpdcamx.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hfydfisb.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yqvtanjz.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oamfmvvi.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2mqdmbvqz.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vujpeage.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2czifpmai.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ywlifooy.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2lbcvxdgp.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2mzhdywfz.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrfehyd.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2ljqyccgt.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gocmhyfz.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2yxzbkddb.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2kbnlvbvn.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2ejthfiov.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2zhmujxrk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2zqseoolw.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2sohlhvwx.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2bwidmlxc.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2xobegexp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2gyvmasfc.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2hztngvbp.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2mtmxpini.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2cncbsque.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bxvpagpx.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2bxtsmycs.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2othuupsy.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2indkxvak.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2atmfljfx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fladzagv.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2hmjykich.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2knqpcrmu.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2yjodsrtf.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vjwncdex.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2sajnnmei.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rogltnoe.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2ammdxspz.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2kpbznfal.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vtoqzlcg.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2kfnkeonl.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2glgkrwth.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ezbydvsl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2hpdjfytk.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2nevvzdzh.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2pigjvqfo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2vjfmtwbm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2kzhvpnkl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ilvwcjce.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2wfqhnbtf.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dhssbwaz.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2aosoozpr.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2itvhibki.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2qokeypwz.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nkwhploq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nubimivw.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hwazuuww.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2wsckwdfl.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2zevbpsfj.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bymncaoh.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ixtphplx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2nhzqxqbw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2cvpqfgtl.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2xufqanql.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gfolusgc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2pesddcus.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2oqsvgwvb.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2olgqrjtp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2usrumuwk.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2sokdiqoy.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2btceprps.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2prjldixd.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2lsitdlhx.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bbyytgsd.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlribuch.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2afsacktb.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2quwasuka.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2llooyjbh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2ntsrmmxp.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2rmmpdtjt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2hgkdoxrx.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xfggfpks.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2pwlbtgpi.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2pwebtwks.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2qhmqtdaw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2qfnxjvxb.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2agutxxyj.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2njxakbdv.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2zgifctxz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2vmemoyyj.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2utkeswhz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2aghwiwxb.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2qegjldua.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2wojqpsix.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2sqkmxpdl.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2iixrzsgo.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2nelmirns.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2lkpllpvh.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2mrrwqtur.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2nczokrmi.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ephyzqze.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2onftvmra.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2lpkfekzy.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2uihtyqml.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2ahjxzmjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldeaarwr.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2cvahvnjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rabohkts.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2jlpevzsf.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wwjzqysm.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2kviusild.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qfrifrar.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hkxzkofq.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2wuhqilge.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ykynguvo.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2auqpyhhp.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2jluuyzrx.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2acounvnt.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2xvengvzj.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ognkhnea.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2leztavrj.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2odhbwocf.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2ytjxsqjx.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2nzicbjnl.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2udhqfpck.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2ipppvlwh.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2oacsycvp.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2xavgfgfd.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2fzvfskza.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2qxzcygbw.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2pipatobn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2dzwhbajm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2ypxkkrgr.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2baexydlj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2wsskcosg.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2rqjcijsp.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjoklgp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ylizcomw.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wxsxshdj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2jyxvhkat.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2zuvdebxy.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2hophkqbg.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oxqxbpwk.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kvorufyh.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2skgtzbcu.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2itupsusd.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2cfynrbvt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2frytpfay.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zzxtmtcg.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2czezddly.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2iqqeudsq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2puordcbp.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2drpenbrr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xaubbzdp.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2udcjrcbi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2kjidnvzf.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2xcpdacig.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ugshynfi.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2ylghsaio.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2tbhyemst.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eozpogns.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ggwmeelj.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2xjkpltua.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dmokulye.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2pqxbqgmk.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2gneyyjqk.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wdjmulfd.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lxfiopdp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2pgxwjsog.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2mbjijuxx.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2henolmwr.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2frltvhqh.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lzbsfrjy.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2mnsqlycm.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2fskiaydl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2oofcrnjb.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2kkiermwo.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2lhvqoxot.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2guliteue.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2jmzweupy.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2xshnfngs.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2lvfwbbay.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2hdyoiaxm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2jarzhhoe.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2sodvtict.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2gxvgbcll.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2ofxbvxqb.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2mdzcdhfp.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2agzahwya.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2dowdrspt.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2patyfjjs.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2quegaqxk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2uftlplof.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bxavsluq.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2odlsmxck.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2xuehmnwj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2eblqilgy.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhuvttft.html

[N11] 二叉树中序遍历
来源：http://www.ydjk.org.cn/Article/details/gt2vlwofvqs.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2fbcpelzz.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2tuzegspc.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2tdiwobzk.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2aoeiqxpa.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2fhihnnpe.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ukhrrfvh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2evaantfs.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2tmsasthk.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2dkwnsiiw.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2arhdktlg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2mkvczrav.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2gqyyuceo.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2mnhmxrti.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2qjojukge.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt2utjavaqv.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2wvvhotwq.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2vyrzcncn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvplcrtl.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2quolgudo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sbnhxdmq.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2ooftzjpa.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2jjiupvji.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2wmixcvol.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.52xcode.cn/Article/details/gt2kyzzwtal.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2yfrwisqq.html

Java: new Thread(() -> f()).start()
来源：http://www.52xcode.cn/Article/details/gt2bjknoqwg.html

Go:   go f()
来源：http://www.ydjk.org.cn/Article/details/gt2doaqbhre.html

Ruby: Thread.new { f }
来源：http://www.ydjk.org.cn/Article/details/gt2vgxorpcn.html

C#:   Task.Run(() => F());
来源：http://www.52xcode.cn/Article/details/gt2miagxcfj.html


<!-- 参考信息 -->