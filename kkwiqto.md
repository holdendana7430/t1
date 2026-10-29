代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gfhnpicyl.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gronjtwcw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gjysdscjg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.hesvh.cn/Article/details/gmijkvixm.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gylakahfd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gaycqdbkr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gqkchgrif.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gvrtqgbvf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://blog.zdbjq.cn/Article/details/guigwwcnr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/glaipzbds.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.zdbjq.cn/Article/details/gnmjuqppm.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gdhysxkzk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.hesvh.cn/Article/details/gcnfuscgz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gfohqfuwg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/gvezllpct.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/gnztvjfik.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/gznixedcr.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.hesvh.cn/Article/details/gpmujacym.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gewuqmbmg.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gomioqctq.sHtML

L. 网络请求
来源：http://read.share.hesvh.cn/Article/details/gvbtwtnmd.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/ghiecspgi.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gjihywify.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.zdbjq.cn/Article/details/gmpfvtsrd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://baike.hesvh.cn/Article/details/gokldirzr.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/grrmgrdcs.sHtML

TS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gbhfmadtn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/gjdunmufk.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.zdbjq.cn/Article/details/golbuybwo.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.hesvh.cn/Article/details/gvxtajalj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gpxykikhs.sHtML

[L02] 发送 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gsfzouwrv.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.fehbvm.com/Article/details/giezzhldb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gbwiznrkp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gsbdryuar.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/ghyzfgcsr.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/grffkfdzx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gvjshsdit.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://blog.zdbjq.cn/Article/details/gufoeifuu.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gbpiqsjsk.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gsrctjpco.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gqoxpfovz.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gryrglaab.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gypzbxpfj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/ggatqzkrc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gqxcnvnyg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.zdbjq.cn/Article/details/giziczywa.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/ghsexqdxn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.hesvh.cn/Article/details/ghinfpqng.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gtgqaobcu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.zdbjq.cn/Article/details/gwtvcaksd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/glpppyung.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/gbcghiwjz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.fehbvm.com/Article/details/gsfldlnbv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.hesvh.cn/Article/details/gcmmyitxv.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gcekpxtht.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.fehbvm.com/Article/details/gplngrfcu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gvrckatki.sHtML

[L05] 上传文件（multipart）
来源：http://www.blog.hesvh.cn/Article/details/glcyarnno.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.zdbjq.cn/Article/details/gbvraavnj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mobile.zdbjq.cn/Article/details/gfxfhkrgq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/grncljvca.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gjlpteeue.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.fehbvm.com/Article/details/gtsomigvf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.zdbjq.cn/Article/details/gfnhwywmk.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gqfbjyzhc.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gnhxipkon.sHtML

[L06] 解析响应为 JSON
来源：http://wap.hesvh.cn/Article/details/gyntpjjjq.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gcaxjmjiu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gattmcpqb.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/grouoqlqa.sHtML

TS:   await resp.json()
来源：http://mobile.hesvh.cn/Article/details/gcezjlqop.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.hesvh.cn/Article/details/gcwszillo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/glbmjiorz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gdhefavxi.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gkdixopno.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gkkhhdekf.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gfqqgiixr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gesbuaycd.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gcknqfahv.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gbtdyjmvv.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gbylwnzzl.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gkrwdakcy.sHtML

Ruby: resp.code.to_i
来源：http://www.m.share.zdbjq.cn/Article/details/gydyixkzd.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.hesvh.cn/Article/details/gxufcxjrx.sHtML

[L08] 并发请求多个地址
来源：http://www.share.zdbjq.cn/Article/details/ghivehwuz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.hesvh.cn/Article/details/ghhqknjoi.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gepxmtmxv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gmpvrmxnw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gdayioluv.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.hesvh.cn/Article/details/gtcopsafz.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gbupybvkj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.fehbvm.com/Article/details/gfhnjodtg.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gbtlwmqeq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gnnsvozza.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gpbywckbr.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwepdcsbl.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gnbtckamy.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gqeubhalf.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/gujygwaxh.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gmteovmyl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/grqovpekv.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gvcqbxnmx.sHtML

Go:   os.Args[1:]
来源：http://www.share.hesvh.cn/Article/details/gdzfiskle.sHtML

Ruby: ARGV
来源：http://blog.hesvh.cn/Article/details/gdounajqu.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/ggcuddwkq.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gnwehzwdw.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/ghxmfigfm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gpxxxylhl.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gqdbkmkmp.sHtML

TS:   process.env.HOME
来源：http://www.m.share.zdbjq.cn/Article/details/gfdelgrnc.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/gemwsmrdg.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gncnzwayh.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/gnszhmwwv.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.zdbjq.cn/Article/details/ggvfknbnq.sHtML

[M03] 执行外部命令
来源：http://3g.zdbjq.cn/Article/details/giwanrnvi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gbhlanvuu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.fehbvm.com/Article/details/gymqgehph.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gxmkjvurh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gpcmzbwdo.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gimhldmex.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.zdbjq.cn/Article/details/gcfmfzqhv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.zdbjq.cn/Article/details/gldashmut.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/ggivpgwyx.sHtML

[M04] 获取当前工作目录
来源：http://m.share.zdbjq.cn/Article/details/gsbnlsnxz.sHtML

Py:   os.getcwd()
来源：http://3g.fehbvm.com/Article/details/gkrfnoohe.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gisoyryyw.sHtML

JS:   process.cwd()
来源：http://wap.fehbvm.com/Article/details/gnlsvsoba.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gfqtpazav.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gkixthhhc.sHtML

Go:   os.Getwd()
来源：http://www.blog.hesvh.cn/Article/details/gttwojrhr.sHtML

Ruby: Dir.pwd
来源：http://mobile.fehbvm.com/Article/details/grfdmvooj.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.fehbvm.com/Article/details/gbfrtjigv.sHtML

[M05] 设置退出码
来源：http://www.share.zdbjq.cn/Article/details/gypekhkhd.sHtML

Py:   sys.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/godqhflby.sHtML

PHP:  exit(1);
来源：http://baike.hesvh.cn/Article/details/gugaisvlh.sHtML

JS:   process.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gkriwlvfa.sHtML

TS:   process.exit(1)
来源：http://read.share.hesvh.cn/Article/details/grjctowjg.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gvdqpiaug.sHtML

Go:   os.Exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gxtenpjyg.sHtML

Ruby: exit 1
来源：http://www.share.hesvh.cn/Article/details/glohletkh.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gkgdfxjnp.sHtML

[M06] 向标准错误输出
来源：http://blog.hesvh.cn/Article/details/gwnviksep.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gprwkdeib.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/ggiqqbolu.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gtnzoilra.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gvmqtqhno.sHtML

Java: System.err.println("err")
来源：http://blog.fehbvm.com/Article/details/gyyswxrud.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gdlfuufpv.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gvibggdwk.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gccvpopbe.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.zdbjq.cn/Article/details/gnngwddpw.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/grobiygob.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gprwvazoy.sHtML

JS:   require.main === module
来源：http://baike.zdbjq.cn/Article/details/gtueavomw.sHtML

TS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gwzfqrxmm.sHtML

Java: public static void main(String[] args)
来源：http://mobile.fehbvm.com/Article/details/gxwvoxlls.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gwpewjmcy.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.hesvh.cn/Article/details/giikjjanx.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gafgibcau.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gaztwtmrs.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gionnuiur.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gzwcomvss.sHtML

JS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/gujqpujux.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gkaclqffk.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gbyhgnqig.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.hesvh.cn/Article/details/gbcohwkou.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.zdbjq.cn/Article/details/gaeijbklc.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/gxrmdbnwu.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gaxviulue.sHtML

N. 数据结构与算法
来源：http://m.share.zdbjq.cn/Article/details/girerdvzr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzmykoslz.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gakwugggu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gfllvlmjt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.hesvh.cn/Article/details/gdfrtetce.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gufsvvsot.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/garfqjfsr.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwcfxctba.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/ggitfabqj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://3g.zdbjq.cn/Article/details/gxcrxonpp.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.fehbvm.com/Article/details/gdusmsask.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.blog.zdbjq.cn/Article/details/gycqlzeus.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/gqhocrrix.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/goyaghthu.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gagtltfrd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gmrdlngvq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.fehbvm.com/Article/details/gvynzonvd.sHtML

Go:   slices.Sort(arr)
来源：http://baike.zdbjq.cn/Article/details/gphfzvhrx.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gdczjgyhx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/guymidgrq.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/giznbusvz.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gmrofziqq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://wap.fehbvm.com/Article/details/gwhibijxo.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gepeadqnl.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.zdbjq.cn/Article/details/gestwmarb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.hesvh.cn/Article/details/gkxbqgqdj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://m.share.zdbjq.cn/Article/details/gfohaeygv.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.hesvh.cn/Article/details/ggkeeqqug.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.hesvh.cn/Article/details/gjnxqcmjq.sHtML

[N04] 斐波那契数列
来源：http://read.share.hesvh.cn/Article/details/gtfysebdt.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gcubzfwgs.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gbowkabdj.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/geenvwtfn.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gdviwtkyt.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wap.fehbvm.com/Article/details/gbpflpmhd.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://3g.fehbvm.com/Article/details/ggyghcisl.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gyemssimf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gykbczoii.sHtML

[N05] 最大公约数
来源：http://blog.zdbjq.cn/Article/details/ggfhwdzdb.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.hesvh.cn/Article/details/gdccgmseh.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gkvqukczt.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/givnophje.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gpqzrcdjl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.blog.zdbjq.cn/Article/details/grtrpocje.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.zdbjq.cn/Article/details/gtamkjhph.sHtML

Ruby: a.gcd(b)
来源：http://blog.hesvh.cn/Article/details/gamvuamrz.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.fehbvm.com/Article/details/gksaacjpl.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/galgzqmlg.sHtML

Py:   s == s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gnlwrnuik.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gnnbbnvsn.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghinszpzr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gwilhieyi.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://m.share.fehbvm.com/Article/details/gxhkpgnvy.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/gtwjqcdcj.sHtML

Ruby: s == s.reverse
来源：http://mobile.hesvh.cn/Article/details/gdzrdwusq.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gntiddunw.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.fehbvm.com/Article/details/gctrzaxzn.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/giijzlesv.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gsgnpziij.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.share.zdbjq.cn/Article/details/gumwpxyrr.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.zdbjq.cn/Article/details/gebtzvuqm.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gdrpnjdeo.sHtML

Go:   // 手写 map[int]int
来源：http://www.share.zdbjq.cn/Article/details/gkadsrtde.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gxpwarnld.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gwvutzoee.sHtML

[N08] 生成全排列
来源：http://www.blog.fehbvm.com/Article/details/gjwmzojlm.sHtML

Py:   itertools.permutations(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gapcvmtby.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gajprbfsd.sHtML

JS:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gapqqedsk.sHtML

TS:   // 手写回溯递归
来源：http://blog.hesvh.cn/Article/details/gdpoydfvn.sHtML

Java: // 手写回溯递归
来源：http://mobile.hesvh.cn/Article/details/gifqsvzow.sHtML

Go:   // 手写回溯递归
来源：http://wap.fehbvm.com/Article/details/guzxktjyy.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gbyrnmalk.sHtML

C#:   // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/gvknghmjj.sHtML

[N09] 栈与队列
来源：http://blog.fehbvm.com/Article/details/gnbzstsdn.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wap.hesvh.cn/Article/details/gdnxleqpm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gxuxhlgvd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gsigqyzkd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.fehbvm.com/Article/details/ggoriaber.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://baike.fehbvm.com/Article/details/glvlxersh.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gawnrttvh.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.m.share.hesvh.cn/Article/details/grlsinlca.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gxejumdir.sHtML

[N10] 链表节点定义
来源：http://3g.zdbjq.cn/Article/details/goafyivde.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://wap.hesvh.cn/Article/details/gmcawqstc.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://wap.fehbvm.com/Article/details/gmmufqicq.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gsjketysu.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://baike.fehbvm.com/Article/details/gfmkxcknk.sHtML

Java: class Node { int v; Node next; }
来源：http://www.blog.hesvh.cn/Article/details/gtgtqodsc.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://baike.hesvh.cn/Article/details/gtejjbpax.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://blog.zdbjq.cn/Article/details/gorddxdpz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.fehbvm.com/Article/details/gmdhlglyr.sHtML

[N11] 二叉树中序遍历
来源：http://blog.hesvh.cn/Article/details/gychipnlm.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gpavgobhj.sHtML

PHP:  // 手写递归函数
来源：http://3g.zdbjq.cn/Article/details/gqwtswaii.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.fehbvm.com/Article/details/gtnuctdku.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/grlynevfv.sHtML

Java: // 手写递归
来源：http://blog.hesvh.cn/Article/details/gybywwopo.sHtML

Go:   // 手写递归
来源：http://m.share.zdbjq.cn/Article/details/gnkapnnrv.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.m.share.fehbvm.com/Article/details/ghvcaatnx.sHtML

C#:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/ganmhghmv.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.hesvh.cn/Article/details/gkgjiwnxu.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://www.share.hesvh.cn/Article/details/gtfmyhziq.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gdhbsphtm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.blog.zdbjq.cn/Article/details/gpnuopzpz.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gfhxunosz.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://3g.zdbjq.cn/Article/details/ggfpvkzwa.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://wap.hesvh.cn/Article/details/gcyrkudto.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://m.share.fehbvm.com/Article/details/gtpauotxh.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://www.blog.fehbvm.com/Article/details/ggcmdfcrq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gitoviyhf.sHtML

O. 并发与异步
来源：http://read.share.fehbvm.com/Article/details/gqeuomovc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxxeljnfl.sHtML

[O01] 启动一个线程
来源：http://m.share.fehbvm.com/Article/details/gxwpqtqzs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://read.share.fehbvm.com/Article/details/geqqzgqjb.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://3g.hesvh.cn/Article/details/gvnqsdkel.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.fehbvm.com/Article/details/gmcirixwo.sHtML

TS:   // 同 JS
来源：http://www.m.share.zdbjq.cn/Article/details/gzaabsgzu.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.blog.hesvh.cn/Article/details/giitjusbw.sHtML

Go:   go f()
来源：http://m.share.hesvh.cn/Article/details/gixtpjkbc.sHtML

Ruby: Thread.new { f }
来源：http://www.blog.zdbjq.cn/Article/details/grzlgjgfl.sHtML

C#:   Task.Run(() => F());
来源：http://mobile.zdbjq.cn/Article/details/gmscgqxus.sHtML

[O02] 使用线程池
来源：http://www.share.hesvh.cn/Article/details/ghnseimah.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://m.share.fehbvm.com/Article/details/gyyxpjvsb.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://wap.zdbjq.cn/Article/details/gdgbyxdju.sHtML

JS:   // worker_threads 线程池
来源：http://www.blog.hesvh.cn/Article/details/gpxkgcpng.sHtML

TS:   // worker_threads 线程池
来源：http://blog.hesvh.cn/Article/details/gangbrkva.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://read.share.fehbvm.com/Article/details/gdmffhqji.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.hesvh.cn/Article/details/gchafnjgj.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.fehbvm.com/Article/details/gszkjhdtl.sHtML


<!-- 参考信息 -->