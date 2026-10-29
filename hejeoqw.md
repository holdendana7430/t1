代发 wailian999

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gxmnbkwgw.sHtML

[K07] 进制转换
来源：http://blog.fehbvm.com/Article/details/gnstgypsc.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gwakdftyj.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://read.share.fehbvm.com/Article/details/guwgqepdq.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gkdevsxay.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gqtvukogb.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gljvwotpo.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.zdbjq.cn/Article/details/geztedmek.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gttybynsj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/galtlelyg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.zdbjq.cn/Article/details/grwzqwdhq.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/glzsmqmtb.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.zdbjq.cn/Article/details/gouwtclij.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gvomrszcc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.hesvh.cn/Article/details/gaxooptcg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gsrbgcwfp.sHtML

Go:   encoding/gob
来源：http://www.share.hesvh.cn/Article/details/gjcxlwmtc.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.fehbvm.com/Article/details/giotnfzjj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gzhehmeon.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gelwwvfhn.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gllrligil.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gaegvppcj.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.fehbvm.com/Article/details/gdzyukzqm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/ghvnpfsok.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.hesvh.cn/Article/details/gxkoqxsqo.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/gtomnfqwd.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gudoldxfo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.fehbvm.com/Article/details/gpafpqloq.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/grswwywmj.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.fehbvm.com/Article/details/gqkeybtwu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/gwbvtjuoj.sHtML

[L02] 发送 POST JSON
来源：http://baike.hesvh.cn/Article/details/gmcyadqxk.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gdpftdhpw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/grxpxjxpc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gaihdvbbu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/gufuuduzf.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gmtazkzqu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gtjpumnxu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gdmyorjjn.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gonkopncp.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gwfwarccy.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.blog.zdbjq.cn/Article/details/gzyvzfkym.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/gmrwdvrfk.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/gjmtediwn.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/ggfsobssj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mobile.hesvh.cn/Article/details/gekcigpco.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gidqagwpi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.fehbvm.com/Article/details/gyerbmwdn.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gvexwmbam.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gmeinfgkd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.m.share.zdbjq.cn/Article/details/gvohxabmh.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.fehbvm.com/Article/details/gbrsktbny.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/guandejyw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gdbxzylhh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gffbjvvvx.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/gqourmbrr.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.hesvh.cn/Article/details/gcxrwpzwd.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.fehbvm.com/Article/details/gkwwdgyia.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gcbpzqhrd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gbsbknsma.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.fehbvm.com/Article/details/gdcyqbibt.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gexaiagsw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gzitomuuh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.share.zdbjq.cn/Article/details/gezosttpg.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gfachadfc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.zdbjq.cn/Article/details/gngbhqdst.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gngmdqfij.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gnigbsvtq.sHtML

Py:   resp.json()
来源：http://baike.fehbvm.com/Article/details/glnhtyvfj.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/gqejigrdy.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gkobjahdl.sHtML

TS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gzmfjxeci.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gnhomzzxi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gyqmzqrxv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.hesvh.cn/Article/details/gsocwkska.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/gjqdkznnp.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gioiotsaz.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gcyssswxc.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.fehbvm.com/Article/details/gjteqfccj.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/ggodvbolv.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/gvhrqpqaf.sHtML

Java: resp.statusCode()
来源：http://baike.zdbjq.cn/Article/details/gxtmyghsa.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gahtzcqkg.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gwpoakxbb.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gndxkiuok.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gtsnsmhqj.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gvuhusaey.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/gxvwutqbk.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gsehqyvbm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/ggcgiphpe.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/gfrohevgy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.hesvh.cn/Article/details/guymqqlxo.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/gbpuoumss.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gdpjzisyy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gweofwagt.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/grulztlpx.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gyehkyznp.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/gyftfncqg.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gngzmzagh.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gftphmglm.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gdabxiqfx.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gzqfadvke.sHtML

Java: args 数组（main 方法参数）
来源：http://wap.hesvh.cn/Article/details/gradqizff.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/goyzhnhzb.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/gljunkotr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.fehbvm.com/Article/details/gnpfznhto.sHtML

[M02] 读取环境变量
来源：http://www.blog.hesvh.cn/Article/details/gpiwjjcft.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/grjalwnqj.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gthhkktyd.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/gpkozngdq.sHtML

TS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gxvlnfkhg.sHtML

Java: System.getenv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gukwzuhql.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/godaypapn.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gxetaecdz.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gxpvupedo.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gwpewydrk.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.hesvh.cn/Article/details/gebxhtrej.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gxdwawmnf.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gwfzwlckw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gcslivhms.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gcggztbaj.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.hesvh.cn/Article/details/gxskfgfhl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.zdbjq.cn/Article/details/gewkfywbg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/ggwqoweci.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/gagowsgxs.sHtML

Py:   os.getcwd()
来源：http://wap.zdbjq.cn/Article/details/gqidfljkx.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/ggboxtttz.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gaawbdgis.sHtML

TS:   process.cwd()
来源：http://read.share.zdbjq.cn/Article/details/grdjosetn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gihsbxnvj.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gnqdzqopy.sHtML

Ruby: Dir.pwd
来源：http://baike.fehbvm.com/Article/details/gtkavhgmi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.hesvh.cn/Article/details/gvwtudhxm.sHtML

[M05] 设置退出码
来源：http://baike.hesvh.cn/Article/details/grppusvpr.sHtML

Py:   sys.exit(1)
来源：http://baike.hesvh.cn/Article/details/gdcrrtvci.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gtmecqyfq.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gpcwyedkf.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gkcdqcopy.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwivnrchk.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/ggxyegtgq.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/ghuzvhjxw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.zdbjq.cn/Article/details/gvsayvfve.sHtML

[M06] 向标准错误输出
来源：http://read.share.fehbvm.com/Article/details/gcbhtaupw.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.fehbvm.com/Article/details/gojkrkhbc.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gumyrzxlu.sHtML

JS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gluldqmwm.sHtML

TS:   console.error("err")
来源：http://www.share.fehbvm.com/Article/details/gpkbeafpn.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gpkqyhyta.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gdxnpdkua.sHtML

Ruby: warn "err"
来源：http://www.m.share.hesvh.cn/Article/details/gpjmunvup.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gvtntvgre.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gzqmwtejw.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gxmdnjqzy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/garhehygr.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gwjiguodr.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/glyqebvjz.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gzcweykmc.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gyscunhkc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gpodkffef.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.fehbvm.com/Article/details/gberruaqn.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gikbgaypt.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.zdbjq.cn/Article/details/gunmmdxvo.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.hesvh.cn/Article/details/gnelpxmmb.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gjkspzbim.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gocmrschq.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gwiezisxt.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gtkzwkmoy.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/ghrwiqggf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.fehbvm.com/Article/details/giolckiin.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gnccrzgav.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/grkanmsli.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gukniftid.sHtML

[N01] 二分查找（有序数组）
来源：http://wap.hesvh.cn/Article/details/glypivmnd.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gznacevma.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gzbpahhkd.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gmfieeayb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gtntkxpxo.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/givwulvjk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.fehbvm.com/Article/details/gotogbklz.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.hesvh.cn/Article/details/gqgmsvbtj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gvdountag.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gwfdfnfds.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.fehbvm.com/Article/details/gxaajubil.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gqzbwzmbq.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gbaepcrxp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gbbxsdhly.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.zdbjq.cn/Article/details/goecvgdga.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gsujajyfj.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/goeifudhn.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gsrpzluwn.sHtML

[N03] 快速排序（分治示例）
来源：http://3g.hesvh.cn/Article/details/gkroiozwa.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.hesvh.cn/Article/details/gtrvytytx.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gvvscwbai.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gsioygmkz.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.hesvh.cn/Article/details/gsmofcxoo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gecrtxdwc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gfspmaahx.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gplsdfswt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://baike.zdbjq.cn/Article/details/gpoecsmqp.sHtML

[N04] 斐波那契数列
来源：http://mobile.fehbvm.com/Article/details/gufopqmdo.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmabvwacb.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://baike.zdbjq.cn/Article/details/gphmlfnwp.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ggdirizme.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/graacdqnq.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gicbfzncc.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gvdibqbzx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/glcohungr.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.zdbjq.cn/Article/details/gqpreihrg.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gcawgvtjr.sHtML

Py:   math.gcd(a, b)
来源：http://www.blog.hesvh.cn/Article/details/ggpdlpmkc.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://m.share.hesvh.cn/Article/details/gwqlgvqus.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.zdbjq.cn/Article/details/goryjkswx.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gvooqoneu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.zdbjq.cn/Article/details/gxiuslsdx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.zdbjq.cn/Article/details/gbmzyfovs.sHtML

Ruby: a.gcd(b)
来源：http://3g.fehbvm.com/Article/details/givnpboox.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gspvqrqjz.sHtML

[N06] 判断回文字符串
来源：http://blog.fehbvm.com/Article/details/gcbtiqprg.sHtML

Py:   s == s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gspqjjnxf.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gajpqtsgp.sHtML

JS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gnavjciqu.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gxdbhrnzn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.zdbjq.cn/Article/details/ghyrspuuw.sHtML

Go:   // 双指针从两端比较
来源：http://wap.fehbvm.com/Article/details/gvmqmqpst.sHtML

Ruby: s == s.reverse
来源：http://blog.fehbvm.com/Article/details/gegesvgse.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/ghkkuousx.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/ggjiiaaxc.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/ghsqitsgm.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/geveumjgt.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/gwpgssdyt.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.zdbjq.cn/Article/details/gcxmiubyr.sHtML

Java: // 手写 HashMap
来源：http://www.share.fehbvm.com/Article/details/ggreryliz.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gdgwjjmik.sHtML

Ruby: // 手写 Hash
来源：http://www.share.hesvh.cn/Article/details/ghuidpzzl.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.zdbjq.cn/Article/details/guyhqavhc.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/gwedncswy.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.zdbjq.cn/Article/details/gduckvskl.sHtML

PHP:  // 手写递归交换
来源：http://baike.fehbvm.com/Article/details/gpxjlaboh.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gcuwafeka.sHtML

TS:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/guvqfwctq.sHtML

Java: // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gnympnnxw.sHtML

Go:   // 手写回溯递归
来源：http://read.share.fehbvm.com/Article/details/ggsakwlwp.sHtML

Ruby: arr.permutation.to_a
来源：http://m.share.zdbjq.cn/Article/details/ghchxonem.sHtML

C#:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/grhqkzust.sHtML

[N09] 栈与队列
来源：http://3g.hesvh.cn/Article/details/gneirbvkz.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.fehbvm.com/Article/details/giupncrge.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gjisgowjw.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.fehbvm.com/Article/details/ggqcyzgwl.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.hesvh.cn/Article/details/givvnhjpz.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gfaggeizl.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://baike.zdbjq.cn/Article/details/ghymrksfr.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gfltdymbr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gjgeeoeqv.sHtML

[N10] 链表节点定义
来源：http://read.share.fehbvm.com/Article/details/gtqcjyzdn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.blog.fehbvm.com/Article/details/glvqaplzb.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gsyfmwofr.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.m.share.fehbvm.com/Article/details/gshttdzub.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.hesvh.cn/Article/details/ggcbealrn.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.fehbvm.com/Article/details/gfpfxvxpx.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.hesvh.cn/Article/details/gkbevgnux.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.hesvh.cn/Article/details/gtciuiexu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gphwlenaf.sHtML

[N11] 二叉树中序遍历
来源：http://www.share.fehbvm.com/Article/details/gfdefmqnc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.hesvh.cn/Article/details/gplqxmwzb.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.fehbvm.com/Article/details/getfqymmp.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.fehbvm.com/Article/details/giczsuiym.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gnhdknayt.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gpwkqjkay.sHtML

Go:   // 手写递归
来源：http://baike.fehbvm.com/Article/details/giubekhpi.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.hesvh.cn/Article/details/gbfddyyse.sHtML

C#:   // 手写递归
来源：http://3g.fehbvm.com/Article/details/garlcdeuf.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.fehbvm.com/Article/details/gsycxwnnc.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mobile.hesvh.cn/Article/details/goraxsvgz.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://3g.fehbvm.com/Article/details/gpiyfarsx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://baike.fehbvm.com/Article/details/gmbqevyga.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.hesvh.cn/Article/details/gobptukho.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.hesvh.cn/Article/details/glzptieve.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://read.share.zdbjq.cn/Article/details/gchmwchhu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://read.share.fehbvm.com/Article/details/gkodzbphq.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://wap.hesvh.cn/Article/details/gqdockvve.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grgwzyafy.sHtML

O. 并发与异步
来源：http://www.m.share.zdbjq.cn/Article/details/ghpyqejpg.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdqjtatci.sHtML

[O01] 启动一个线程
来源：http://wap.fehbvm.com/Article/details/gpkgpedzs.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fehbvm.com/Article/details/gkxacypjs.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.hesvh.cn/Article/details/ggbolphmz.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://www.blog.zdbjq.cn/Article/details/gztmestwh.sHtML

TS:   // 同 JS
来源：http://blog.zdbjq.cn/Article/details/gohjnfuxb.sHtML

Java: new Thread(() -> f()).start()
来源：http://www.share.fehbvm.com/Article/details/gdhhytjuk.sHtML

Go:   go f()
来源：http://baike.fehbvm.com/Article/details/gnffcrukx.sHtML

Ruby: Thread.new { f }
来源：http://read.share.zdbjq.cn/Article/details/grcinqqrl.sHtML

C#:   Task.Run(() => F());
来源：http://www.share.zdbjq.cn/Article/details/ggxavpevb.sHtML

[O02] 使用线程池
来源：http://read.share.zdbjq.cn/Article/details/gswoymffj.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://www.blog.fehbvm.com/Article/details/gafarlfjg.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://read.share.zdbjq.cn/Article/details/gfxmezvyl.sHtML

JS:   // worker_threads 线程池
来源：http://wap.zdbjq.cn/Article/details/gypqzfmvj.sHtML

TS:   // worker_threads 线程池
来源：http://baike.zdbjq.cn/Article/details/gmgjslxvd.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://wap.hesvh.cn/Article/details/gwqwmcdyt.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://baike.zdbjq.cn/Article/details/guwerrrgv.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://m.share.hesvh.cn/Article/details/gdgmljebd.sHtML


<!-- 参考信息 -->