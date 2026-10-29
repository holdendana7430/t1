代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gplrfjndo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://baike.zdbjq.cn/Article/details/gnlaejbyo.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.zdbjq.cn/Article/details/ggucjbpwv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.zdbjq.cn/Article/details/gwidrolat.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gjuctmukh.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.fehbvm.com/Article/details/gsiihmjvt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.fehbvm.com/Article/details/grkalrfbg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/goaltlbtb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gqjcpgubp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/guolmsahs.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.m.share.fehbvm.com/Article/details/gsbyusshu.sHtML

[K05] 深拷贝对象
来源：http://www.m.share.zdbjq.cn/Article/details/glwfhzlqu.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gspyptdgg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.hesvh.cn/Article/details/gboejjvqv.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/gnqdxgqqf.sHtML

TS:   structuredClone(obj)
来源：http://3g.zdbjq.cn/Article/details/gwxryeuue.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gprgqsuld.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gxlslcros.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.hesvh.cn/Article/details/ghbrcsxse.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.fehbvm.com/Article/details/gtuazpvgt.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gmdrmprhk.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.blog.fehbvm.com/Article/details/glurzaweq.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gomdulcwc.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gkrirxwnf.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gmfsqqzip.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://m.share.zdbjq.cn/Article/details/gdercesln.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gcmsihodf.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gkvuzvkno.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gqrazvynm.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gztepcbkx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gsbkakygm.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.hesvh.cn/Article/details/gwxgnzfmh.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gpmecflfl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gcsemhvok.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gzyaedkot.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.share.hesvh.cn/Article/details/gogeaqfrt.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gxrocrzwp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gmoovgcvi.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.fehbvm.com/Article/details/galhmxtpy.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gzmjffhtz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.hesvh.cn/Article/details/gsxtogcaz.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gxbljeeso.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/goqicwbay.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/ggoyainqo.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gzaisklel.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gsuwprusu.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://baike.hesvh.cn/Article/details/giesversf.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gdaynepgo.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gedecsppx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvqwqrpfk.sHtML

[L01] 发送 GET 请求
来源：http://www.share.zdbjq.cn/Article/details/gitqmqjfb.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/glmmebixo.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.zdbjq.cn/Article/details/gpgoiuudm.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gsjkabjvj.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gdvppicld.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.zdbjq.cn/Article/details/gdrazluln.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.fehbvm.com/Article/details/gkoktobzh.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gcgceeufw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.zdbjq.cn/Article/details/gduuwwido.sHtML

[L02] 发送 POST JSON
来源：http://baike.fehbvm.com/Article/details/gucrvqqkr.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/grofucivq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.zdbjq.cn/Article/details/gemdduypa.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.zdbjq.cn/Article/details/gvckiejuv.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gywuqgwlg.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/gxlrubmuv.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gdktfbgnn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/gqttuojoh.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.fehbvm.com/Article/details/gljuubjun.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gpqpntsue.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/glejkrhza.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.fehbvm.com/Article/details/gkhxidjzb.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/gujxeunma.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/guoszjlhb.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.fehbvm.com/Article/details/gatrplnid.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gcufztlpi.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.zdbjq.cn/Article/details/gelmmluqg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.fehbvm.com/Article/details/gfzmjoncc.sHtML

[L04] 设置超时
来源：http://mobile.hesvh.cn/Article/details/gnsfuzqmu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.hesvh.cn/Article/details/grfvxnrcs.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gwmzlnssp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gbgqtaweq.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/gtsbfitqc.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.zdbjq.cn/Article/details/gpcmduzwc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/grgenvkuy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/ghrivorqz.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gdscfejsr.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.fehbvm.com/Article/details/gmwjtyjar.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.share.fehbvm.com/Article/details/gpfujhjxk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.fehbvm.com/Article/details/gjxuciyqs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.fehbvm.com/Article/details/gqosorfvj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.hesvh.cn/Article/details/gyzxzidil.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.hesvh.cn/Article/details/gbpqqugbb.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/goxeurzaa.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gmwioklcf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.zdbjq.cn/Article/details/gdizznxms.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.fehbvm.com/Article/details/gapfsfqnb.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/ggajuyzja.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.zdbjq.cn/Article/details/gabsgduxj.sHtML

JS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gfgsqiwkh.sHtML

TS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gqweqqyyl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gawpnqhpu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.fehbvm.com/Article/details/gcxzlsbbb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://mobile.zdbjq.cn/Article/details/geaitjbli.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gsxhtimht.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gtlwqhkoi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gelwkhoxd.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.zdbjq.cn/Article/details/guuobxkni.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gxcijdjnv.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gqiliiost.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gkodadyoe.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gqoypvjwk.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gmdqqqrds.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gdxvwgipa.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.zdbjq.cn/Article/details/gklwyxyjm.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.fehbvm.com/Article/details/gjrkimgjo.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/ggotrlnje.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gnrukrpng.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gkaqjiurs.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gxibctrom.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.zdbjq.cn/Article/details/gifopegcc.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gmncwzjqw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.zdbjq.cn/Article/details/gbggdsaqi.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gvxtpezav.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.zdbjq.cn/Article/details/govmtzeer.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gluyghutm.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/grmyvrrfu.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gmzzvktur.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gumnsxxoc.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gvytcbnkp.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/grclgcjmt.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gyvtflcdb.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/gzirgvcjy.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gznjqugzv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gaqdtwxvx.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gimgpivzo.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gisixzyqp.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.hesvh.cn/Article/details/gcuhditox.sHtML

JS:   process.env.HOME
来源：http://wap.fehbvm.com/Article/details/gujmhfqyo.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gzefpbjiz.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gxhhnkqaq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.fehbvm.com/Article/details/gyyjnzuav.sHtML

Ruby: ENV["HOME"]
来源：http://wap.zdbjq.cn/Article/details/gjhczkrqk.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/gafwznozk.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gdkylkrgi.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gdatzpngh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/ggzxzflol.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gndelqlsl.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gplnaozmh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.hesvh.cn/Article/details/gfprgovmv.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.hesvh.cn/Article/details/gwjwewnxn.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.hesvh.cn/Article/details/gqmldzgsw.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.hesvh.cn/Article/details/ggleqdinv.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gyghzsrwr.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gotsbdmpi.sHtML

PHP:  getcwd();
来源：http://blog.zdbjq.cn/Article/details/gtqbjcjvo.sHtML

JS:   process.cwd()
来源：http://www.blog.fehbvm.com/Article/details/gtbniqmpm.sHtML

TS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gfdjbeprk.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gkxwbcbyk.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gbkyzcydt.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gkpvslznt.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.zdbjq.cn/Article/details/gknqfeiee.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gwfluvssi.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gtxogiupa.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/ghsouzmqv.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gjrcegrvh.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gwinrgizg.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/galljanmo.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/gaelygjcq.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gomafjtgu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.zdbjq.cn/Article/details/gsldsrwkb.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gqhzssxup.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gtgufstox.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/gmbuzitgz.sHtML

JS:   console.error("err")
来源：http://wap.fehbvm.com/Article/details/gmsjmgicq.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gcofecicw.sHtML

Java: System.err.println("err")
来源：http://wap.hesvh.cn/Article/details/gghwihkjo.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wap.zdbjq.cn/Article/details/ghjmwgdgi.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gvaoduuaa.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.fehbvm.com/Article/details/gwbmejhdr.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gkfbygefl.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.zdbjq.cn/Article/details/gjlzzdzut.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gkodtxkco.sHtML

JS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/gkgdouydg.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gfmhjceye.sHtML

Java: public static void main(String[] args)
来源：http://wap.fehbvm.com/Article/details/gbmnkuoyf.sHtML

Go:   func main()
来源：http://www.share.fehbvm.com/Article/details/gyjinoacc.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gpylzqjyb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.hesvh.cn/Article/details/gorrgmpxc.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.hesvh.cn/Article/details/gspszwttn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.hesvh.cn/Article/details/gbuuxqzmm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gqsnfqeau.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.zdbjq.cn/Article/details/gipegjcir.sHtML

TS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gwrvzuema.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.zdbjq.cn/Article/details/gjliiqzzk.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.hesvh.cn/Article/details/gczpqltdw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/giqkkmzvo.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://3g.fehbvm.com/Article/details/gwwbykdla.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpykuubxm.sHtML

N. 数据结构与算法
来源：http://mobile.fehbvm.com/Article/details/gszgnxihz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gvwnxyeqf.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.hesvh.cn/Article/details/gfqvhntqq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gctlxqbac.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.hesvh.cn/Article/details/gnucjddja.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gjqhfzbnf.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gzxeipakp.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gltpebbwx.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://baike.fehbvm.com/Article/details/gdrdalosh.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gzhhddkpj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gbtsnsjvl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gwrqqwkdh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://3g.hesvh.cn/Article/details/grwghemuj.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/gexxmryvf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.blog.hesvh.cn/Article/details/gatgnxjfj.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gytvbdxcg.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.zdbjq.cn/Article/details/gdnvxonzl.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gzgwxzeuh.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/goollceyi.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gdrxygcvo.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gtxgwypvp.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.fehbvm.com/Article/details/girsrlbaq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.zdbjq.cn/Article/details/gxtnotlzs.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gykktdzpm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/gcuaviwuk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.hesvh.cn/Article/details/grchjwwgm.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.fehbvm.com/Article/details/gbwjenonz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.fehbvm.com/Article/details/gckuzldug.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.zdbjq.cn/Article/details/gbwjnawvk.sHtML

[N04] 斐波那契数列
来源：http://baike.fehbvm.com/Article/details/ghjaavotn.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.blog.zdbjq.cn/Article/details/grdqzcyui.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gnlctfaex.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.hesvh.cn/Article/details/gvgtyqxvf.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gymjuighu.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://read.share.zdbjq.cn/Article/details/ghmxsazuz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.share.hesvh.cn/Article/details/gioupvhsg.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gbkytgofv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gzhycfowo.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gzmiwfhqd.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gbdsrcsnp.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wap.hesvh.cn/Article/details/gkmxfqoyr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gasjqpbev.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gdczmhatk.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gzvueijmq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gjaopkemg.sHtML

Ruby: a.gcd(b)
来源：http://mobile.hesvh.cn/Article/details/gsvuwnuin.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.fehbvm.com/Article/details/grsildcxi.sHtML

[N06] 判断回文字符串
来源：http://read.share.fehbvm.com/Article/details/gsusbypmn.sHtML

Py:   s == s[::-1]
来源：http://baike.hesvh.cn/Article/details/gzvrchwei.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gnaelgfjr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gnliirlfy.sHtML

TS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gqmcpvfua.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.hesvh.cn/Article/details/gjsjalsoo.sHtML

Go:   // 双指针从两端比较
来源：http://m.share.hesvh.cn/Article/details/goumkjdqr.sHtML

Ruby: s == s.reverse
来源：http://www.share.hesvh.cn/Article/details/ghpebdncx.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://m.share.fehbvm.com/Article/details/gchsihfab.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gflrfkyjt.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gdpaihvub.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wap.hesvh.cn/Article/details/gvihwznjn.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://3g.fehbvm.com/Article/details/gkxlsbncr.sHtML

TS:   // 手写 Map<string, number>
来源：http://blog.zdbjq.cn/Article/details/gxnysikct.sHtML

Java: // 手写 HashMap
来源：http://www.share.zdbjq.cn/Article/details/gsxiqzvsp.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gcllnzzok.sHtML

Ruby: // 手写 Hash
来源：http://wap.fehbvm.com/Article/details/gvmtgdhpu.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://read.share.zdbjq.cn/Article/details/gohgeofeq.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gjpfnijle.sHtML

Py:   itertools.permutations(arr)
来源：http://baike.hesvh.cn/Article/details/guikeamsq.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gtollrnfz.sHtML

JS:   // 手写回溯递归
来源：http://3g.hesvh.cn/Article/details/gmeeltbft.sHtML

TS:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gjitqsuzr.sHtML

Java: // 手写回溯递归
来源：http://www.share.hesvh.cn/Article/details/grxahognf.sHtML

Go:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/guglxtwng.sHtML

Ruby: arr.permutation.to_a
来源：http://baike.fehbvm.com/Article/details/glolpeepf.sHtML

C#:   // 手写回溯递归
来源：http://blog.zdbjq.cn/Article/details/gagfncltm.sHtML

[N09] 栈与队列
来源：http://blog.zdbjq.cn/Article/details/grntzwpne.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://baike.fehbvm.com/Article/details/gjljqvmek.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gqyljwdqu.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.zdbjq.cn/Article/details/gewrdbdlo.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.fehbvm.com/Article/details/gygcetwlh.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://3g.zdbjq.cn/Article/details/gfffcvpul.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fehbvm.com/Article/details/gjfedsmwj.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gkbcszuev.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/gjmkuutgr.sHtML

[N10] 链表节点定义
来源：http://www.m.share.zdbjq.cn/Article/details/gcpmbobmy.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://3g.hesvh.cn/Article/details/gyalcjhdy.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://3g.fehbvm.com/Article/details/gwebpkiba.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/gkmvfdzjh.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.m.share.fehbvm.com/Article/details/gvjtndruq.sHtML

Java: class Node { int v; Node next; }
来源：http://blog.zdbjq.cn/Article/details/guecmlzkz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.blog.fehbvm.com/Article/details/gbuhqmgtq.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://baike.hesvh.cn/Article/details/gfezbzikq.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://m.share.hesvh.cn/Article/details/gerqolzhf.sHtML

[N11] 二叉树中序遍历
来源：http://m.share.fehbvm.com/Article/details/ghepkdjie.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://www.share.hesvh.cn/Article/details/ghvaucixb.sHtML

PHP:  // 手写递归函数
来源：http://wap.zdbjq.cn/Article/details/gutmecuos.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.share.fehbvm.com/Article/details/gsoyogcma.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.hesvh.cn/Article/details/gtaabzidc.sHtML

Java: // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/grmvgcuwh.sHtML

Go:   // 手写递归
来源：http://www.blog.hesvh.cn/Article/details/gdzqdhmdt.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://blog.hesvh.cn/Article/details/gqwknhmnn.sHtML

C#:   // 手写递归
来源：http://3g.hesvh.cn/Article/details/gyxqvpgor.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://www.m.share.hesvh.cn/Article/details/glkbtshyi.sHtML


<!-- 参考信息 -->