代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2etfggekk.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2vafdbrqz.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2bdxbanjn.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2hppqxtpu.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2nzbkkbnc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2dwppmoue.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2mnnzehwe.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ctxnyqzq.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2amqrneep.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bdepqrke.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ljkrtvay.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hxkblpcr.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2hzmpkgjr.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2xkfoirkt.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2gztlgcsx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2sduzjhvx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2yhedsnjw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2smcjejck.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xdtbckxx.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2qqkptomm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2yfzenoia.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zcpbwdiq.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2ftdldldp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2nvlukqxt.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2icffbgqk.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2eqllwyqk.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2rrfcpamo.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2ddyrzqms.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2habmvmox.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2ulyyijjl.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2gvbftrqh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owrsxdio.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2kaegnfsb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glvpvlmu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2zjgojlvs.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dmeiotic.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2uucxvpmx.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ziadnlaj.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2xhnwejeh.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2qhqsylqo.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2qlsljgwr.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2bimwyffw.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2bosfysvd.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rfbdukcz.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2brmvpmuv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2xuxllkbw.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2takerhtp.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2kpioemif.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2bjkbpbau.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2ekvbrkob.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bntsyvcr.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lojaxetn.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2lbicwnfq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2ubshlkpf.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ugthkuum.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2skgpkmeq.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2jflwwfjr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2yfjjwzqw.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2xduvpdzr.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2qkdepkor.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2djmlsrkr.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2hwxegets.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2hqtewvcf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2kzvntufg.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hssbmrtm.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2meefpltr.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2zkdeokjy.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2ymeiulbw.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iybpcrst.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2okhzzuzy.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2yajbalfh.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2htjnarhi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2aephmqvu.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2duahlhcb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2ioibsswp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2ydjkxivi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2dutzfnxp.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2xsxmqwml.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qzcyuctf.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2saqsyaho.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2imametrk.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2timwfnnx.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2obwqqqhd.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2doyjpwkh.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wpmdsfis.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2rztqjvdi.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2xbfvkigc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2unvdzeii.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2btvfyrhs.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2kkbnlumi.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2vwiramcd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2wtudwwih.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hdwfzlzg.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2otufvezx.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2dutcjthp.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2fycwljbq.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2jitrmgvc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2hnqelmxm.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2rpajdgnm.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2vimdrlhr.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jfwofbkm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jtzkavii.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2klxcdyag.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2dpjbmupq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2gfqlbjas.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2bwtpzrci.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xmvribpw.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2cljvfldw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2umwyqoff.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2vzxpoxyv.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2yowxagam.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2xuvrgxkb.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ktrgbzfr.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2rakcbcce.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mgkymqlo.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vdkehcmz.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2tttjlfjk.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2ihpagoor.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vvvzpdzb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2sadlceoa.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2sgpneckd.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jlkztebr.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2wovyclci.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2dafyeyyf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2podhlaph.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2iemdhyue.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2aduvkvza.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2eauzkavj.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2ewahbkot.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2hhnulgms.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ysxeqfhz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tshrkmrk.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2ormwbyaf.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2xcdxxuom.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2zqkunrce.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2dpfmmqxz.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2lxbvzkif.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2uzoyabxn.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2vawscyua.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2blanmfrd.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ycqbvhbc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2uwyidqpd.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2phsfbdov.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2bwpisrsp.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2tyxwrtxi.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2eanbioqk.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qhzohiqe.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2giqopmfc.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gcfsteco.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xhivhdbr.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2udttxxtv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlthcymk.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2otwficay.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2nopsfwbg.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2gzawauop.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2wkvmtakc.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ifbqihsf.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2osegsrpe.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2gwrjbcgj.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vehazxoj.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2eoyrjotw.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2lnlssmyy.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2sqiqedzb.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2ailmzjln.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2rjbtvmue.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2nklxmzhz.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2zzkqykhz.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2twpkjcsl.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2nbzuzsbv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt2exresvkd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tsiatidx.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2xjnoexrd.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2tamhixyw.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2wkuemfze.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2lihrtdna.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2cudchfgn.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2phcmruzd.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ywawgbrb.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2egmpkujm.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2mdcsoplc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2phwbixfn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jkukkeot.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2wurumhwr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrvdksqg.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ejwycnfr.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rvcsqhks.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2dvvinjkg.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2hkpuxzpy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2qtnjwbck.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lioaqbmu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2woorafuc.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2twbkppoj.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2uaztvmqq.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2nufafhjy.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2wdkhrqeh.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2ayulqovz.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2vxqbetbq.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2qmrpyebr.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2apsrpixv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2spoygere.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2hsjewvvd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2tixxwcgb.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2nzewqxvr.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2ohbmchbp.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2bcijosul.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iqzclxrc.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2lyhhankt.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2jzdbugwj.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2drkowlhk.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2wdmpagbf.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2yfqlylyl.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2znvnbvtl.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2kxvfmfco.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2entfnaqc.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kjnnricz.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2uvrzjitf.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2xrtddktl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2tthyhxgd.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2ttvngpri.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xzftujkw.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zbjcqayo.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vgemqedh.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxqldomt.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jiwshfcx.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2xtbwkgme.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2ahehovdj.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2dtrcdrxp.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2vmgbvdwt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2ulnorjer.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rerzspgg.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2awzrytgu.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rpyueurb.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ordxvzqe.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yxvhufix.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2evtdubyu.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2tbqqyrpb.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vdkzecwe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hmcxjfcp.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2kzlnrxyy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xlmkwotq.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2dsdkocvp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2qfotojru.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2nyzjoyeo.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2jfhfbbyh.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2ytagtxmi.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2xphdprkc.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2cbnetoad.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2fcvqzbeq.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2slsibfyy.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2gswtjtku.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ngmjxsgu.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2hfbujkqi.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2nikvbdqi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2povdguvd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2pyiveyik.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2dowujzua.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2tmmrmahz.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2kkaycamz.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oitsczzq.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nkxctjag.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2gvtknzfy.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2djlviell.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2zidyofke.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2ssejgdyy.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2rxlzysbe.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2ubdxslsy.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2cfexozoo.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujhalgvs.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2vmurrcyt.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2piyinofo.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgvbzskb.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.ydjk.org.cn/Article/details/gt2fnznfscn.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2uhnlpfso.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2frrrwbrb.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2wrlgkrdr.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2jbnnpkbu.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2evsvzyyh.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2gvcfqtkn.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2psuegzrk.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2iutavqei.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2digudxqm.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2wjyyvuea.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2ausekukf.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2yyusggoz.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hxgnjyjc.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2momtwqvp.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2pohqqldk.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2igfnbagx.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2zqvzfusu.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2luifbqml.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2clkrgsqf.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2yzdreazf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lxqkxkvx.html

O. 并发与异步
来源：http://www.ydjk.org.cn/Article/details/gt2sxiquhwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgdclprp.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2tybeluvu.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.52xcode.cn/Article/details/gt2apylmohs.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt2qealaobl.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2yosaddca.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2jprbdqzm.html


<!-- 参考信息 -->