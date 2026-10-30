代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://3g.hesvh.cn/Article/details/gqeaqeefu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.hesvh.cn/Article/details/ghnieysdv.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gqnmkiuyi.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.zdbjq.cn/Article/details/gtoomwmto.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gzcwgzyxn.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.hesvh.cn/Article/details/gbqlkswwb.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.hesvh.cn/Article/details/ggkzjlhpc.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.fehbvm.com/Article/details/gwwhlmypr.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gwkyycobn.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/gqgyctsxi.sHtML

JS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/ghhtjijfb.sHtML

TS:   structuredClone(obj)
来源：http://read.share.fehbvm.com/Article/details/gudpmvvyn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://baike.hesvh.cn/Article/details/guabuonqz.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.hesvh.cn/Article/details/gjikkvbcn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.fehbvm.com/Article/details/gihowfumj.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gbrrdlblo.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/govauecih.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gyfjlkmpo.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.zdbjq.cn/Article/details/glmzsvgaj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gzdcxioqx.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.zdbjq.cn/Article/details/gywnsydio.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gkbqnymfi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gkfoyanid.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gidvgrnxt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gzgevcavs.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gdiojrftl.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/ggcwffbkq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gomrlmkfg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gpxfnqxtx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gybpccjfi.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gjehuambx.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gsqftrfhl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.fehbvm.com/Article/details/gfspjxltk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gzedmegnp.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://wap.hesvh.cn/Article/details/gvhfrcpwm.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gqfelmkjj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.zdbjq.cn/Article/details/gpuazvbwx.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gzhaihoyr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gjhmizjzu.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.zdbjq.cn/Article/details/gsslqlvio.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/govtjlyjp.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/gjuudlnnf.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gdhpkqcjf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gquduqpzy.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/glawzscvo.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggkjdwjny.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.zdbjq.cn/Article/details/gdqhbznju.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.zdbjq.cn/Article/details/gmafekxpm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/gtfvkomyl.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/gjnkwfxoj.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gioahyedc.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gshrmgidw.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gibtolnmt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/glzjfgfov.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/ggowqhulx.sHtML

[L02] 发送 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gpdvtcvdd.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gfzozdamw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gzwbijfuv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gqicywanb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gnvfrtdsi.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gabntxmql.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.hesvh.cn/Article/details/glyftzxlr.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gcyqbqbcm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.fehbvm.com/Article/details/gspncltnn.sHtML

[L03] 设置自定义请求头
来源：http://wap.hesvh.cn/Article/details/goewnvzap.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.zdbjq.cn/Article/details/gnmjbwzvo.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.blog.zdbjq.cn/Article/details/gfmlskeid.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gzclegtfm.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gfejegoys.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gxritnjjc.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/ghjzpdhzp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://blog.hesvh.cn/Article/details/goxtdirte.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gizpvlluc.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/ggyijgizg.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.hesvh.cn/Article/details/gxvigniqu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/giqcsdxlo.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gvlbxayor.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gkzafiivl.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.hesvh.cn/Article/details/ggfxanyai.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.fehbvm.com/Article/details/ghhezytnx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.hesvh.cn/Article/details/ghhsbgyge.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gxrpdgqlh.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gnxqmoccu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gxvbrbozh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gemtssuao.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gqxlfzgyl.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gpphvfclh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.hesvh.cn/Article/details/grqforryu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gkcezdojb.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/ggmzimjts.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.zdbjq.cn/Article/details/gxhrmadsa.sHtML

[L06] 解析响应为 JSON
来源：http://3g.fehbvm.com/Article/details/gdvpefvup.sHtML

Py:   resp.json()
来源：http://www.share.fehbvm.com/Article/details/grblujblk.sHtML

PHP:  json_decode($body, true);
来源：http://blog.fehbvm.com/Article/details/gcaqlaxlw.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gqnirvilk.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gogeptbqa.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.fehbvm.com/Article/details/gybsvzads.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.zdbjq.cn/Article/details/ggpbvqhiv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.hesvh.cn/Article/details/goajbpufw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gquhearsw.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/guqtyhxqr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gsmkjsvmn.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gzpoilgri.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gmtqcjmnr.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gmjxiwnwi.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gdecafftb.sHtML

Go:   resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gewwdfphb.sHtML

Ruby: resp.code.to_i
来源：http://blog.hesvh.cn/Article/details/gtcltxovx.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/ghgedqtmn.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/goyntphbu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.hesvh.cn/Article/details/ggjqqtroc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.fehbvm.com/Article/details/galnbfeeh.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gzxuctpxk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.hesvh.cn/Article/details/gnmxhqnes.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.blog.fehbvm.com/Article/details/gskpupixx.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/ggswqqywi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.fehbvm.com/Article/details/gzesgtmfp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/ghrmemgtl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gewhzoktk.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.zdbjq.cn/Article/details/gdykhwjvv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/getqlmbwx.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/gqcwcwqlp.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gksslxele.sHtML

PHP:  $argv;  $argc;
来源：http://3g.zdbjq.cn/Article/details/gogimsliq.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/gieblpxke.sHtML

TS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gnaecgjkt.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gjughrurz.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/ggeenrmus.sHtML

Ruby: ARGV
来源：http://mobile.hesvh.cn/Article/details/gvaxekfzn.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gfnyhsqjn.sHtML

[M02] 读取环境变量
来源：http://wap.zdbjq.cn/Article/details/gjjxkkefj.sHtML

Py:   os.environ.get("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwmxzjkng.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://3g.zdbjq.cn/Article/details/gumyiiymj.sHtML

JS:   process.env.HOME
来源：http://read.share.hesvh.cn/Article/details/ghauqlwvt.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gqwieuhwf.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gfagnogak.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdhzpnvhm.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gfboiwgws.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gdegmhluv.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/geawwmpqq.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wap.zdbjq.cn/Article/details/gqhyleref.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/ggxaklxwx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gmssmjkop.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gysbaabzr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gjbghdgww.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/glkqztvjq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/gvtjeiduu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/ghqqcsmzm.sHtML

[M04] 获取当前工作目录
来源：http://baike.fehbvm.com/Article/details/gxgzruzdz.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/gzidxwpoy.sHtML

PHP:  getcwd();
来源：http://m.share.fehbvm.com/Article/details/gnwthzdgo.sHtML

JS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gngvhqyya.sHtML

TS:   process.cwd()
来源：http://3g.zdbjq.cn/Article/details/gliohdeir.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/gobziiqat.sHtML

Go:   os.Getwd()
来源：http://www.m.share.hesvh.cn/Article/details/grkeiyjii.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gcejntujt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gsdpmccyg.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gelndndkv.sHtML

Py:   sys.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gbjqczhwj.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gasymsdcv.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/gvfbbcyfg.sHtML

TS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/gyvzufwgn.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwnmojhvq.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gyyssjqzq.sHtML

Ruby: exit 1
来源：http://m.share.fehbvm.com/Article/details/gexhbekur.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.fehbvm.com/Article/details/gojbuwznq.sHtML

[M06] 向标准错误输出
来源：http://www.m.share.zdbjq.cn/Article/details/goipcenbx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gpyfirudr.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.fehbvm.com/Article/details/gdheglkzg.sHtML

JS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gsujsaxut.sHtML

TS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gsxukkvez.sHtML

Java: System.err.println("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gvfiyuryp.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/gafcvtxww.sHtML

Ruby: warn "err"
来源：http://www.share.hesvh.cn/Article/details/gsapbgvxi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/glrthxedx.sHtML

[M07] 判断是否为主入口
来源：http://mobile.hesvh.cn/Article/details/ghwlumrdt.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gvpylszmy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.fehbvm.com/Article/details/gcmkccekt.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gflejuvoj.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/grydnsadz.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gbpcfevlm.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/gknavcsas.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gkcbkevcx.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.hesvh.cn/Article/details/gsrdgknip.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.zdbjq.cn/Article/details/gcddzuxox.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gjbtuexki.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/gzjmasyxj.sHtML

JS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gwxuofdcw.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gykzddxtb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.hesvh.cn/Article/details/gysvnaurp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://m.share.fehbvm.com/Article/details/gbqamkiru.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.fehbvm.com/Article/details/gylgiqfjp.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.zdbjq.cn/Article/details/ggmcvaoys.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghyckrvtu.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gojqzarbq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmcsmscgf.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gyezpmmhi.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gxjhvqujt.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gwovabrnf.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/goxzdjvbj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/guwqzbcaf.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gvkkfnsdj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.fehbvm.com/Article/details/grahwdntl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gyqfjgyvb.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gcuiynuik.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.zdbjq.cn/Article/details/gwomsnbln.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.fehbvm.com/Article/details/gvttfjrac.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.zdbjq.cn/Article/details/gvluqmmsa.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gfuxqlbgz.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/gzrjyiowp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gfxtopjyf.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gljpjsixp.sHtML

Ruby: arr.sort
来源：http://mobile.hesvh.cn/Article/details/gnypsgxbm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/ghpmjkkap.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.fehbvm.com/Article/details/gdmolguav.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gzyifjtuw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gfhyznzqh.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/gondixdxh.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/grcgoznno.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.zdbjq.cn/Article/details/gbeokazzm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gpxwyksfi.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.fehbvm.com/Article/details/gxwqgqhzb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/gxskyinhp.sHtML

[N04] 斐波那契数列
来源：http://blog.fehbvm.com/Article/details/gkwwhtfkh.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gohzuqjub.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/ghxzxlqrw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gqqygqtae.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gpgokwxyy.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/glxdkizrz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.zdbjq.cn/Article/details/gqujcttlt.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gsoycumqe.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gfjboqxby.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/gnifvnmmp.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gjxbwspqs.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.hesvh.cn/Article/details/gelaniieb.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mobile.hesvh.cn/Article/details/gfoqbcsty.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.hesvh.cn/Article/details/gkptgpdwu.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gssbxltcz.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.m.share.fehbvm.com/Article/details/guskvuqhi.sHtML

Ruby: a.gcd(b)
来源：http://wap.hesvh.cn/Article/details/gxiwwnfyi.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.zdbjq.cn/Article/details/gzsgfslpo.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gerxshoxa.sHtML

Py:   s == s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gykejqvkj.sHtML

PHP:  $s === strrev($s);
来源：http://3g.fehbvm.com/Article/details/gngcekagq.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gyvlhhsma.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.hesvh.cn/Article/details/gutfnncdr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gotqixjhn.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/gocpvtaql.sHtML

Ruby: s == s.reverse
来源：http://baike.fehbvm.com/Article/details/gzbitbtvs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gtwhjepdi.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.zdbjq.cn/Article/details/gnjgfocrh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wap.fehbvm.com/Article/details/gxnevnije.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.share.fehbvm.com/Article/details/gwsrvzakp.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://baike.hesvh.cn/Article/details/gbrzgriwc.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.hesvh.cn/Article/details/ghjgryzaf.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/getqmewkj.sHtML

Go:   // 手写 map[int]int
来源：http://mobile.fehbvm.com/Article/details/grhmofuie.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/glzaxqxps.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/gzktzetrd.sHtML

[N08] 生成全排列
来源：http://baike.hesvh.cn/Article/details/gbznmncre.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.zdbjq.cn/Article/details/goongcjhl.sHtML

PHP:  // 手写递归交换
来源：http://wap.fehbvm.com/Article/details/gbmpzijoq.sHtML

JS:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/geyfdqfpw.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gezirvlbi.sHtML

Java: // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gsnwzsudi.sHtML

Go:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gzebxrikb.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gradsatsa.sHtML

C#:   // 手写回溯递归
来源：http://www.share.fehbvm.com/Article/details/gjtbwlorx.sHtML

[N09] 栈与队列
来源：http://mobile.hesvh.cn/Article/details/gdycnsjem.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://mobile.zdbjq.cn/Article/details/ghhokuhhi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.zdbjq.cn/Article/details/gemqokznb.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.fehbvm.com/Article/details/gszjpkcci.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/gpfpjzpnq.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.hesvh.cn/Article/details/gdsibykpm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://m.share.zdbjq.cn/Article/details/ghrpyuhah.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://m.share.hesvh.cn/Article/details/gnpavqfhr.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://3g.zdbjq.cn/Article/details/gehocpgew.sHtML

[N10] 链表节点定义
来源：http://www.blog.fehbvm.com/Article/details/gjomwjegn.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://m.share.zdbjq.cn/Article/details/gnnvnlcpp.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.zdbjq.cn/Article/details/goyxtkvdw.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/ghbkwevey.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.fehbvm.com/Article/details/gegnukhlx.sHtML

Java: class Node { int v; Node next; }
来源：http://wap.hesvh.cn/Article/details/gzozyxbfe.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.fehbvm.com/Article/details/gnvbleqjd.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.zdbjq.cn/Article/details/grtxspysr.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gstonujek.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.fehbvm.com/Article/details/gtmkqzlbt.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.zdbjq.cn/Article/details/geivsggjv.sHtML

PHP:  // 手写递归函数
来源：http://www.share.zdbjq.cn/Article/details/geojoygnm.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.fehbvm.com/Article/details/gvkwxpyky.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.zdbjq.cn/Article/details/ggepcszon.sHtML

Java: // 手写递归
来源：http://www.blog.fehbvm.com/Article/details/gbhcfpkqx.sHtML

Go:   // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gnnepewqj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://wap.zdbjq.cn/Article/details/gilxkmull.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gjmsukhyi.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gddblnytp.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.fehbvm.com/Article/details/gdhliwlzo.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://blog.zdbjq.cn/Article/details/gpnvddnqm.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://www.share.hesvh.cn/Article/details/gyfhafepc.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/ggrykvvwn.sHtML


<!-- 参考信息 -->