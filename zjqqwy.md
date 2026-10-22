代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2rjhpsdjw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2lhkzltqj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2leanyljv.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2hrdrqrbt.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2jtcrzcfv.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2nsrvherq.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2qljbrtmy.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2cskrpgid.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2akjuojhp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2grynwawj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2uajjqwob.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2rptsxiac.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2wqfdozti.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt2lxsniquj.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2quuobpvk.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2sdqzueeg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cbhcjfsr.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2bcdjulrb.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2opjmhalt.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2gxsjbans.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ykgovyuq.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2yjrqiahs.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2nufmybtp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2fomodens.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2jmzxzios.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2tbsbyojm.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2rpchleka.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2ysallotj.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2mvktqiqn.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2spzqjnsu.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2fwzobtlq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yathjioj.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2nasshnot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyeqrzbk.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2avfeggey.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2wojwdnbd.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2fjsekxxb.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2fuvzeoua.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2jviqmioj.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2vhdfwory.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ydsertry.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2zilznzin.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ydhbgrhq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2ayvyznjc.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2jejvomly.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ecmdvdkp.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2icjmkmeo.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2rkyrdkrv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2zrljnjsm.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2iwgcpqgt.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2utewxnny.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2qhbqtkio.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt2mxcduwtm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2szjyuwsq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2mnnbqkah.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2qzumqnba.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2nhzvhhbr.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt2rjwfzymr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2fhjftjce.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2ejiclwfn.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2zzswptsb.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt2gdrucalf.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2svdivdmm.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2lmdjuiio.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vpbwghqa.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2dfpifhmu.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2oggfrahi.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2octtifmh.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2vzedesws.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2wcadfujt.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2leuunrjj.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2fynehvrb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2zegvnzjb.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2xgebflsg.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2wohycbsq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2gyaycluw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2lkjhwgpy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2umkhtfqm.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mkfyrcyh.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ooelmyib.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2swcarrac.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2qknwntye.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2nhcazxbb.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2zldxdpau.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2fkkxcpfc.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2ofzdmrgd.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2qbsaunkb.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2szmncnpf.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rgqrctvp.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2ggeucdjq.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lkrorppm.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tjimfful.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2tyyvudty.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2tnjljmpd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pglmosrx.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2zccbjeez.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2kwpcnqym.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2enrslaid.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2iwcobmbu.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2qifduory.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2vrvqhibz.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2jpyxkxul.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2guoxleeu.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2myzukxnu.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2seerprfh.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ytwpkgii.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcolphlk.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt2avcgqtgx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvwbekpy.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jqetvcrt.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2aryybpjx.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2wubdjxjx.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2nxbwgyve.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2zzyuajeq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2jzlbakky.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zhfypxbj.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2dvntdukd.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2rorohbds.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2odrrsduq.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2ocssoabi.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2exrwxhmn.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2grqwnvnt.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2cepieyyo.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2pyqyadbi.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zlslkavi.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2knlvtxek.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2zavjcayl.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2dfngdzth.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2qbyobmkj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2uxyskkia.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gxgjuood.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2wsnylfnh.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2xjiqwjle.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2msboxmge.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2mavylmzc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2ogoodatr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2sbcznqve.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2tykjmkeg.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2eimladld.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2bsneyoar.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2waafgznc.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2hvfeghyi.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2bslqhfkg.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2aokzpulm.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2avptxyde.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2btdnitdi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2aticlftv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2qujdzrdr.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ayahucuo.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2zjbmzost.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zbtmyjhn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2doowlkmw.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2dlefcwvh.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2pkujubfk.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2aprecuwf.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2avlpixdj.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2kzbstuhp.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kcbkausr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2yhrpawei.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2gzjjolnz.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt2rkbjhfbf.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2dmkmrvpf.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ddgtvynr.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2nrgggoed.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2wlacwtcu.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2fuargxwn.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2nklgxmzb.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2fgdrdots.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2qfahyzcc.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2towrnoxo.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2gbubepkf.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2iipzqcuj.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2mgmamopn.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2cstbphzn.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2yvmpayck.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2tqkfwily.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2cadkcbyz.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2ifoymejp.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2ztbfqccf.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2zaillwlx.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2mzdnuoov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pucvuhtk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2pxilqofz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sfqqzbqo.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2mpcwfhnm.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tzbsqche.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2hgsanfib.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2gwhebiyi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2fwopphpx.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jmrdfozv.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2hwitcwbb.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2scxcvzhc.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2kkrrjskj.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ttoobffv.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jcggfekw.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yyqkywhv.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2xwhthcfh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2vwyytdcq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2upwkkwow.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2wbwbwwsx.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt2uvbcarsd.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.52xcode.cn/Article/details/gt2vzcfajls.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2qqolgytx.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.ydjk.org.cn/Article/details/gt2lruqgtwv.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2abbljptk.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2utbfmzro.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2axmzvmyx.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2ofxozdve.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2evzthvzu.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2oocbmjio.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2hzckhxiq.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2maqicwub.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2pkvaqylx.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mypmphed.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2cedpquod.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2tpzjqnip.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ubarmhom.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.52xcode.cn/Article/details/gt2vokaggxp.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2lcanwyzx.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2aaofcnsk.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2gdxlovib.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zwhxbpnp.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt2viiohjvh.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkysnhch.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2unzwgiye.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt2hsiaanmg.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt2xnkmlzlq.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt2seqojqss.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt2vpvbzayi.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2zxulkpoo.html

Py:   s == s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zlsynzgi.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2zcnjlfdg.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2tgwnkigo.html

TS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pnifnqtr.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2eytrflkz.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt2rwnelgxi.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2egpsrilq.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2nnjnhsvr.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt2tthwarhy.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2bllypjtd.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2khvyiydu.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt2hayxiuda.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2uqofclbs.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt2owsdowfb.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2apgycjlz.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt2gpxocznm.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt2mutjqqny.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2wpdkfhrg.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2apuzyxso.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt2bbngyuqa.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ukoomwfp.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2anpoxtti.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2ntyukxgi.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2jrvhtblv.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2ulcnvyaz.html

C#:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tgdninsl.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2ikvbubjq.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2acvfhknw.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2dcjmnpaj.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pvfsutoy.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt2xvgaqdqo.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2fotflnwy.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt2gdvljeao.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2hnhxrxsf.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2pjrhpvpc.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt2lkubmzdx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.ydjk.org.cn/Article/details/gt2gktlhbfy.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt2vtlumlty.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt2omuduwjr.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.52xcode.cn/Article/details/gt2teirdeiy.html

Java: class Node { int v; Node next; }
来源：http://www.52xcode.cn/Article/details/gt2jtjtequd.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt2lyfgxeng.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt2zdnvewfm.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.52xcode.cn/Article/details/gt2ihkqboyv.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt2bkbkjfjl.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt2gaozgfzf.html

PHP:  // 手写递归函数
来源：http://www.ydjk.org.cn/Article/details/gt2ywbywogj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2ysulzujv.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt2sstbarjq.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2jdhywcds.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt2btsbtize.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt2buowxthb.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt2pakarted.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt2ublvcimj.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt2dnlpdcwk.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt2ycfohlrj.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2rrynqmiu.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt2silnkbon.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt2nqdioeni.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt2nhmdqlam.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ofnusbtw.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt2tfcnbpiv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rtwhabtm.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt2difyyjrn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zuswyali.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt2qsawgmhr.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt2epklmguj.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.ydjk.org.cn/Article/details/gt2retrxypc.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt2hsxjxdzz.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt2ipvavoxd.html


<!-- 参考信息 -->