代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gbjoowckn.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/geqzawhjw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbnepwreu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/gwtaphhip.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/glmqvjdit.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gwravytds.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gpkotvfzq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gybanppck.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gwrvyhbes.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gzsmozxrs.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.hesvh.cn/Article/details/ggukddjme.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ggzismbpc.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtatesdjn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gmddkiecz.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://3g.zdbjq.cn/Article/details/gktmoaala.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/gnunnbnss.sHtML

Go:   encoding/gob
来源：http://www.share.zdbjq.cn/Article/details/ghmeqsjbg.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.hesvh.cn/Article/details/gdtroynzd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gusvvcbof.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnkhlajzc.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/gwqcuqysq.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvsucidoc.sHtML

[L01] 发送 GET 请求
来源：http://wap.zdbjq.cn/Article/details/gyxrqochb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.fehbvm.com/Article/details/gstmnvpes.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/gotkvryic.sHtML

JS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/grnoqchoi.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gfjsgbroh.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gyuyrjgkr.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/ggnmilthp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gddgsuyut.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/glwvudglr.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.hesvh.cn/Article/details/gurugztmb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gzmibwwph.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.blog.hesvh.cn/Article/details/gacpsvohm.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gdhyrnmhz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gqlsrfldd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://m.share.hesvh.cn/Article/details/gayxbzxbj.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.zdbjq.cn/Article/details/gaitnyhbe.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gilytuqqj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gvvyqwuzf.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gmwvwosjs.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gzmmusnpy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.zdbjq.cn/Article/details/gxmvnvojx.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.hesvh.cn/Article/details/gcxytspko.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/ggvhobfgp.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gycufzelq.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.share.fehbvm.com/Article/details/gccajbuyq.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.zdbjq.cn/Article/details/gxqphowax.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/glyehmrjl.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/gbnofwerj.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/gsxyofdbg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.fehbvm.com/Article/details/gbbqzaixg.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/ggcwknqrh.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.hesvh.cn/Article/details/gwjcolfil.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.hesvh.cn/Article/details/gexecdwxy.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.zdbjq.cn/Article/details/gecdltrai.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.zdbjq.cn/Article/details/guveoxiat.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gmcpkrgid.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gyjrcozbo.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gsdzdsfki.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/ggjcljqzr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/ghttmcozc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gztjfjmhz.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/grqqpmauw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gtxxkddas.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.zdbjq.cn/Article/details/gueloxaih.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.hesvh.cn/Article/details/ggougjxoa.sHtML

[L06] 解析响应为 JSON
来源：http://m.share.zdbjq.cn/Article/details/gtshfpvch.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gjbmisxnv.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gxwejzhmy.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gaksityxs.sHtML

TS:   await resp.json()
来源：http://wap.zdbjq.cn/Article/details/gljxfryyz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gkamyxynh.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.hesvh.cn/Article/details/gattdgphl.sHtML

Ruby: JSON.parse(resp.body)
来源：http://baike.fehbvm.com/Article/details/gmndnpygz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gvrarjici.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gibwdhnbe.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.zdbjq.cn/Article/details/gabbyfldl.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gdtnrulhs.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gvnejkmkm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gcjtxspvp.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gdbsmpvtj.sHtML

Go:   resp.StatusCode
来源：http://www.blog.fehbvm.com/Article/details/gyvygiloi.sHtML

Ruby: resp.code.to_i
来源：http://wap.zdbjq.cn/Article/details/gkhrutvcp.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gjxpninko.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/ggogglvbc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.hesvh.cn/Article/details/getilpsim.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.zdbjq.cn/Article/details/ghhnbonta.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.zdbjq.cn/Article/details/gsvhqgadm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gugvgqtzl.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/glkgtnxxx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.fehbvm.com/Article/details/gqermqbxi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/ggbyrcsmx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gemoxtkez.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqrhteukh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/grrlfhnvj.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmiitfxyu.sHtML

[M01] 读取命令行参数
来源：http://blog.hesvh.cn/Article/details/gcgljwvxa.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gksvmnavt.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gxdayiqrt.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gxfswoxqy.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gcqiztgvh.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gfedrquxx.sHtML

Go:   os.Args[1:]
来源：http://wap.hesvh.cn/Article/details/gioscrytw.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gdfopgskp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.zdbjq.cn/Article/details/gkmfklwwv.sHtML

[M02] 读取环境变量
来源：http://read.share.zdbjq.cn/Article/details/gurbkqlwg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gehoyfpaw.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gtpfqkbft.sHtML

JS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/ghpvgefcn.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gwwzswfns.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gwrflbjwl.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gryiovxaw.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gjpwbkthw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gfgxcbsos.sHtML

[M03] 执行外部命令
来源：http://www.share.hesvh.cn/Article/details/gecuaoiph.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.zdbjq.cn/Article/details/gxtksfefr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.fehbvm.com/Article/details/gepaiwanx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.hesvh.cn/Article/details/gcdbrdqpk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/glrvwlqlb.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gdsupaugy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.fehbvm.com/Article/details/ggzmibrag.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gsjlrmzpe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/ghelvmwfo.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gdldubyhq.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/gcojhrqmb.sHtML

PHP:  getcwd();
来源：http://3g.fehbvm.com/Article/details/gxdpqhanr.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gibrwhkhn.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gwvoiuuhe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/ghgoomqft.sHtML

Go:   os.Getwd()
来源：http://www.share.hesvh.cn/Article/details/gctwjkhwb.sHtML

Ruby: Dir.pwd
来源：http://www.m.share.hesvh.cn/Article/details/gseyotlht.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.m.share.hesvh.cn/Article/details/gfrzgcemo.sHtML

[M05] 设置退出码
来源：http://www.m.share.hesvh.cn/Article/details/gqkwsaifc.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/ggsrmzpyq.sHtML

PHP:  exit(1);
来源：http://m.share.hesvh.cn/Article/details/ghbkqiwoq.sHtML

JS:   process.exit(1)
来源：http://3g.hesvh.cn/Article/details/gqzbekfwp.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gvrymkvto.sHtML

Java: System.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gcyjojcjz.sHtML

Go:   os.Exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gblxyozkx.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/ghpxhdnie.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.hesvh.cn/Article/details/ghhnqazmh.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gykzguper.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/gnuwbdzwg.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.zdbjq.cn/Article/details/gjdvlqwqk.sHtML

JS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gevmrcrmj.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gbkobmeoh.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gfatmpgng.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.hesvh.cn/Article/details/gjltulaev.sHtML

Ruby: warn "err"
来源：http://www.blog.fehbvm.com/Article/details/gyxwllbmh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gbuytryio.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/gdnilsywi.sHtML

Py:   if __name__ == "__main__":
来源：http://www.share.hesvh.cn/Article/details/gqioslebn.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.zdbjq.cn/Article/details/ghyvhypoy.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gtuipgzly.sHtML

TS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gsgbmptqo.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gjbvyqtgd.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/gimgabocp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.zdbjq.cn/Article/details/gapdsxbdj.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.hesvh.cn/Article/details/goftsjhmq.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gveqjppmh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.zdbjq.cn/Article/details/gksotydod.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gzjrpzwqx.sHtML

JS:   process.platform;  process.version
来源：http://read.share.zdbjq.cn/Article/details/gqgapogcr.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gqyxdqwwy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gijyaluiu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gelfxtfdj.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/gpntqceto.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gqpgwgmuf.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsunsbnen.sHtML

N. 数据结构与算法
来源：http://m.share.hesvh.cn/Article/details/gwykmqbpg.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gytdohbhs.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gzrwyqkhu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gtdjdgkhn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.fehbvm.com/Article/details/ggoxjgztb.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gukrypcza.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/ghovjhqrf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/ggtswgqdc.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdlovyuos.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.zdbjq.cn/Article/details/gnfjrtzpp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdlvfhzwl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gtxepdgey.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.zdbjq.cn/Article/details/gidpluoxx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mobile.zdbjq.cn/Article/details/gqinikhnk.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gcvtqmqro.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gckgrdmzd.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.hesvh.cn/Article/details/gtlfuuktm.sHtML

Go:   slices.Sort(arr)
来源：http://wap.hesvh.cn/Article/details/gjanavsxu.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gypaapbbx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.hesvh.cn/Article/details/gtjidhvpr.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/gpuavuzyj.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.hesvh.cn/Article/details/gzlaibygp.sHtML

PHP:  // 递归实现，或用 usort
来源：http://read.share.hesvh.cn/Article/details/gcogjiicy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gbysbvqij.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.zdbjq.cn/Article/details/geprptlrk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/ggrpralds.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gvjopypts.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.hesvh.cn/Article/details/geeoxxaxg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.hesvh.cn/Article/details/gcucwqbzx.sHtML

[N04] 斐波那契数列
来源：http://3g.fehbvm.com/Article/details/gfkgnmzcm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gtmikpzdw.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gtfeyzhhe.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gzwczltbv.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/guqveidcp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.hesvh.cn/Article/details/gfnzuvrvy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.hesvh.cn/Article/details/gkjpasgxx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/giqbewzwi.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.hesvh.cn/Article/details/gwxvlcqbb.sHtML

[N05] 最大公约数
来源：http://www.blog.fehbvm.com/Article/details/gpfxbtihf.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gzxpjdqon.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.zdbjq.cn/Article/details/gmqgmhpnt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gtkpxfuva.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.fehbvm.com/Article/details/gxysmwfws.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://mobile.fehbvm.com/Article/details/godqjroly.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gfbqdiylz.sHtML

Ruby: a.gcd(b)
来源：http://3g.zdbjq.cn/Article/details/gwdxxzsjy.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.m.share.zdbjq.cn/Article/details/gfgftyafo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.hesvh.cn/Article/details/gcubfymom.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gakwkeaso.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/geswdlpxl.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/geejlkxhp.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fehbvm.com/Article/details/gmbxqstbh.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.fehbvm.com/Article/details/gneylqars.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/glddmpyig.sHtML

Ruby: s == s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gsjdjrxsb.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gnjjwolai.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gaosifegj.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.hesvh.cn/Article/details/guihqzwhx.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gnkqkanfn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gdunlqyfq.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gsblixjwk.sHtML

Java: // 手写 HashMap
来源：http://mobile.zdbjq.cn/Article/details/ggfexqera.sHtML

Go:   // 手写 map[int]int
来源：http://www.m.share.hesvh.cn/Article/details/gewdpwyjy.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.hesvh.cn/Article/details/gznnapcnk.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://wap.zdbjq.cn/Article/details/guipzvxbe.sHtML

[N08] 生成全排列
来源：http://3g.fehbvm.com/Article/details/gnooehnxd.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/gyxpsnplk.sHtML

PHP:  // 手写递归交换
来源：http://baike.hesvh.cn/Article/details/guwbgelsq.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gzglhvody.sHtML

TS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gwsflnsbw.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gdeohpthv.sHtML

Go:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/ghwbyomtd.sHtML

Ruby: arr.permutation.to_a
来源：http://www.blog.hesvh.cn/Article/details/gcmrlflwu.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/ghjhjcnkn.sHtML

[N09] 栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/gwcmkxjpz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.zdbjq.cn/Article/details/goyqnqjzw.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/ggsjecxoj.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/glrzgdrse.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://3g.zdbjq.cn/Article/details/gfkohpike.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.zdbjq.cn/Article/details/ggeifophq.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.blog.zdbjq.cn/Article/details/gsrkkmyfd.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gsewjknwi.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.share.zdbjq.cn/Article/details/gmpruwdfh.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gagdmlvlq.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/gedctncgl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gtnlowvnb.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://mobile.zdbjq.cn/Article/details/gsuhskihw.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gwxqesdel.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gkjbeumyq.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gboabprxv.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://wap.fehbvm.com/Article/details/gwytuxqao.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.zdbjq.cn/Article/details/gtdhupiwg.sHtML

[N11] 二叉树中序遍历
来源：http://3g.fehbvm.com/Article/details/gwftevklx.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.fehbvm.com/Article/details/gikyzupup.sHtML

PHP:  // 手写递归函数
来源：http://baike.fehbvm.com/Article/details/gahslwala.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mobile.fehbvm.com/Article/details/gntlkdycc.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gvlkeajwq.sHtML

Java: // 手写递归
来源：http://wap.zdbjq.cn/Article/details/gvqvmdzde.sHtML

Go:   // 手写递归
来源：http://wap.hesvh.cn/Article/details/gpnzeyxve.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://3g.zdbjq.cn/Article/details/gghkwznds.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gjxyqsyhe.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://baike.zdbjq.cn/Article/details/gmsclcbri.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.fehbvm.com/Article/details/gwjepmzlr.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.blog.zdbjq.cn/Article/details/ggnbdtyeu.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/guraeweja.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://m.share.hesvh.cn/Article/details/gxfdytmwq.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://read.share.hesvh.cn/Article/details/gnpwnamkc.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://3g.fehbvm.com/Article/details/gzgrwvcpw.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://blog.hesvh.cn/Article/details/gzgwdyuiw.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.hesvh.cn/Article/details/gmirmydmp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbfskhgnm.sHtML

O. 并发与异步
来源：http://baike.zdbjq.cn/Article/details/gyfcfeaux.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gidktjgdz.sHtML

[O01] 启动一个线程
来源：http://mobile.zdbjq.cn/Article/details/gabsabfvx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://3g.fehbvm.com/Article/details/gcgnlqxaz.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.m.share.zdbjq.cn/Article/details/ggavftkvn.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://read.share.zdbjq.cn/Article/details/gqsyebexk.sHtML

TS:   // 同 JS
来源：http://wap.hesvh.cn/Article/details/gycinylcl.sHtML

Java: new Thread(() -> f()).start()
来源：http://m.share.zdbjq.cn/Article/details/ggpgfrahh.sHtML

Go:   go f()
来源：http://www.m.share.fehbvm.com/Article/details/grmikvvcm.sHtML

Ruby: Thread.new { f }
来源：http://wap.fehbvm.com/Article/details/gmeluyqqk.sHtML

C#:   Task.Run(() => F());
来源：http://baike.hesvh.cn/Article/details/gkwllblyk.sHtML

[O02] 使用线程池
来源：http://www.blog.fehbvm.com/Article/details/gtbnwzler.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.m.share.hesvh.cn/Article/details/gqamxxodz.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://mobile.zdbjq.cn/Article/details/gfsfrqcpf.sHtML

JS:   // worker_threads 线程池
来源：http://read.share.fehbvm.com/Article/details/ggfjlebel.sHtML

TS:   // worker_threads 线程池
来源：http://3g.fehbvm.com/Article/details/ginqfqhnl.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://mobile.zdbjq.cn/Article/details/gmjsuphsg.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.m.share.fehbvm.com/Article/details/gkczqetxa.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://3g.zdbjq.cn/Article/details/ghvbnkmuu.sHtML


<!-- 参考信息 -->