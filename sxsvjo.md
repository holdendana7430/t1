代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2rswrieyc.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2rafaefwk.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2miecctet.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2pladxzxk.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2axhajdfy.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2yfcmmbro.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2hlrnhvci.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2xysnzrep.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2kfyiuaae.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2yymjsumt.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2hhuirmbo.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hvwozdhh.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2biofjeop.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2bhekgyke.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2cqyztetm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kekfosox.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2sdslunvy.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2eqnuuikp.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qgpomfda.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2ybsorrzo.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2ciqfahql.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2kweuqqex.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2tnxacxwy.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2yuifpqyv.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkogyar.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2zqyknbkf.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2cdzweoww.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2mivceuur.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tulbmlmy.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2djhzsxsy.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2lufckeum.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2tzagsnld.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2bsbudmau.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ywfrlwat.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2kibcojrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zctphpwc.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2pgvklijk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvqwdqpc.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2tunxmazt.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2mmryqggi.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2kangplpe.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ymiopexo.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2grxmdfix.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2cnwfltsb.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2gdqssdpu.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2fcppripf.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dwpkgxxs.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fgvjfavf.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2zdiivgvg.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2yazqoptc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2obmhaucf.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fsnygauc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2wxsdahpt.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2nfpnhvdc.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2uohprwli.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2tiefehrz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2zcaobbxf.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2lakrqyel.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ummgfcuu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tkiwbwzr.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2tfpfowzy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2logtqywg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2cnwrgluc.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2avksdodh.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2hpvdttan.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2rplghfvj.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2wnezndoc.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2cdmxvmmq.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2ehvvzbea.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2hoipswxu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2joilwjyq.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2oaibdwuj.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2llwbbkiv.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2nvsqfetx.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2xdxxuunt.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2ucbrbeue.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2hxfasbca.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dsmopdti.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2jxciouua.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2tezmscan.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2fqpfhwdd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2esuqyuhq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mepqyqix.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2rlipcsmv.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ztoflicl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2zridekmr.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2riwwlusg.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ckfbxxbu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2rxsxmwqb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2yvdhwsmi.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2mgwpxpzk.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2iudhgvai.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fvnygipv.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2mtyrjyza.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2sxogvayl.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2mhumyrws.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2jyppzhgw.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2bckklcuf.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2nhuruxao.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2ejyycrcl.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2vsfofgpc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2nsytceom.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2usaxsxvz.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2pkjoehus.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2mqdasozs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2qxzhbywh.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2nxusszso.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2vbiywejn.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2hqibsaoy.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2wvhnvjas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uocfygxp.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2eihuexog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gkbakwjg.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dydjlmwk.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2wjlehqil.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2rczzflzt.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2ziztczes.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2xvpsdgal.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2atggexel.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2ehlbnbvd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2oqzcgtbc.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2imejnnmq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2wuzjfawy.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pfzbywca.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2wotxiouw.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2rlilghzr.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2juhpymgf.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2rgqhnpfy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2nnhkvtyg.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2fsxqlong.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2dhexkkny.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2dbzlhzuq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2mstpgyzh.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2trzdnvdm.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2oaeukzzd.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2sxbcdwvr.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2uliatjtc.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2lsilwdfq.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2fqaevzll.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2bqhiwxjx.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2cstiigbx.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2kycebuqh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2oofcrwyp.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2znvtkwdb.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2zcokioyz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2ehlqcszj.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2hgzpypvz.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2dukycbhy.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ibtjfdmj.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2fetzduah.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xsrxknyd.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2bvqtmggy.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xjibskhz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2geisqngo.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2souhndjk.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xynujdlg.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2sdcwbyhq.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2glrrbcip.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2bsyvoifs.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2cloopqcj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2wxtgecqx.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2feprkgbb.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2vfjkssqn.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2otacjqwm.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2lkodniqg.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2vnprhkew.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2aafdzktl.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rsnnxzuo.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2micbcdmk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2plirisnz.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2btdxxvcw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2pxvdmjlh.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2hxmdvoem.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2gufisoyq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2vtfrylhs.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2ntrvvusf.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2ptyoncai.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2ddntraty.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2qnphuseo.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bmcmfmnd.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2otpsggps.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2wbyunbtp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2stepwmab.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2udpiqjra.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2nlxexujo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdwcgtja.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2kyufjqto.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2urblyekl.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ywidjrgz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2xsenjqxl.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fssmkixy.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2pkgtrcmw.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2zunffddr.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nuvbuelr.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2oxcygfjg.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2qfkmknta.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2toaqlskk.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2bhbfpxnu.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2buvdsliv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2xnitqpze.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2xuumnyfx.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2ljjvokgs.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2gkasrfzv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2llxjgtmh.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2fursmoja.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2ztscmqlx.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2bktvjana.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2cjcnizaq.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2hhndmyyc.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2vsyckrzp.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2ehofhfgc.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.52xcode.cn/Article/details/gt2ngfbtvtm.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2mnhzhfda.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.ydjk.org.cn/Article/details/gt2lhfnrcsj.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2twmrgisk.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2xfzxoine.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ovwzadri.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2xotfwhbr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2syvtnouq.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2brvqmzva.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2utwbbeku.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2sbzixzhz.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2hvikqtdw.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2yirrkknu.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2kngpfggm.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vdwdmhea.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2xecriuba.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2jfpnmuma.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2cdkmqymb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2zgzgxdgr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2chzctkxs.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2tortnkvl.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2wiaperzn.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2mwedlpol.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2fauhvqbd.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2byxvcnod.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2urxyylwv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lqiqyvem.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2rfaxmexr.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2itogdzlo.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2qqsulbyx.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qdnsgetn.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2hslhasgg.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2ydyorfco.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2nusodfpp.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2uqyyjiwx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2ctglyblw.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2lneagfey.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2myhvegkp.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2ovydllas.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2qtwzcamk.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2inmitiwq.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2hbumgrlj.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2vybixxtv.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2pbumzncl.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ewrwlque.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2teqpeiiv.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2euyftzkc.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2rznhvcea.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2inpgcdie.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2yhshhpga.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2jyoxtmur.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2btjyhkta.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iybxkjzt.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2qrjckhws.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.52xcode.cn/Article/details/gt2qvwwxfiw.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2rfwhqfad.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2gsbxuuqs.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.52xcode.cn/Article/details/gt2zhlbowci.html

[N10] 链表节点定义
来源：http://www.ydjk.org.cn/Article/details/gt2agorbiap.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt2roveesrv.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzcxgzrh.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2weboyofk.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt2hlljxkaa.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt2dewxmyiq.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2oprvfppf.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.ydjk.org.cn/Article/details/gt2ezelhlio.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt2qpngxrpo.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2yrzsbrmw.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt2aqpxlrqb.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt2pstepere.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2cduxvomb.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt2xanfdpbg.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2wapitnor.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2qeymepdh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt2bjspkapl.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2xwgeodbl.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt2odgtexje.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2hxbaoezf.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2btqmgjkf.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2uhkrhjfl.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt2jhupiwbg.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2erteliia.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2aiyrnmyk.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt2lktprqad.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2ivudkomw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unlmwtwd.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2fipfalld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jcrhcjgu.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt2gjtiqklv.html


<!-- 参考信息 -->