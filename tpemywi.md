代发 wailian999

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gexabyqiy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gotgugsbq.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/ggjqolvve.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://3g.hesvh.cn/Article/details/gpwxaxvkx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://baike.zdbjq.cn/Article/details/gklepeqpz.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.fehbvm.com/Article/details/gdibravoh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/giapqbsia.sHtML

[K05] 深拷贝对象
来源：http://www.blog.fehbvm.com/Article/details/gguyrvpnb.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gjwvkvvam.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/ggocaygob.sHtML

JS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gcyogndmj.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gygbeihii.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://mobile.fehbvm.com/Article/details/gsbjisosx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gvrsiauru.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gkmlisebd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gseimuzuz.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gcbridmil.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gqsnpezur.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gafrvjfmd.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gteagjpkz.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/griwmtvka.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gmpbiiiqr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/groptbvmz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gaynpxviy.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.zdbjq.cn/Article/details/gssqqhzpp.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gqwcelyle.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gvjtsyufg.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/giqawbeon.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/giyhimggm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gvmvtcmyw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/ghauquebf.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gqwladyut.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.hesvh.cn/Article/details/ghiksxqks.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/geeorugpl.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/glrleford.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gelqpuecv.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gqgrvocwh.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/ghpdxxodp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.zdbjq.cn/Article/details/ghjajlaei.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.hesvh.cn/Article/details/gyqtcvplu.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gzaeqaoxi.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.hesvh.cn/Article/details/gleyyoqzn.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.hesvh.cn/Article/details/gnijvuzhv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxwdqejhq.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gfbkhmepd.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gjzukwxin.sHtML

[L01] 发送 GET 请求
来源：http://blog.zdbjq.cn/Article/details/gqilufque.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.share.fehbvm.com/Article/details/gusozvqkw.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/ggkojqcfw.sHtML

JS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gmwyurntl.sHtML

TS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gwmjyzxlx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.zdbjq.cn/Article/details/gdyyggnzo.sHtML

Go:   resp, err := http.Get(url)
来源：http://read.share.hesvh.cn/Article/details/gkcvjsmld.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.zdbjq.cn/Article/details/glbjahuxp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.hesvh.cn/Article/details/gzbeticwj.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gfhjlveqa.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.blog.zdbjq.cn/Article/details/ghedvzebz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/gctpamnkb.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://read.share.zdbjq.cn/Article/details/gvinwqovu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gbqlnyiob.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gwnvjdtpy.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.hesvh.cn/Article/details/gsdnsbbki.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/gherezxpm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gzxvcjvsh.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/govxwmiho.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gssptgkkt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gwohpobyi.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.hesvh.cn/Article/details/gljhnalgv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gpdzffdrk.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.zdbjq.cn/Article/details/grwfopcbk.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gksocypvj.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gpgdjbwxd.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gwxqjbysi.sHtML

[L04] 设置超时
来源：http://m.share.hesvh.cn/Article/details/ggxsimmjo.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gckuuvlgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gvcefkqwd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.fehbvm.com/Article/details/gbkdjcilm.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gtzvirlea.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gkifztujg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.hesvh.cn/Article/details/gfcqgsuod.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gfsualqvg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.fehbvm.com/Article/details/gullcgxqc.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gloxnnmlg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gqzwwzrog.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gvtskarbi.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gssqmzfpv.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/giulaplfx.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.hesvh.cn/Article/details/guzdhrhso.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gqsecvytx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.fehbvm.com/Article/details/gdpifdabl.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcnbuxfho.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.hesvh.cn/Article/details/gbomhxazl.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gxvfgazyx.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gqumhbuml.sHtML

JS:   await resp.json()
来源：http://www.m.share.fehbvm.com/Article/details/gqwxjjuzo.sHtML

TS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/ghdaxlbmz.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gihecoipu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.fehbvm.com/Article/details/graljqhsm.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.fehbvm.com/Article/details/gwvffchhd.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.zdbjq.cn/Article/details/gaazwyuqt.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gzpbgngbr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.zdbjq.cn/Article/details/gjtmeviax.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.hesvh.cn/Article/details/gycnzyzpk.sHtML

JS:   resp.ok;  resp.status
来源：http://blog.hesvh.cn/Article/details/gixwozdcx.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gvwtrpuyx.sHtML

Java: resp.statusCode()
来源：http://www.m.share.zdbjq.cn/Article/details/gewbcsoab.sHtML

Go:   resp.StatusCode
来源：http://blog.hesvh.cn/Article/details/gjtybawkp.sHtML

Ruby: resp.code.to_i
来源：http://blog.fehbvm.com/Article/details/gthjpgnvs.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gabopcdqi.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/giarjoqeh.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mobile.zdbjq.cn/Article/details/gsvuidise.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/gbnblfffn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gywlmzasm.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gkgphqhle.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.fehbvm.com/Article/details/grevympdf.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.hesvh.cn/Article/details/gzcjgjslg.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gjkoozwoh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.fehbvm.com/Article/details/grosmocnj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/grbcuqzgz.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.zdbjq.cn/Article/details/gtyyfqtio.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gysldvzeq.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gazihclsr.sHtML

Py:   sys.argv[1:]
来源：http://read.share.zdbjq.cn/Article/details/gsnyhfuem.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.zdbjq.cn/Article/details/gdzyqqhgf.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gfbnahjry.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gzcjhsylw.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gqqmjyvwq.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/ghwhiowol.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gdhvcuvjq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/gutphuhuq.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gxyyiycjl.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gnkllprpd.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gqrfxpowg.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gjhsodjky.sHtML

TS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gsvwvgvwt.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gsusavdio.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gczinxlzn.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.hesvh.cn/Article/details/grfnqycrb.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gpvshvvgs.sHtML

[M03] 执行外部命令
来源：http://wap.fehbvm.com/Article/details/gachjroyo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.fehbvm.com/Article/details/gintpyhoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.hesvh.cn/Article/details/gtlatgkcg.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gvhhyqosd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gnjurmkza.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/gaeuqamxg.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gshyytlvg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/gqnwuqmoy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.fehbvm.com/Article/details/giswamixz.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/grkxghoyk.sHtML

Py:   os.getcwd()
来源：http://read.share.hesvh.cn/Article/details/gpisbvzmh.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gmnvaynee.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gorxipztn.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gobyrwnek.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/gbmjcmesx.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gthtlfmpw.sHtML

Ruby: Dir.pwd
来源：http://wap.zdbjq.cn/Article/details/gwxmucyjs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.zdbjq.cn/Article/details/ggffwgras.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/gzqhexakw.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gdzbaggcl.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/gryzosoxw.sHtML

JS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/goxadkicy.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gbncrzssl.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/gqnhrqnph.sHtML

Go:   os.Exit(1)
来源：http://blog.hesvh.cn/Article/details/gumumiofo.sHtML

Ruby: exit 1
来源：http://blog.hesvh.cn/Article/details/gianfjcrx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/gpswkgqub.sHtML

[M06] 向标准错误输出
来源：http://read.share.zdbjq.cn/Article/details/gdixvmimq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/gmpvoabvs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/ghlwlmxxn.sHtML

JS:   console.error("err")
来源：http://3g.zdbjq.cn/Article/details/geixolwzy.sHtML

TS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gfgoeiaux.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gzurrvjmh.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gktlopeex.sHtML

Ruby: warn "err"
来源：http://blog.hesvh.cn/Article/details/gfdbputdg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gomyoieqr.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gkoaakvkv.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gsfesmgvs.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gcvnptzkm.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/galnnufsm.sHtML

TS:   require.main === module
来源：http://www.share.zdbjq.cn/Article/details/grqtkauwu.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gsursopmr.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/glodwfdhj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.zdbjq.cn/Article/details/gcqobuwcy.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/ghujfiqhv.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.hesvh.cn/Article/details/ghbyvbpfm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.fehbvm.com/Article/details/gwgckmykb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://read.share.hesvh.cn/Article/details/ghbrxhcvy.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gnjejymvj.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gaujxhgfp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/ghgwpcsyc.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gkyhathws.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gtmxpjhhg.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.zdbjq.cn/Article/details/guhvlildk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gokpbuzqk.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gwehlqhpz.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtdkxctlu.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.hesvh.cn/Article/details/gmykcdfys.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.hesvh.cn/Article/details/ggkncgphj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.zdbjq.cn/Article/details/golzlcuoi.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/ghhyvqnmh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gwmlwjwec.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/giudtknlf.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gsmeovbkj.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gdkqxmmuq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gpxutsjvd.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.fehbvm.com/Article/details/grbtftdoe.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.zdbjq.cn/Article/details/gjtmshvoy.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/ghzkwhxxp.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.fehbvm.com/Article/details/gziyhlmra.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/grcluhvth.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.fehbvm.com/Article/details/gkfxsiaff.sHtML

Go:   slices.Sort(arr)
来源：http://baike.fehbvm.com/Article/details/gmqkqcnkf.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/ghxagsjak.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.fehbvm.com/Article/details/geqtuntcg.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/ghvonmorh.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gvfhphtqn.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.m.share.zdbjq.cn/Article/details/gjztpcrye.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/giwepthnp.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/guvepxvtt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wap.hesvh.cn/Article/details/gcrwsorvf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gxhwmcakt.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.fehbvm.com/Article/details/gfyfeczop.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gclpiisaj.sHtML

[N04] 斐波那契数列
来源：http://3g.zdbjq.cn/Article/details/gdcdagulm.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gmqxoegva.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gyiauhjwm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/giklwmzbs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/glrbhkkay.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gxxrxedko.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gisqedhsk.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/gmbjlibom.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gbwpkjyuz.sHtML

[N05] 最大公约数
来源：http://3g.fehbvm.com/Article/details/grldrtfop.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.hesvh.cn/Article/details/gsiyrgxkd.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gwenijjqo.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.share.fehbvm.com/Article/details/gmfkliktq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/gokfcsmbn.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gktnajlru.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.fehbvm.com/Article/details/gcyyxamcq.sHtML

Ruby: a.gcd(b)
来源：http://wap.zdbjq.cn/Article/details/gccfqexlm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.blog.hesvh.cn/Article/details/gmekfymhw.sHtML

[N06] 判断回文字符串
来源：http://baike.fehbvm.com/Article/details/gdjqkkvtu.sHtML

Py:   s == s[::-1]
来源：http://blog.zdbjq.cn/Article/details/galmquizj.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.hesvh.cn/Article/details/gztdeqkzz.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/ggikvcpac.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gjboaciln.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gygfgokmw.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.fehbvm.com/Article/details/gdxmrbrkr.sHtML

Ruby: s == s.reverse
来源：http://3g.zdbjq.cn/Article/details/gtkmcofut.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/getmotlnd.sHtML

[N07] 两数之和（返回下标）
来源：http://read.share.fehbvm.com/Article/details/geuyizzws.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.blog.hesvh.cn/Article/details/gegjebfax.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.m.share.hesvh.cn/Article/details/gpsuvceur.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.hesvh.cn/Article/details/gcehtimsk.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/gyhwvdgod.sHtML

Java: // 手写 HashMap
来源：http://read.share.hesvh.cn/Article/details/glvleyvzz.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.zdbjq.cn/Article/details/gsvpgtxgl.sHtML

Ruby: // 手写 Hash
来源：http://www.blog.fehbvm.com/Article/details/ggfcuqdtw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.zdbjq.cn/Article/details/goybsoyfx.sHtML

[N08] 生成全排列
来源：http://www.share.hesvh.cn/Article/details/gpozqdwap.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gikdymlgf.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gqqsskxnf.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gmfkflfxq.sHtML

TS:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gunvylvph.sHtML

Java: // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/ghgyodnpk.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gofdktfgf.sHtML

Ruby: arr.permutation.to_a
来源：http://www.share.hesvh.cn/Article/details/gcpwnornl.sHtML

C#:   // 手写回溯递归
来源：http://3g.fehbvm.com/Article/details/gvzwzlnfc.sHtML

[N09] 栈与队列
来源：http://m.share.fehbvm.com/Article/details/gbnymezyb.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.fehbvm.com/Article/details/gkaxsiqsx.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://mobile.fehbvm.com/Article/details/gqmxwkzbz.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.share.hesvh.cn/Article/details/goqzwdtwu.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://www.blog.zdbjq.cn/Article/details/gzrjhtgny.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/ggsbbtcey.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://read.share.hesvh.cn/Article/details/gpemqyesp.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gwyrdbyyg.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://wap.fehbvm.com/Article/details/gfuutcagh.sHtML

[N10] 链表节点定义
来源：http://m.share.hesvh.cn/Article/details/gepbppdvh.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.zdbjq.cn/Article/details/gpywcwfkl.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://read.share.zdbjq.cn/Article/details/gvsvjsknc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://www.share.zdbjq.cn/Article/details/gwqrsnwpl.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://wap.hesvh.cn/Article/details/gigapxlhb.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gljmkoscs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.share.fehbvm.com/Article/details/glzzoaftp.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.blog.fehbvm.com/Article/details/golnpxcrd.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://www.share.fehbvm.com/Article/details/gnkofvyow.sHtML

[N11] 二叉树中序遍历
来源：http://www.blog.hesvh.cn/Article/details/gpnarjyae.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.hesvh.cn/Article/details/gxktekkjy.sHtML

PHP:  // 手写递归函数
来源：http://mobile.hesvh.cn/Article/details/gxryrvezv.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://3g.zdbjq.cn/Article/details/gjyuqdian.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.hesvh.cn/Article/details/gorerekzk.sHtML

Java: // 手写递归
来源：http://read.share.fehbvm.com/Article/details/gymnbyeaf.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/goxpioawn.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.zdbjq.cn/Article/details/gfhjuvict.sHtML

C#:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/gyuaxgnwz.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://wap.fehbvm.com/Article/details/gbusfyusn.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.zdbjq.cn/Article/details/gzubbdumk.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://mobile.fehbvm.com/Article/details/gizdghzhx.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.hesvh.cn/Article/details/gjngalyvs.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://mobile.hesvh.cn/Article/details/gxwyaolxs.sHtML


<!-- 参考信息 -->