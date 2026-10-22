代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nlbcqssx.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2kpgflwma.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2irhdtkwy.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2waggmgrd.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2mthprnzt.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2iwsgosmq.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2iqimpcqz.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2qebzddzx.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2tfhaysfd.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2eekutpvc.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2umshfbkj.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2werztghm.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2svrwkbev.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2ibshnahf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ubfrkqhz.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2zgqjlaac.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2pcdkigmt.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2joblemht.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jsuqifga.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2sfgsugjv.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xtfxxirc.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zoacqjmo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2bteoxgoi.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2rklnfzew.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2idvbmrmc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2jmfreemd.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2yntspqms.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2jcazzznb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2adzteftq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ydakrmid.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2zssoyytj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2uyktnthh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2vnfsgkhn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2euiwuppx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2ahxhxzkg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kxtgkuqx.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2ndsetvev.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vyqbfbbu.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2hyhqpbov.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2xfhfrcnl.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2borkmcks.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2gvqrwdoi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2mxmkppry.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2cxafddmc.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2kwsinpnq.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2milwcrkm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2yqbkqvsi.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2njcvxosi.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2bcybzwwl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2qofafbzq.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2xzwcgzte.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2frqysfqz.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2cnaprfsw.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wzrinsep.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sthyattv.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2bzjjeztk.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mviotygr.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2xxlsepja.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2gzsmlplm.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qxocdgrn.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2wpbghwrk.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2trgmotqq.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tnsmpijk.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2lfyvhcgj.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2yohjkrxv.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2nrzuapja.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2qwjecwls.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2irvcoqdt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2qramvckx.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2amgsestb.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2nwysjxrv.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2vvmzsgzg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2iptgnypm.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2crpuqeqa.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2qnpbmwxi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fpohbgcc.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2pctoyrvt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2bouxxxfu.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2zggckoiz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2jxlazfvu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2wqhcyhaf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2cqpbxwjp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ibkgsuzg.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jmkouqsg.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2lzlesehb.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2ammwhund.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2detljsdk.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ytlmhsbc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bcbxnmwb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2smdnzwlq.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2aetxiwig.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2iitvopcr.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sdffmlbt.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2psyxeqim.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sbacvxnv.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2qebirpxa.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bvvkerqk.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bbrdzfmg.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2rmgtkvkd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2juonitqo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ckzohhhr.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2epnvzcdu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2vqvafirc.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2clrdcgyu.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2uqpbiuav.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ljzmoqme.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2gcivzxbw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2ebypcxgf.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2eyqmghma.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2hhhezpzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2chshszvv.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2qhtdkafa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bswtodbz.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2zjqvdjgx.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zbdzugbq.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2zhqlxdcg.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2gieqjxaw.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2vhyvvnth.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2yhznbndm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ydtcskvk.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2ltpptuqh.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2havibzvf.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2eekzqoop.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nugetdqw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2tbuqjevj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2gbujezci.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2nizkuxoo.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2prtlgxba.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2caoldbpp.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2togsntzr.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wekjazvj.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2wvqrwrct.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2wvzvqdaa.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2meiucvez.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2oqrvwvok.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2ckwegeew.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2szyilwom.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2ixyykdjc.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2vqrbuazk.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2xsitfkjz.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2gxoleeae.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2iwljumpi.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2dfcyrark.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2ajalmacd.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2grlwuhvr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2opvmanco.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2znjhteep.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2mefawwox.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2btgqrcxh.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2qdyirsky.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rtxlajme.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2tfgrrmbw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2yhtskkih.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2budmgsqy.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sfpjseej.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gpdfubbf.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2ngbsvcke.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2wsihvpzh.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2dsxaqdyj.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2kafndjus.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2zpjquhle.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2lwmoqcbc.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2swqrnvzy.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2xplygpjo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2aoznkjkg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ffhsumqx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2wzkdguor.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cpqkrilb.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2gmeezlyu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2obukfccq.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2dquefhjh.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2cashuxtd.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2uxxowqeg.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2nhacpqov.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2tlfgeeol.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2bpifvqyl.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2cniwvujd.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2yazohyxz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2cotpjxqa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ldnwmyru.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kmmwpedo.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2ylwqjvrq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2lrjjsbid.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2whyuvxln.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2iynejhnf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pdzqobnr.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2lsylovup.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pcbczezq.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt2nkufwtjh.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tklgylrf.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2ksjhgqcc.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2zdiykeeb.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2rtuyjmpi.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vzdezqbp.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2mwpidomb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2owqkytnx.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2leskqqhz.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2hefquouj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2ewiafecw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jgdafics.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2mipukovy.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ojytgdqk.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2nhwgvoly.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fsibpecz.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2sfntkcjj.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ijgvqzjk.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qjumfgje.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2rmblbhrn.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ijsbnslr.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2nbbhxcuz.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2iktjpxty.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ouuyczvz.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt2ujttokro.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2gbrwvqfw.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2xlciuxga.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2ypozuwsi.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2wbyempni.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2kofaiwif.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2konwrjqv.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2cwlsqdpt.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2qpnowoxh.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2gecmcarz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2rgizexab.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tfeuqeez.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2zmmybbpg.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2nfcwkxco.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2scgoqoyu.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2wdocgpjt.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xswaqwei.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2obzeokdp.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2ceenhzbv.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2zwbfqznt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2odnelhco.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2epvszapz.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cotpafkl.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qgghjdfa.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mrdqtpij.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2epoiqbev.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2cerlftsv.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2udouydvg.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt2xolvtexe.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2fojufvwx.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2ixjlselb.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.ydjk.org.cn/Article/details/gt2xdgxizuo.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2gxzllhpo.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2xyuwukch.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2dnwstkvk.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2uoioknlp.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2razzwuhd.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2igummkft.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2jcsvjgnp.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2xscohhuw.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2nfdgzsou.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2mgphceer.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xyhxlroh.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2icozgbcd.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2bjarntjx.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2klxogssd.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2ofcsmpwh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2hbdzqxmb.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2edzglwkb.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2ajbvdlru.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2zswfhckk.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2nlgqbxjd.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2rgvnwzhv.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fvqzijba.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt2qreziays.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2nocvkybq.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2dqoduktt.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lggxaymq.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2fyxgfaoh.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2paydjomk.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2trsxwiaf.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2eksefiae.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2flbzmuop.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2cvggquig.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2gelltvgd.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjuvmlsp.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2fmygzlnc.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2xvxtibom.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2uemoxskg.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2lidovcqv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2bjlinoqv.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2uzppsisi.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2goxvcbpp.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2gpqlmrhm.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2nxgfjglt.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2nzvoerrh.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt2ibfctjst.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.52xcode.cn/Article/details/gt2tuimuhom.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2oobiibpa.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2teaeelhc.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2pskstect.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2brlsvaoq.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2muwzignk.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2llvzrjst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bshtzhop.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2gapmqzpn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dcoqvicw.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2irzvcatf.html


<!-- 参考信息 -->