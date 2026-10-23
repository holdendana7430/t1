代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3aqiyuwzj.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3bfkwzcmb.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3rakmbrqg.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3agzomict.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3pcutmuyw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3pxmitkce.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt3jryvqrzf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3itayvbxv.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3vqjlhvxz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3hdljtxqp.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3iodepguz.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wclbggpg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wipnzkow.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt3pthwnmld.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3uoafgqbl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3pnlzhafx.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jcmgkxeh.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt3jnhfqjba.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3zrqzsijp.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3mxxxfpxg.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3uleokftw.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3tjihujwz.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3cziefase.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3jtsfnfbu.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3ktdlnjdt.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3esxxoasx.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3fwdababk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3odjbyadu.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3diiaonhq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3wsqayaqn.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3kjldwkye.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3hzrsmadh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3lcyscvsf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rthpmxpw.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3cpkxuwax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gfjwfffm.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3fxixelzu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3arzbbjdv.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3tialoqer.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3vfvfkjgk.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3cfagbwqh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3ujsagnld.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3vwirqbkv.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3tpptbqqi.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3uxkdifpm.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3pqlqckqn.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt3zqezdntq.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3biaxjurm.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3xudypunm.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3wuzfjkbu.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3fjtznrfi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uqxhulfv.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt3dzodmwvb.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt3ucrgvdxn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3wbqbeqpt.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3hyxfkdgw.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3ggicpgwl.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3qrpxwwsp.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3gnfftfhw.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3nuvfhnlw.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3rhtcztfs.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3hardhkzn.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3szflalwm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3xesaqitq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3fvagtpit.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3lurddkkw.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3wndptggr.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3xivndmpa.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3aasuufgz.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3kskvgeue.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3hjepnolh.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3nfpoyvho.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3hertpcci.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3bvlldgvt.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt3uuvlmqmy.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3zyxlwcib.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3pirflaqf.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3vyijqnhx.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3osneetqi.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3plmodlro.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3pwlsnnqq.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3xpiaqwqx.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ycveetjr.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt3xzmjsrns.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3lkogyinl.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3uqzviumg.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3impbivxq.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zbtbeenf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3butwyefj.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3nvqpdngj.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qmoabtrl.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt3fdrxsbfz.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sjegiare.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3hblokzde.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3masfgrii.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gokvxjos.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3yxmnyzur.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3utmtnvbs.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3pgkvdkop.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3jjxrocdm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3afelaljf.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3cxpzdimg.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3woukqoyv.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3efwdsgai.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3pbasvheh.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3dvsxwljp.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3gpftgzoq.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3unrfvcqw.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3qlvlaxsg.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3fsonheqw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3izdtsptn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3svjjjqer.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kyrrnwxf.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3lskoxakj.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kapszphe.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3qpoxbfme.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3slhjpspy.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3iobtawbo.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3zsivfdqc.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3lqqsxtyp.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3lwvwiwba.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3hjdghxdj.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vfmsjcky.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3lptupmjn.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3zvcqcgmq.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3wypjgxdj.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3wldewskm.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3brloirty.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3nvfgpglf.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3fnvccsqx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3nepnumpm.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3fqfsqjhq.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt3kgfwszhm.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3mnfrntpo.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3hssyqbxo.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3bdornvah.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3plxpjptl.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3vguvkjrt.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt3myorsuvp.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3zifxryxa.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xrlvedbe.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt3juhvefyh.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3zehnclbb.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kaovqmio.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dlojpndd.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3ahcekejv.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3dfhzbkxg.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt3jejuwgpk.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3zllpxajy.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3osgobvls.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bimgecwv.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3ncbyihku.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3xhkvqhmt.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3usxehnoz.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3nzqlmmmv.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3auipezpp.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3kjfehkgs.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3urvnymmm.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3ymvjbplo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3icrmnegx.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3mmrrpwtw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3fzbxklji.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3lppfepnd.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt3zrpmdydk.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3ttwpmztu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3jwbgdhfo.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3xcrxnyim.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3byvqtmvr.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3qswrtezy.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt3ytjrtune.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xrelhuji.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3binciszw.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3vihlryqv.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3euxtrtzd.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3idxqixip.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt3uyvydiii.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3qmcvtxtj.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3ndvkhvtr.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3snzpgmby.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qxaiouhb.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qnjmsvux.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3mdnozler.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3fjqwjwyu.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3xaebvhen.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt3dgaojbby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3thmbykcm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3tkjyrrlf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3svpawchu.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3tjtrjapz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qleavfff.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3elmcmhqr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3yovismas.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3circgogw.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3sckwkvtj.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3finybkax.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3kkqyfwhq.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrzuytc.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt3auibvenj.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt3cdvgvgyy.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt3qsxwozvk.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt3xkfdmcwh.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt3wocmuyjq.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt3bxajwuvr.html

Go:   slices.Sort(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nwhemheu.html

Ruby: arr.sort
来源：http://www.52xcode.cn/Article/details/gt3akleyqzr.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt3jvgqxxvv.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt3ehrspprl.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt3hwptvcnt.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt3iyjnsnsf.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3zkkhvroj.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt3jqccewxn.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt3xvjlicsx.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.52xcode.cn/Article/details/gt3ucrznpby.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt3etlzkham.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt3ubwiptup.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt3pznziuke.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt3kgxgtymm.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3dtdwlhtj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3ejixyduu.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3pfumbdzs.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt3kvmhaobl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt3ayqsnzre.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt3bahoecub.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt3slubkdcc.html

[N05] 最大公约数
来源：http://www.52xcode.cn/Article/details/gt3tsexnwoa.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt3moeiemjt.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3cetlwigb.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt3vmrfzvpr.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt3ysxyjxis.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.ydjk.org.cn/Article/details/gt3zgezlylk.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt3fmdrnnvu.html

Ruby: a.gcd(b)
来源：http://www.52xcode.cn/Article/details/gt3kikvofbw.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.52xcode.cn/Article/details/gt3fqeaxfwa.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt3wootdwgi.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3itzudtpm.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zapjihfq.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xoqhvmze.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3remaiipl.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt3oeelavsj.html

Go:   // 双指针从两端比较
来源：http://www.52xcode.cn/Article/details/gt3xyjapcme.html

Ruby: s == s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tljusnov.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3yjvedtid.html

[N07] 两数之和（返回下标）
来源：http://www.52xcode.cn/Article/details/gt3pzivbsxi.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt3piebrkxz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt3erzdptij.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.52xcode.cn/Article/details/gt3dhswpvxx.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt3xvtovktu.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt3fzyvgpga.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt3naziqxyr.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt3gmxulasy.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt3mwbmkwne.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt3otrcosei.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt3kgmozyti.html

PHP:  // 手写递归交换
来源：http://www.ydjk.org.cn/Article/details/gt3dzwvplib.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3mgjgzjot.html

TS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3srttwxis.html

Java: // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3vvzbcdkd.html

Go:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt3hdadgpdh.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt3lptpwyvm.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt3okbrsavt.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3emowyrjp.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt3frpxafrd.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3iwahqhnl.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt3qbuwtndq.html

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.ydjk.org.cn/Article/details/gt3ygenspwi.html

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt3gjjgksnp.html

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.ydjk.org.cn/Article/details/gt3eaisncwp.html

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt3pbguzblm.html

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3kpjmlwme.html

[N10] 链表节点定义
来源：http://www.52xcode.cn/Article/details/gt3pczpsntj.html

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.52xcode.cn/Article/details/gt3ebwguzhx.html

PHP:  class Node { public $v; public $next = null; }
来源：http://www.ydjk.org.cn/Article/details/gt3llobadhj.html

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.ydjk.org.cn/Article/details/gt3agekcwbs.html

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.ydjk.org.cn/Article/details/gt3peoqvjtu.html

Java: class Node { int v; Node next; }
来源：http://www.ydjk.org.cn/Article/details/gt3zlqfoiny.html

Go:   type Node struct { V int; Next *Node }
来源：http://www.52xcode.cn/Article/details/gt3zolvmtee.html

Ruby: Node = Struct.new(:v, :next)
来源：http://www.52xcode.cn/Article/details/gt3ofphykuv.html

C#:   class Node { public int V; public Node? Next; }
来源：http://www.ydjk.org.cn/Article/details/gt3wunlowza.html

[N11] 二叉树中序遍历
来源：http://www.52xcode.cn/Article/details/gt3talrqein.html

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.ydjk.org.cn/Article/details/gt3bqqifnxt.html

PHP:  // 手写递归函数
来源：http://www.52xcode.cn/Article/details/gt3ncilvdpj.html

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3wqjkjfre.html

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.52xcode.cn/Article/details/gt3mtpofdkx.html

Java: // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3jwhxcrcd.html

Go:   // 手写递归
来源：http://www.52xcode.cn/Article/details/gt3spaganqh.html

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.52xcode.cn/Article/details/gt3sxzckpul.html

C#:   // 手写递归
来源：http://www.ydjk.org.cn/Article/details/gt3qictwfhs.html

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.ydjk.org.cn/Article/details/gt3ahtrqodv.html

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.52xcode.cn/Article/details/gt3blopacfn.html

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.ydjk.org.cn/Article/details/gt3lhypamxy.html

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.52xcode.cn/Article/details/gt3bnrxtghf.html

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.ydjk.org.cn/Article/details/gt3wcobeiux.html

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3ukxfpdgy.html

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://www.ydjk.org.cn/Article/details/gt3cmkqkvhf.html

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3xhurreku.html

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.ydjk.org.cn/Article/details/gt3twouibdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jnzynitw.html

O. 并发与异步
来源：http://www.52xcode.cn/Article/details/gt3eoxffrvl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wzdjpakz.html

[O01] 启动一个线程
来源：http://www.52xcode.cn/Article/details/gt3xkuxaztn.html


<!-- 参考信息 -->