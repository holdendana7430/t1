代发 wailian999

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ofpgnnzm.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3nfpkjaqy.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3timdlbuq.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3jdagysty.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3mweqwgbh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3vfqjjkcf.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3bwbnpmnv.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zonjmtwc.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mklqosid.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3gjphzxkv.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3gdjyfpmb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3jmafskwx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3dnfrcfwf.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3amkjczmh.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ydsvuuuh.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3qriepcja.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3dyvtmmdf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3wsfajtof.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nifhfxix.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3lhdcopkm.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3rapcmenk.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3xttkynle.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3apzxaibb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3uwwthtst.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3lozkbmjo.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hrqfrtdg.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3emveajyt.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3njdarpjq.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3puviyjki.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3lvelyjdq.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3agpwjsut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgmfrail.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3flxtebri.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qvxqxypf.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3ukuukwie.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3aulpeuwe.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3egjsuzfz.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3fhsrifua.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3qpynukhk.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3gmplgles.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3cqpmyzcw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ydixcvvm.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3evzscddk.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cozvbmqe.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3yqetmcot.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3pqqeuhcv.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3buwxslff.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3buekwupc.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3brytkxaz.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3duvquubj.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3lnwxtycp.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3xplfqxxr.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3zcvlgpyo.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3qeuggfez.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3tcyncubh.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3nwncvfcl.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3ztxpiwob.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3xhteamxg.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3rundqaev.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3qwybwjmc.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3hvkdeoru.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3loveywrd.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3pwtjvtyf.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3qkkapetl.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3occuilit.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3wqhmnzoq.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3pskpzbuh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3otpwyzpc.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3lsxwpjcs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3idsnvywk.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3rjqobbak.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt3uorbpepb.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3hnhffwyi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3iyxyrdin.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3jvnludfa.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3hvmdkvqv.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3gyitacul.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3rtrutmwu.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xlkfwmdi.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ffpknrto.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3ctlnpsql.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3ytexvcug.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3bbsrckco.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3qnodiapu.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3ximmmlbd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3vexfgink.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3kwnjjgzc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3kdwwvjlx.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3honlvvfe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3tzecnymo.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3kztejmwx.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3aeyjwwds.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3dmocnjaq.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3tzwkgmfb.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cgfmnimh.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3mtedyfvy.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3cgbbmqrp.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3imjcjrib.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3tzzesbti.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3yzyjnvro.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ujkfatcm.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3tmbfiexo.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3jlvmwhck.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3vwnlzfzs.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3kdpcrpqm.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3qdlfirru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsweekdz.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jtxeegaw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mxplqtwp.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gzsovqig.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hafjwlae.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt3uoyqqpah.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3lkxbhvxg.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3dsylunfk.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3vrxjzkai.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3crikjpug.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3nukkyial.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3hycowkfy.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3okyykhnb.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3vicaqyiq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt3rlciuegu.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3njrpqkjf.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3htmfngfv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3thogijtf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3odqncrby.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fsgbeykd.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uwzfjptt.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3liuakdyw.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3wuubhhvw.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3rvmjghim.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3lnbdsvka.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ohzgomjo.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3dlbbybwg.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3iyuyvcmf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3rsomjecj.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3artowrhd.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3ppbvcznn.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3cixayurw.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3ptezyvwz.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3iebvqode.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3aixjsktz.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3uplvrncc.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3ainmjmcr.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3rdipyndt.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3elllzvyk.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3dsymoklf.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nlvyzwnc.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt3vgykzaif.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3updwifsu.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wmdunacf.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3cfdnjunm.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3iehhzoxd.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3qjdtnoha.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3dhqguytr.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3zjdyvbqv.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3sovrjxrt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3pbulnhpw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3crrnyzhw.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3ailytyvn.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zotukixt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3uvjcusbk.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3chhecqjx.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3phhkfqbd.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3grrcnpnc.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3pwymrnam.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3sjifptxb.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3ithqoell.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3qdobexht.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3ujjirxtx.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3slecfdqb.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3tnbsfiov.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3qvcrxver.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt3xbmxwyia.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bmtalert.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3fzjvtnan.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3jelklszr.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3vntabrmx.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3rhlyilfz.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xpnypzpi.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3gsxyokjy.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3jsdstkju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xupnjrhj.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3rcrgxhhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csksnyyu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ruxjgiba.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3lcozemvj.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3mldzrizk.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt3hjipxrxg.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3juwqkobb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3biksdidu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3fiytjlue.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3uoyduoav.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3unybakuh.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3rapbajfx.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3wiaoxsgv.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3pbixxair.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3fuionkpi.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3ywzpdacd.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt3qddmyrmf.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3emqozhvs.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3ppmtsrbp.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3imtxdksr.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt3lhsfbzxq.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3dznydjja.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt3risbqjuy.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3iguexese.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt3becivxod.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3amkkggfx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3hvatowzl.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3borkpeea.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3imvoghmo.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3cumjkkxa.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3tlmctnwj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt3fggbtnyr.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt3bnavqkla.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3onvoksmj.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3oriuaftk.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3pbmpvlor.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3ckozebse.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3dtigiimk.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3kizecone.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3sbcdfgkw.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.52xcode.cn/Article/details/gt3fbxogqjm.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3xtddcmkb.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3eelhjpza.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3pekmbzxq.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.ydjk.org.cn/Article/details/gt3mdbhtraa.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt3bhqzfxpt.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3yduvxljc.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3qagalvcg.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3npiokbhg.html

PHP:  $s === strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nzggclrv.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3eeddiimf.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lfoyagda.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3ziakqwxd.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3faanfkpq.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nmmadkqm.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3tzmrqrwy.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3pfitxbxr.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3guhvwbnm.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt3uhgkszkn.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3udqnzqsp.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt3jclqvdli.html

Java: // 手写 HashMap
来源：http://www.52xcode.cn/Article/details/gt3dweqxdmp.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3msgcvcxg.html

Ruby: // 手写 Hash
来源：http://www.52xcode.cn/Article/details/gt3rgxabfgl.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.52xcode.cn/Article/details/gt3jbmjkwud.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt3uueroprr.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3pbjbqwvd.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3apinmyed.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qdugvolf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iucltwzq.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3iuefnrjw.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3qimxjbut.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3yiminumg.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3lrgbpaev.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt3hbtewpax.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3glfqesrv.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3bogyxkff.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3sbbmnbef.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3nmqvczfe.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3frwhsgvn.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.52xcode.cn/Article/details/gt3xvranvnd.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3vkqpdjnc.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3wfqxjrsw.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3wcuuulfx.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3uuwfvcdm.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.52xcode.cn/Article/details/gt3juyrgtsw.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3aghpyrjl.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3bimkchna.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wzdoknjr.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3qblbgyrr.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3wqphzudu.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3ztrteuso.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3fkksacva.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.52xcode.cn/Article/details/gt3vcazgbmy.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3blaluerv.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3fdovvlxi.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.ydjk.org.cn/Article/details/gt3qonvblug.html

Java: // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3efyptjln.html

Go:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3fqqxmmpx.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.ydjk.org.cn/Article/details/gt3tszfbpsh.html

C#:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3ujpectcd.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.52xcode.cn/Article/details/gt3iblznbsr.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.ydjk.org.cn/Article/details/gt3hoohomlv.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3edeirhce.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3ahyicnow.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3plojzcbl.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3nrojdpav.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.52xcode.cn/Article/details/gt3wxnqprkd.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.52xcode.cn/Article/details/gt3axrozsey.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.52xcode.cn/Article/details/gt3yfmlghoh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ieqfgval.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3memjdmui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cbrtfumn.html

[O01] 启动一个线程
来源：http://www.ydjk.org.cn/Article/details/gt3isslaeaz.html

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://www.ydjk.org.cn/Article/details/gt3ssynraxk.html

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.52xcode.cn/Article/details/gt3qovvwjpn.html

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.ydjk.org.cn/Article/details/gt3qhzwwtli.html

TS:   // 同 JS
来源：http://www.52xcode.cn/Article/details/gt3jbvnttet.html


<!-- 参考信息 -->