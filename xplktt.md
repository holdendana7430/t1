代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2hctcpcfg.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2qieabdtp.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2kwegtftt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2uprkusin.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2dgugclhq.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2izkpujrz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2butkraca.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ymvqjufv.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cvwttguy.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2synmdlzq.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2yiqaoojy.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2wfnprhyj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2svfzbhiv.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xgdwoyti.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2lcmnwgwi.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2wgnngrlb.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2gpwjztcb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2exgetfwk.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bxxknosi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2betukqcu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2ftauhgbv.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2skvuyjmz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2gpvpjeat.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2rveihgug.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2inawrxqm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2qlviuvmz.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xwxbcmiz.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2knfjiohf.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2iiyjmyps.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2nuvcpebg.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2bqfujhbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pjfzwhww.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2aeermyma.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fpmvilfh.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rxuejztf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2bptdxnya.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2zyueibnq.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2jcjduwgl.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2dmktipld.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2lewqklha.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2duqvqxzn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2treacdzy.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2pxlfvkgg.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xdlpkdke.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2lbsbfdcb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ieffsjfl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2qfowkqql.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2unxklpee.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jqyxroea.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2xfkcjzca.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ojuzifyz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2mqzlsewj.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2lnuendkx.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2eytpefzc.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2rtyfhmjx.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ljcygotc.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2fisxqfgu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2megqvoyc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2kxwydjmg.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2ukyzfbfa.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2wohkoevm.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2mbmnbead.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2xqioeyzh.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2vbtcexpb.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2jygnpxlr.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dwzvunbw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2pcsqiocx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2xbpthszh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2fajlgbww.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2kgfxquio.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2uowggjas.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2gkqsbgrm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wotxytzq.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wyawyiwb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2brckcwxs.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2kzqzxbat.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2scszmits.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2hcijjdut.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nkrfptat.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2vcntfewt.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ghlmkwia.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2mwqkdfnk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ruexmaxz.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2hqsrwjza.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2vwzfopnc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2wfrfdsqo.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2itgvarxq.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2jpkzsqke.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tzsipmru.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2axkcbbuc.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2autqosev.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2aupbqsqj.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2tnitnfmw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2nlgijkdb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vqmhejgx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zzxomtzs.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2pekzacxn.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2ojryjzhm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2folykfrm.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2bliqmsjw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2zwiwaguj.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2dgenabdf.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2sfiqimde.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2lgnzpggd.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2zuoxurjj.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2weouymuu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2irugprwh.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2osuwrnzv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uoszuyew.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpddtmqx.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2xhivfggu.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2tiyxjxmw.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2jbwfskhd.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2hmumspce.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2hofjjzvo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sxrssddl.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2bbeecozl.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2xwrjciph.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2rmvfxajc.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2meqligap.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2epzlcjzx.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2antijezm.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2ayzdtrwb.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2veynfjgc.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aseclxdw.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2ucdtzfzs.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2ialggann.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2zcvhgrga.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2uqnacovz.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2rkvpsvai.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2amgifhjd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ybvcxhja.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2ojpdjhmp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2neoashjn.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2pudvejsp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dtrutzld.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2qdmwlalq.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2vviunojo.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2trymyufy.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2nzonblab.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2cmpusqno.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2rnsqahwr.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2qkjxqzom.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2ygblwcrw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2spmzcgyt.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2lrcvwxjw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pdelqxnb.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2rgojolds.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2bhhmnufq.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ibdddunw.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lbgtwjsh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qyrjufwj.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2zxsyllgz.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2xapvrduo.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2noyxutcl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2ffgpfqpc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2lzogkdev.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2jnfveiyn.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ntkorkht.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2utaifkzu.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2mhdyftcb.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2pvpixrhk.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2tuaujbus.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2qxvlilik.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2tkmbluqz.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2goxzjoss.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ptlnsgvr.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2ffortfoz.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2jdhzabed.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2bbgmevdp.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2jjmzjzpo.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2aefcdrqs.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2ohbegrei.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2msnjbkse.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2kmylkjdm.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2zgbujncx.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2fzcudlux.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2thupbxla.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2gcvummya.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2whiakdtr.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2tflqthgk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xqhynqhi.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wapabjxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kajlrppw.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2briezkdk.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tixfxqqo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jppwmskr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hhmfqwuv.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2uzwxqkhr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dtbbzmkb.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2phldjlmw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2xvgybjvv.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2hjskthxi.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ggxbteek.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2uxxubxsf.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2bxlitgqv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vgsasorc.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2velvmnib.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2mhcqtgzk.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rrztvtbc.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2gccsbghc.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2fzeqgwuu.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2nlybtmxy.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2crntqffa.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2vgkpibwa.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nbjziooy.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2qyxmumdm.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wbsmidng.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2djzqjajs.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2eqhdhaxp.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2cxvohfae.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xvsjhnnr.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ckciktgg.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2wdtnofpm.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2aiiqonpj.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2vzoqdrvd.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ayfdxgto.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2hhdkgoqw.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2oerjsusj.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2lnxcuuvu.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt2dcecwsxl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zdtqhzjt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2frsljhsd.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2mlvjkloj.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndmozolu.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ohwmfyjg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2fubhdbhr.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2tonpjvth.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2mwtzpxyr.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aqatdmqz.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2effymczw.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2efmvecpw.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lvmwjgbt.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yflyljsj.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2qpspikiu.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2ovfavswn.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lgqizcwi.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2annawjhm.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2wppocwxb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2rwmrcrdw.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2cexxoeif.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2dhxxgrxr.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2wagerkjb.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2fkuoyiof.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2tzajhpvs.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2gnaxzztc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2ddtmrwuu.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2glblkjfb.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2xvfdljpa.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2qfgpqwqa.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2vlsslnrx.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2loxddekq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2assawzts.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2zahqospu.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2wexaozmc.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2aquwqyxb.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2dgajxghu.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2vtbzcrou.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2owmkxwhz.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nqfoqyti.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.52xcode.cn/Article/details/gt2pgnxdqrm.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2odiomyua.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2efurrnbo.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2ucerepid.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2vazxirel.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2appkdgke.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2rrtovuop.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfstdusd.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.52xcode.cn/Article/details/gt2buecdtwh.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2bvhcmyhj.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2cgviutjv.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2brjloowj.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2fdudzvfd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2urzusdnj.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2phfyouee.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gacclqbm.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2atpclbpz.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2taxrrgpw.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2ifffsprp.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2igcllxhk.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2owyagmqk.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2ljqmumyc.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2ptjugpet.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2khxjqriu.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2jjtlegeg.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2fbtbibhh.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2tbpdyyxb.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2dbmipopr.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2fkhfzccy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2uoxowldo.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2mvercygk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2hdktbqkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pehyjxjh.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2bhpjwjiq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qodgozfa.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2kehmhhes.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2wzucjgqp.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2kzyjxwup.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2flmouukx.html

TS:   // 同 JS
来源：http://www.ydjk.org.cn/Article/details/gt2stpwostx.html


<!-- 参考信息 -->