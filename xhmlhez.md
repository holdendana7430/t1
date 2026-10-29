代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gsywcvzmb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gycosbdvk.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/ghmwcxefw.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.blog.hesvh.cn/Article/details/gnarjyojx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/glpzjjpqb.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.hesvh.cn/Article/details/gettefban.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gvwacdmav.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/gkuvohrgu.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gzchhhypb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://wap.zdbjq.cn/Article/details/gizqspali.sHtML

JS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gdpiqgreg.sHtML

TS:   structuredClone(obj)
来源：http://blog.hesvh.cn/Article/details/gnwngcoqy.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gvkklqjzu.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/gqaftbwwk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/gadkzextz.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.hesvh.cn/Article/details/gvrqjmgct.sHtML

[K06] 解析 URL 查询串
来源：http://blog.zdbjq.cn/Article/details/gjveiddki.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gnmndizwx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gzzlqcczf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gviktedpt.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gfyhbofye.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/gyvoydarc.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gkruzqffw.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gsmcwdifb.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gyzsbwfdw.sHtML

[K07] 进制转换
来源：http://baike.zdbjq.cn/Article/details/gyrvvoyow.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gjqxqsuez.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/gnoxqeofy.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gspndeuto.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/ggvbqontc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.fehbvm.com/Article/details/gtzmmyzno.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://baike.hesvh.cn/Article/details/gopzyamju.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.share.hesvh.cn/Article/details/gjqlmpvgc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gmrtmqceo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.zdbjq.cn/Article/details/gntshwovy.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.hesvh.cn/Article/details/gznivfpcq.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.fehbvm.com/Article/details/ggnxhsitw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/glmixaxax.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://blog.fehbvm.com/Article/details/gtrfxqgji.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gkwatdcyb.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gizldlaiw.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/gwycxamys.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/guzfkijfw.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gpfawgxwf.sHtML

L. 网络请求
来源：http://read.share.fehbvm.com/Article/details/gjmqkzomx.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gymslvsug.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.zdbjq.cn/Article/details/gwvfazqhm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gmssetmqa.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gewodrpsy.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/glnvjyuvk.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gbmqenvuk.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/gurcgyyrz.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gkrvewwrl.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.fehbvm.com/Article/details/gpdemzdel.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.zdbjq.cn/Article/details/gcbvjlfzt.sHtML

[L02] 发送 POST JSON
来源：http://blog.hesvh.cn/Article/details/gknpnncex.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gogbexdia.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gcyskaiwr.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gmtkzbxhb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gspviymba.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gbjkrasii.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/gnbdajkbk.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.hesvh.cn/Article/details/gncjztnil.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gzbkygivc.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gqekejhfr.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.fehbvm.com/Article/details/gfydkwwvw.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gjrxfgkiz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.fehbvm.com/Article/details/gwaogkehg.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gsiilstwc.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.zdbjq.cn/Article/details/gaiflzprl.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gejviqdii.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gcqznyvoz.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gwpiaqopu.sHtML

[L04] 设置超时
来源：http://wap.zdbjq.cn/Article/details/gksjjwprx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.hesvh.cn/Article/details/gganiwgmp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.zdbjq.cn/Article/details/ggvkwjake.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/guskgcqav.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.hesvh.cn/Article/details/giobctrnr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gaznxsynp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/giitfgufz.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gwyywplgp.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mobile.fehbvm.com/Article/details/gqmbjdwal.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.zdbjq.cn/Article/details/gafgnaetu.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.zdbjq.cn/Article/details/gfnfviksg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.fehbvm.com/Article/details/gregrdvlw.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.fehbvm.com/Article/details/gwvmwwqpz.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/gfexaoflx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gdacisvfu.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gqzmksdvf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.hesvh.cn/Article/details/gnmcstgkv.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gdwlhfpvp.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gpqqmnvhn.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/gmnnfxbws.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/giarvpnhq.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gsqzbhvhr.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gjmfbdhuj.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gmjcmnfii.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/gbpnwchcz.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.hesvh.cn/Article/details/gaysdbwmr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gaqyoysjp.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gtqarinyd.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gcfcuobbr.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.zdbjq.cn/Article/details/gjhurxzoh.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.zdbjq.cn/Article/details/gyuflpjed.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gjkekgias.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gbclickkd.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gphpluioe.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/grbqdjxyp.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/gqgloleig.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/gvrpzmdvy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.blog.zdbjq.cn/Article/details/ghpmqtupl.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gwslwqggd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gncimzoum.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gmuykefme.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gukuwotog.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.zdbjq.cn/Article/details/gbwkwhpdi.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.fehbvm.com/Article/details/ghvsubgcm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/geafymunv.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxeicopzg.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gpfmxciwu.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvayxictp.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gmuzcpvrr.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gkemqkifr.sHtML

PHP:  $argv;  $argc;
来源：http://blog.hesvh.cn/Article/details/goqmasxcm.sHtML

JS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gocbkfqcn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gbkqizdud.sHtML

Java: args 数组（main 方法参数）
来源：http://3g.fehbvm.com/Article/details/ggoodhngz.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gphvaoijs.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gjvoeecrb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gyyeogltc.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/glbcmrklh.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gdmzpksyn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.fehbvm.com/Article/details/gbovfypos.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gjpnhteko.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gmibkipdv.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/gkvrabgdi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gwskfyczq.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gblpvvbzb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gdacblobp.sHtML

[M03] 执行外部命令
来源：http://blog.zdbjq.cn/Article/details/gpzcjgpdv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gusrruidh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gtbbswlqx.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.hesvh.cn/Article/details/gvkubkpcv.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gmgobband.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gxeinpcef.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gzhuxtsix.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gfxtoqfjw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gbhgnthyl.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gobppzzqt.sHtML

Py:   os.getcwd()
来源：http://blog.hesvh.cn/Article/details/gqaccgyaw.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gahnrwgkx.sHtML

JS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gaeqdxuyu.sHtML

TS:   process.cwd()
来源：http://m.share.hesvh.cn/Article/details/gemqdwrcn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/gsicxxgii.sHtML

Go:   os.Getwd()
来源：http://baike.fehbvm.com/Article/details/gpolbsxcy.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gyvkkcims.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gfdulakkk.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gttkgzwvv.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnbowykdn.sHtML

PHP:  exit(1);
来源：http://m.share.fehbvm.com/Article/details/gwbnbevxj.sHtML

JS:   process.exit(1)
来源：http://read.share.zdbjq.cn/Article/details/ggrcnrofj.sHtML

TS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gcwklxvru.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/guvwavcny.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/ggaslxjhw.sHtML

Ruby: exit 1
来源：http://m.share.hesvh.cn/Article/details/gmcvnphui.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gidtzqmjq.sHtML

[M06] 向标准错误输出
来源：http://m.share.hesvh.cn/Article/details/gdrgjttin.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gumftytum.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.share.fehbvm.com/Article/details/gnsawcuta.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gwpnknfyi.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gwfurzyoa.sHtML

Java: System.err.println("err")
来源：http://mobile.fehbvm.com/Article/details/gvioxazso.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/ghpykipls.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/getpjwjmj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gerpxasgb.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gekocfwam.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/glxrspsbt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gfchdowax.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/giuxejbpj.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gcwmcmhaj.sHtML

Java: public static void main(String[] args)
来源：http://baike.fehbvm.com/Article/details/gymfyfybm.sHtML

Go:   func main()
来源：http://3g.fehbvm.com/Article/details/geozeypey.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://m.share.hesvh.cn/Article/details/gqsklvkcy.sHtML

C#:   static void Main(string[] args)
来源：http://www.share.fehbvm.com/Article/details/gbxomxqib.sHtML

[M08] 获取系统与运行时信息
来源：http://3g.fehbvm.com/Article/details/gdsjddibw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gyglenuvp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gqvlaedfb.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.fehbvm.com/Article/details/gxvuxnqqr.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gfdtkiycv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.zdbjq.cn/Article/details/gdfworvtq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gpyqbnkeo.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.hesvh.cn/Article/details/gdwijmukh.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/gsrhwfbhu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glbyclvtf.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gvnldgouv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpdkiloqa.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gfjrxuizg.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gzptjjxlj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gdymdkrig.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gevawqboh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.hesvh.cn/Article/details/gxqgfdtef.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/gvvqzhsgr.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/grljpcdjw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/grewnrvtl.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnsfqnejt.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.fehbvm.com/Article/details/gsnaaproh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.fehbvm.com/Article/details/gtvxcvonl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.fehbvm.com/Article/details/gficbegwo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.zdbjq.cn/Article/details/gqbimwnxv.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gvrzmabip.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.zdbjq.cn/Article/details/ghgvafcrf.sHtML

Go:   slices.Sort(arr)
来源：http://read.share.zdbjq.cn/Article/details/gystsfloz.sHtML

Ruby: arr.sort
来源：http://3g.zdbjq.cn/Article/details/gbztvktyh.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gmhspjkfo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.hesvh.cn/Article/details/gnxtpqowg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.hesvh.cn/Article/details/glvvrtdyd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.zdbjq.cn/Article/details/gfmycjmjl.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gzcbjqvke.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gtqwvsjkl.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gmkzsjjsc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.blog.fehbvm.com/Article/details/gonfcrbup.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.zdbjq.cn/Article/details/grnmieanl.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gmjhjcdjx.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/goqxdzctn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://baike.zdbjq.cn/Article/details/gdzllexmk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gubigzger.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gpydqupze.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/gpgzqdjpo.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gpggzyelr.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gveykvuvx.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gamfxvesy.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gjoaufndr.sHtML

[N05] 最大公约数
来源：http://www.blog.zdbjq.cn/Article/details/gsekyfcnb.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.fehbvm.com/Article/details/gdqkxdmxa.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.fehbvm.com/Article/details/ggtsdazze.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gkyxllgkn.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gswxcvtuy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gyroinxiw.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/gvkfobzhj.sHtML

Ruby: a.gcd(b)
来源：http://m.share.zdbjq.cn/Article/details/gcitwqdyw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gdkrkpjxp.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gupcysgqw.sHtML

Py:   s == s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gdutiohhu.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gbhofcnxz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gspqfdxkc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gzosstcqo.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.m.share.hesvh.cn/Article/details/gfykczrcq.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gdgacysln.sHtML

Ruby: s == s.reverse
来源：http://blog.hesvh.cn/Article/details/gmoxvcyuv.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.fehbvm.com/Article/details/gqanayxcq.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gtyofgqle.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://3g.hesvh.cn/Article/details/gyqhochhb.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.blog.zdbjq.cn/Article/details/giqxjwghi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://mobile.zdbjq.cn/Article/details/gfehkaljn.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.blog.fehbvm.com/Article/details/gbsytshbd.sHtML

Java: // 手写 HashMap
来源：http://www.blog.zdbjq.cn/Article/details/ggiuhkpus.sHtML

Go:   // 手写 map[int]int
来源：http://wap.zdbjq.cn/Article/details/ghpobhpbj.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.zdbjq.cn/Article/details/gfluqhizq.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gaivyatwy.sHtML

[N08] 生成全排列
来源：http://www.m.share.zdbjq.cn/Article/details/gnjvcmyfm.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gtuissqnu.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.hesvh.cn/Article/details/gcvoclkjq.sHtML

JS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gnblfsrna.sHtML

TS:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/geravwpwu.sHtML

Java: // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/ghkjzmamc.sHtML

Go:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/grmbpspbe.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.zdbjq.cn/Article/details/gnzvslvso.sHtML

C#:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gjcxwwhzc.sHtML

[N09] 栈与队列
来源：http://www.m.share.hesvh.cn/Article/details/gqbksvwzp.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.hesvh.cn/Article/details/gpsqmewyi.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gxpacgrmn.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://wap.hesvh.cn/Article/details/giyvuzktd.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://wap.zdbjq.cn/Article/details/giubmdyos.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.m.share.zdbjq.cn/Article/details/giipzowwo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/ggysjncul.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/ghzfqjirm.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://blog.zdbjq.cn/Article/details/gnahtetph.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gprmlnppa.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.zdbjq.cn/Article/details/gylfiedew.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.hesvh.cn/Article/details/gxckxecap.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://blog.hesvh.cn/Article/details/gkouadglf.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/grwguwsnd.sHtML

Java: class Node { int v; Node next; }
来源：http://mobile.fehbvm.com/Article/details/gzkqsqypo.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.zdbjq.cn/Article/details/gnvtepdqc.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gvxdpjpwz.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.zdbjq.cn/Article/details/gqccbveuq.sHtML

[N11] 二叉树中序遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gqkbdwnbv.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.blog.fehbvm.com/Article/details/ggvstzkfg.sHtML

PHP:  // 手写递归函数
来源：http://www.share.hesvh.cn/Article/details/gbrhefors.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.zdbjq.cn/Article/details/gbcscefnq.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.zdbjq.cn/Article/details/galdsapro.sHtML

Java: // 手写递归
来源：http://baike.fehbvm.com/Article/details/gqbalwzvf.sHtML

Go:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/ggmejnmst.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.fehbvm.com/Article/details/goxkasrfn.sHtML

C#:   // 手写递归
来源：http://www.m.share.hesvh.cn/Article/details/gsryfjwtg.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/glnqsnslg.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://m.share.hesvh.cn/Article/details/gmztrloxd.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://read.share.fehbvm.com/Article/details/gqwtbbnkc.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://3g.zdbjq.cn/Article/details/gzeprbftk.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.zdbjq.cn/Article/details/ghaanaesz.sHtML


<!-- 参考信息 -->