代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gvdikyvhq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://3g.zdbjq.cn/Article/details/ghdfoiois.sHtML

[K04] 读取 JSON 文件
来源：http://www.m.share.hesvh.cn/Article/details/gncnaymfv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkrtocwso.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gtutdgddi.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gxtprhmoz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.zdbjq.cn/Article/details/gsudnibda.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gkobnuatt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gmsmtxfzg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.zdbjq.cn/Article/details/ghkimtlbq.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wap.fehbvm.com/Article/details/ggytlupvp.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gzdoiqehn.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gagkzvczi.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gxpwexwza.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/ggtbcqkbd.sHtML

TS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gevficfqi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.zdbjq.cn/Article/details/gesmfkqpn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gjbfydlhn.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/glqbjacdm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gbfjppzca.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gbtzrybdx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gbtbjenar.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gynghirza.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.hesvh.cn/Article/details/gefhwbcaw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/gpxhsoxgz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.zdbjq.cn/Article/details/gofldxywr.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gbzwdzmcq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gpenzcjkm.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gfboetpqp.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/godpexwsx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gujfskkeh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.hesvh.cn/Article/details/gnvqfkoky.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gonpgdacx.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/ghexsvuir.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gfuftddqd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.fehbvm.com/Article/details/gilrbkutl.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.zdbjq.cn/Article/details/gosfhwmpa.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/grxveswnm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gupmkhqet.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/ghkzobgxk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.fehbvm.com/Article/details/ginhtickl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gkwverdhc.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/gltemseaz.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://m.share.zdbjq.cn/Article/details/gggnwaokh.sHtML

Go:   encoding/gob
来源：http://m.share.fehbvm.com/Article/details/gejawmvab.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.hesvh.cn/Article/details/gxqdrwnpq.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.fehbvm.com/Article/details/grxslxeml.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/guhldgomu.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gzdhdvifi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gzpxrtnsn.sHtML

[L01] 发送 GET 请求
来源：http://3g.zdbjq.cn/Article/details/ghypiqzso.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.hesvh.cn/Article/details/gnmlfexgn.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/guyijdsjm.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/gujopitrh.sHtML

TS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/geeieyysx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gtwrsckwx.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gktmfwvty.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.fehbvm.com/Article/details/gsiqkhxzx.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gdmyvyfbl.sHtML

[L02] 发送 POST JSON
来源：http://blog.zdbjq.cn/Article/details/glznofhkw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.hesvh.cn/Article/details/gvrfqvemh.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gblsygvbq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gchmoqrql.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gadkpbxyz.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gjfagvvsp.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gjvnpkpob.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.fehbvm.com/Article/details/ggvrotmdm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/guaqgxrfz.sHtML

[L03] 设置自定义请求头
来源：http://wap.zdbjq.cn/Article/details/gqnknhrdz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gobkluatj.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gadrbfpbw.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gvntpfflo.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gyxdecqvs.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.blog.zdbjq.cn/Article/details/gkbffzdqw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gcvpyyrcn.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gutekybyq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gvsurjfkr.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gslofhjwv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.zdbjq.cn/Article/details/gdgcjllfe.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gouuuhrbd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.zdbjq.cn/Article/details/gjqufmfgp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gdttdsibr.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/ghpowpczt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.hesvh.cn/Article/details/gkybmccis.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.fehbvm.com/Article/details/gkvkdgkln.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.fehbvm.com/Article/details/gfnipwevj.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.fehbvm.com/Article/details/gzhjsmtka.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/geshwopgu.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gozemzinb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gazcvenrb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gmpycepsh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gbuilqtvq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.fehbvm.com/Article/details/gynalwgit.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/guoqdzfkz.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.fehbvm.com/Article/details/gxqkdcfkd.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/giuosyvqz.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gdhgzpemj.sHtML

PHP:  json_decode($body, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gaaagccnr.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gaetsddls.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gpankaqwo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gldmssmbx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gkkhunxre.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.zdbjq.cn/Article/details/grfcugolf.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gpnobklau.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/grlwlosem.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.zdbjq.cn/Article/details/gvmfpcysa.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.fehbvm.com/Article/details/gjceidice.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gvvdpouac.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gfmvfrdyb.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gxffuwwjo.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gsuixjejd.sHtML

Ruby: resp.code.to_i
来源：http://mobile.hesvh.cn/Article/details/gjmzgmpxe.sHtML

C#:   (int)resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gkvykmial.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gzkqibmfu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.zdbjq.cn/Article/details/gtfsgyijt.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/glcqskyov.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/godedhwil.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gaznpxxdi.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gwtxaxwof.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gveknqccz.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.zdbjq.cn/Article/details/gxlwwqhve.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gpotykkju.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/guafgpbvc.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.hesvh.cn/Article/details/gagvoctoe.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gomwnaxkn.sHtML

[M01] 读取命令行参数
来源：http://3g.fehbvm.com/Article/details/gjhsiwdcx.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gatuatelw.sHtML

PHP:  $argv;  $argc;
来源：http://wap.zdbjq.cn/Article/details/glecbthpz.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/grwkdmawl.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gujynyjqh.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gbaiqcivx.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gglfsleck.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gprpztklb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.zdbjq.cn/Article/details/gcrdlcfcj.sHtML

[M02] 读取环境变量
来源：http://mobile.zdbjq.cn/Article/details/grtzzgpxo.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.fehbvm.com/Article/details/gwrtswcpf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.zdbjq.cn/Article/details/gkluwersf.sHtML

JS:   process.env.HOME
来源：http://mobile.zdbjq.cn/Article/details/ggfwwjats.sHtML

TS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gwhfdpspq.sHtML

Java: System.getenv("HOME")
来源：http://3g.hesvh.cn/Article/details/ghghyonva.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.fehbvm.com/Article/details/gmibbdejb.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gtlwmvugf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gdulbpmhn.sHtML

[M03] 执行外部命令
来源：http://www.m.share.hesvh.cn/Article/details/gfonaqava.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.fehbvm.com/Article/details/gdubsbnrd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.zdbjq.cn/Article/details/goyemhvxq.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gzblmwzlz.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.fehbvm.com/Article/details/gwtdzjria.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/gidmpwniu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gprcrbmdf.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/guexbdfnv.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gwvrjcert.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/gwtaoqpwj.sHtML

Py:   os.getcwd()
来源：http://mobile.zdbjq.cn/Article/details/ginsasvgb.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/grdjoblyh.sHtML

JS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gvisoopmu.sHtML

TS:   process.cwd()
来源：http://m.share.zdbjq.cn/Article/details/gqoaasuga.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.hesvh.cn/Article/details/gahkkhtox.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gnmmxcnpd.sHtML

Ruby: Dir.pwd
来源：http://www.blog.fehbvm.com/Article/details/gpzuqqqav.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.fehbvm.com/Article/details/gvdshwyuz.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gxpfatusf.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gfavjotpl.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gaeoazhuc.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/ghyfltall.sHtML

TS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/ggszjccrx.sHtML

Java: System.exit(1)
来源：http://baike.fehbvm.com/Article/details/gpbbqdeap.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gwoinpekm.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gcemchcjx.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/glmpeqlck.sHtML

[M06] 向标准错误输出
来源：http://baike.fehbvm.com/Article/details/gnpnnxxdf.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gczxenpfw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.fehbvm.com/Article/details/ghywjggft.sHtML

JS:   console.error("err")
来源：http://blog.hesvh.cn/Article/details/gsnypscyr.sHtML

TS:   console.error("err")
来源：http://wap.zdbjq.cn/Article/details/gcpyyivzp.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/gmlarqgfw.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.fehbvm.com/Article/details/gxokwotcw.sHtML

Ruby: warn "err"
来源：http://www.share.zdbjq.cn/Article/details/gbnvuqvxc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.hesvh.cn/Article/details/gmnjcnplp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/gdlgzbrby.sHtML

Py:   if __name__ == "__main__":
来源：http://read.share.zdbjq.cn/Article/details/gxjfvndvp.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.zdbjq.cn/Article/details/gmbchcavm.sHtML

JS:   require.main === module
来源：http://www.blog.hesvh.cn/Article/details/gcjjoqdhn.sHtML

TS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gtkxpdjdo.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gexowrysm.sHtML

Go:   func main()
来源：http://www.blog.fehbvm.com/Article/details/gzprgwepn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://read.share.fehbvm.com/Article/details/gptyrgrym.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gbjuilqgx.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.hesvh.cn/Article/details/gpphqigva.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/grmpjogld.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.zdbjq.cn/Article/details/gqgzzoyun.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gcgdzsynp.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/gbtdsuoix.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gtnqrpnxh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.hesvh.cn/Article/details/gbtjspvgb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.hesvh.cn/Article/details/gpslmnctl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://read.share.zdbjq.cn/Article/details/gvevfkjhl.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvtmchqcj.sHtML

N. 数据结构与算法
来源：http://www.m.share.fehbvm.com/Article/details/gkxxspzko.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gznocjesz.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/gjietibzu.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.fehbvm.com/Article/details/giqacffxw.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.zdbjq.cn/Article/details/geufrtovy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/gcznnaukg.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gabehwsan.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gihjxsyvo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdslxldom.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.m.share.zdbjq.cn/Article/details/gwvnuwxaj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gistrxdrz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gzrumjybm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.fehbvm.com/Article/details/gcvhiljjv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gonfoikyl.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.fehbvm.com/Article/details/gpcohdifp.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.zdbjq.cn/Article/details/glnxmfcil.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gmkxjemep.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gzohtwzwb.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gnsdkjqgt.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.hesvh.cn/Article/details/gasvtiukh.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.zdbjq.cn/Article/details/guqsgvotw.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gtbwaeeib.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/ggchsieia.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gxevbafza.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gveijmsdw.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gglnlhkdd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.zdbjq.cn/Article/details/gvztoygay.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gujkvvsjy.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gtjrajazx.sHtML

[N04] 斐波那契数列
来源：http://read.share.fehbvm.com/Article/details/gjhpfndnz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gyrkjheml.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gedafppnd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.fehbvm.com/Article/details/gfokncgjg.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/ggazdzzmu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://3g.zdbjq.cn/Article/details/gjtxcofwf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/ggqfigmnv.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/geawnjtjo.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gqhkduurp.sHtML

[N05] 最大公约数
来源：http://m.share.zdbjq.cn/Article/details/gzftszkap.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.fehbvm.com/Article/details/glelrzufk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.fehbvm.com/Article/details/gvmklbnih.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.zdbjq.cn/Article/details/gthnuxyvw.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/grsrplidy.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.hesvh.cn/Article/details/gnbjwujrx.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gsptraqcy.sHtML

Ruby: a.gcd(b)
来源：http://read.share.hesvh.cn/Article/details/gllvjcdil.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/grkvftzry.sHtML

[N06] 判断回文字符串
来源：http://blog.hesvh.cn/Article/details/gyjuuhead.sHtML

Py:   s == s[::-1]
来源：http://3g.hesvh.cn/Article/details/gavfthrjt.sHtML

PHP:  $s === strrev($s);
来源：http://blog.hesvh.cn/Article/details/ghzsvzeqk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnaaajpir.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gllismkum.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://blog.fehbvm.com/Article/details/goalaquyh.sHtML

Go:   // 双指针从两端比较
来源：http://baike.fehbvm.com/Article/details/guyjbubde.sHtML

Ruby: s == s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gzbdxycov.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gdfcnffwn.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.hesvh.cn/Article/details/gvmquncjq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.fehbvm.com/Article/details/gfawhgqvy.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.fehbvm.com/Article/details/gweicjsff.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gdknooljg.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.fehbvm.com/Article/details/gqhlumscv.sHtML

Java: // 手写 HashMap
来源：http://m.share.zdbjq.cn/Article/details/gxwhmwums.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gvdprmmvp.sHtML

Ruby: // 手写 Hash
来源：http://read.share.hesvh.cn/Article/details/gwvsugpqr.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gpsybhruz.sHtML

[N08] 生成全排列
来源：http://3g.hesvh.cn/Article/details/gidrhylbi.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.fehbvm.com/Article/details/gvkuvxjny.sHtML

PHP:  // 手写递归交换
来源：http://wap.zdbjq.cn/Article/details/gpiziihdk.sHtML

JS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/goukasnqo.sHtML

TS:   // 手写回溯递归
来源：http://www.share.zdbjq.cn/Article/details/gfuvigfpw.sHtML

Java: // 手写回溯递归
来源：http://baike.fehbvm.com/Article/details/grhvjjqyo.sHtML

Go:   // 手写回溯递归
来源：http://www.m.share.hesvh.cn/Article/details/gjxekcpdo.sHtML

Ruby: arr.permutation.to_a
来源：http://wap.fehbvm.com/Article/details/ghuvlvmmk.sHtML

C#:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/guzwctojx.sHtML

[N09] 栈与队列
来源：http://mobile.fehbvm.com/Article/details/giaifpuoh.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://blog.hesvh.cn/Article/details/gsyabhwjn.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.blog.fehbvm.com/Article/details/gcypzexfl.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gggdkxatg.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://blog.hesvh.cn/Article/details/gcpgbleeh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.fehbvm.com/Article/details/gtgjsprim.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gctrxpcqc.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gbynvaine.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://mobile.hesvh.cn/Article/details/gihhpllki.sHtML

[N10] 链表节点定义
来源：http://www.share.hesvh.cn/Article/details/gsgszvejt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://read.share.zdbjq.cn/Article/details/glortjmqa.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.m.share.fehbvm.com/Article/details/gxxzddbmn.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://baike.fehbvm.com/Article/details/gylnnsbyx.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://m.share.hesvh.cn/Article/details/gcfamctol.sHtML

Java: class Node { int v; Node next; }
来源：http://baike.fehbvm.com/Article/details/goyydafop.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.zdbjq.cn/Article/details/gfhyeqcxy.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.m.share.zdbjq.cn/Article/details/gnsrourvu.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://wap.zdbjq.cn/Article/details/gkgsvehrh.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.zdbjq.cn/Article/details/gxvgwqqzc.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://3g.fehbvm.com/Article/details/gcvmjdrmc.sHtML

PHP:  // 手写递归函数
来源：http://www.m.share.zdbjq.cn/Article/details/grcjlmvbc.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://baike.fehbvm.com/Article/details/giesuxrdk.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gmmdvhwbo.sHtML

Java: // 手写递归
来源：http://blog.fehbvm.com/Article/details/gokfyxhnt.sHtML

Go:   // 手写递归
来源：http://m.share.fehbvm.com/Article/details/guzspmxdd.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.hesvh.cn/Article/details/gcjugdmpo.sHtML

C#:   // 手写递归
来源：http://mobile.zdbjq.cn/Article/details/gomvgzrty.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.blog.fehbvm.com/Article/details/gmlfjoewv.sHtML


<!-- 参考信息 -->