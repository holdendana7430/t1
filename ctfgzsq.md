代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gydlsekax.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gpezzexod.sHtML

[K04] 读取 JSON 文件
来源：http://wap.zdbjq.cn/Article/details/gfoogzgke.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.fehbvm.com/Article/details/gobmoygrm.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gpjyqyoth.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gsmygfhaz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gxscekirr.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gpnanpfuu.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gspxwpwtv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gcfnpexye.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.hesvh.cn/Article/details/gsqadfmxn.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gvyawsgza.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gyuebpuvr.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.zdbjq.cn/Article/details/gjcmwjydn.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.zdbjq.cn/Article/details/ghqlhmjef.sHtML

TS:   structuredClone(obj)
来源：http://read.share.zdbjq.cn/Article/details/gxwfduwdu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gnegaysqy.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.fehbvm.com/Article/details/gykxzhjqd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/glmeiyhol.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://mobile.zdbjq.cn/Article/details/glacapjth.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gxqlenlvi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://m.share.fehbvm.com/Article/details/gkilkefbl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/ghgeuqvje.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.fehbvm.com/Article/details/gxmyebeji.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gdxgpfzul.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.hesvh.cn/Article/details/gecjftsfi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/giiytjlij.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gfdkguuph.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gjqhjmpsc.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gksgcgign.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gadrmfyeh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.zdbjq.cn/Article/details/gubujfghw.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gezxfthzd.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gwxwzvcxa.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gcpcustxc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.zdbjq.cn/Article/details/gxualcszi.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.fehbvm.com/Article/details/gyugllxux.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/ggwwjhzec.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.fehbvm.com/Article/details/gtuahnsza.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/gofbinsxr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/giwjtmhbc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/geseivlzx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gglgtbwsc.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.hesvh.cn/Article/details/gloukozme.sHtML

Go:   encoding/gob
来源：http://read.share.hesvh.cn/Article/details/gvheavmxg.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.zdbjq.cn/Article/details/gnbpssvmo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.zdbjq.cn/Article/details/gckouqhdh.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gpsqrdzkz.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gzqcafnzp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/guezbiysm.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/ghyqemvvx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gdunqkjjm.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.hesvh.cn/Article/details/gdvrmvwzg.sHtML

JS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gbboqxnlz.sHtML

TS:   await fetch(url)
来源：http://wap.fehbvm.com/Article/details/gcgoptvov.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/ganqrzyjs.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gxgeyowxy.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.zdbjq.cn/Article/details/gaookewba.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.zdbjq.cn/Article/details/gjtorfbjk.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gwtxscoyq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gsrlvhxmd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/gytheqkfv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.zdbjq.cn/Article/details/gsgagmvwr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gyyzusybm.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gqoiirsrm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.hesvh.cn/Article/details/gxiabbktt.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gdntysjop.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.hesvh.cn/Article/details/gxdtmkqfu.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/grjosbhbx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/grhpfgthy.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gsuarvper.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.fehbvm.com/Article/details/gaidmtttw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.zdbjq.cn/Article/details/ghzgcdwbq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.fehbvm.com/Article/details/gyojptnlx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.fehbvm.com/Article/details/gkbwjzdii.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gmwcoiprc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gvpicmkjx.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/geugdnktp.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.hesvh.cn/Article/details/grbojucco.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.zdbjq.cn/Article/details/gtrcimduh.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.zdbjq.cn/Article/details/gsgngypku.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/grpdtqfcy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gjckegcll.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.fehbvm.com/Article/details/givdhikcd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://3g.hesvh.cn/Article/details/goboxxxpr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gryayupar.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gyvvotrcn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gtueyuvgp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gttekistf.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://read.share.fehbvm.com/Article/details/gcpiwnpui.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gufavwkhf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mobile.fehbvm.com/Article/details/gmtfmfyxy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gckrdbvyw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mobile.fehbvm.com/Article/details/ghdssekpa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.fehbvm.com/Article/details/gfvqybkmm.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/ghhfisufx.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/giibjkkap.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.hesvh.cn/Article/details/gcmhffusv.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/grriirjok.sHtML

TS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gvsseplka.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gqdenhbow.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gqwztmkbb.sHtML

Ruby: JSON.parse(resp.body)
来源：http://m.share.hesvh.cn/Article/details/gudrfvrug.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gjwfkjmpy.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gwcorvepl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gkuajgfji.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.blog.hesvh.cn/Article/details/gxvbsgtvq.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gdkmgtigq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/ghpghpcvd.sHtML

Java: resp.statusCode()
来源：http://blog.zdbjq.cn/Article/details/gtvmwwjfr.sHtML

Go:   resp.StatusCode
来源：http://blog.zdbjq.cn/Article/details/gqdmcubbt.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gorjlcwmy.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/glopizemr.sHtML

[L08] 并发请求多个地址
来源：http://baike.zdbjq.cn/Article/details/gxlucewtc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://baike.zdbjq.cn/Article/details/gplpgcwjq.sHtML

PHP:  curl_multi_init() 系列
来源：http://mobile.zdbjq.cn/Article/details/ghzzfmnfi.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gaziqlvei.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/gmaorlaaz.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gvlnqbilp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.zdbjq.cn/Article/details/gfbcyjlae.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gciieyqfv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://m.share.zdbjq.cn/Article/details/gndrviffa.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gzujtwxlm.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gdfwhvysm.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gkjloqcwy.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gwacmcnwa.sHtML

Py:   sys.argv[1:]
来源：http://3g.fehbvm.com/Article/details/gyxvzjzim.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.hesvh.cn/Article/details/gnmnjundm.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gxdyfaqjc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.fehbvm.com/Article/details/gfckeojhw.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gegdeynnq.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gnylzcowr.sHtML

Ruby: ARGV
来源：http://www.blog.hesvh.cn/Article/details/giqqlxahi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.fehbvm.com/Article/details/gtwguitpx.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/gkocunfzi.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.fehbvm.com/Article/details/gacuwgsjc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gihpfqxqs.sHtML

JS:   process.env.HOME
来源：http://3g.fehbvm.com/Article/details/gdfwxthjb.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gzvwmshoh.sHtML

Java: System.getenv("HOME")
来源：http://blog.hesvh.cn/Article/details/gqvdkpxoq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gbsxakswp.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gwagvcdpr.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/grthhfptk.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gxfpqzodn.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gufnaoxsi.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gflpmzmug.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gnezrqnve.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://m.share.hesvh.cn/Article/details/gxnartfmf.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://baike.fehbvm.com/Article/details/gqugrcmcb.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gopcbmnhv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gshylmddg.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/ghodgcurr.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/gdudlemty.sHtML

Py:   os.getcwd()
来源：http://m.share.fehbvm.com/Article/details/gejvielau.sHtML

PHP:  getcwd();
来源：http://www.blog.fehbvm.com/Article/details/gtexuumiw.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/glkqzgotd.sHtML

TS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gzxfyudrx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.hesvh.cn/Article/details/gwxwwjyjd.sHtML

Go:   os.Getwd()
来源：http://baike.zdbjq.cn/Article/details/gkbahfgtb.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gyeoxfiwr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.hesvh.cn/Article/details/grymtnyry.sHtML

[M05] 设置退出码
来源：http://www.blog.hesvh.cn/Article/details/gresksuwf.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.hesvh.cn/Article/details/gauiklorx.sHtML

PHP:  exit(1);
来源：http://baike.zdbjq.cn/Article/details/gkjjrptzg.sHtML

JS:   process.exit(1)
来源：http://wap.fehbvm.com/Article/details/gdmannjef.sHtML

TS:   process.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/ghnfmmahr.sHtML

Java: System.exit(1)
来源：http://m.share.zdbjq.cn/Article/details/glbvprsyf.sHtML

Go:   os.Exit(1)
来源：http://wap.hesvh.cn/Article/details/gqcapiauy.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gduytvvrz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/ghbzajaxa.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gmrwgwwzj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gyrebjrxw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://read.share.hesvh.cn/Article/details/gsqpmmedk.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gnxuecqqx.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/gyvkplfqp.sHtML

Java: System.err.println("err")
来源：http://www.share.zdbjq.cn/Article/details/gsifbfymk.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.fehbvm.com/Article/details/gcztxkjzb.sHtML

Ruby: warn "err"
来源：http://blog.zdbjq.cn/Article/details/gwmiztlpl.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.zdbjq.cn/Article/details/gjinyspec.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/ggwendehx.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.zdbjq.cn/Article/details/gjkmmqlzw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.zdbjq.cn/Article/details/gtvfdnazl.sHtML

JS:   require.main === module
来源：http://www.m.share.zdbjq.cn/Article/details/gyhqgbmrn.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gfjbruaek.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.fehbvm.com/Article/details/gwjyqtcgu.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gtjduiijt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.fehbvm.com/Article/details/gwhdxtgeo.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gcyrpzfby.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gedkckete.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.fehbvm.com/Article/details/gykkuknll.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.hesvh.cn/Article/details/ghbamcanw.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/ghhjnmkyf.sHtML

TS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/golfbugod.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wap.fehbvm.com/Article/details/gykulqexp.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gsmrtbqng.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://m.share.fehbvm.com/Article/details/golldmvup.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/grgkbgpqf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gyzsplopz.sHtML

N. 数据结构与算法
来源：http://www.m.share.zdbjq.cn/Article/details/gnzmwsiks.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gwdxvjbie.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gtordkaox.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.hesvh.cn/Article/details/gummbtiuj.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gjukfoejq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/gjkadekhx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gwhmoxidc.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/ghfyiszgp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://wap.hesvh.cn/Article/details/gidhtuobq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://mobile.hesvh.cn/Article/details/gukhtqkxg.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/ghkyagwyk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/garwrfeiv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/ghddsphsu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gslqcnfqv.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.hesvh.cn/Article/details/gkelvzupf.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/geowdmzqn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.hesvh.cn/Article/details/gjjshomoe.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.fehbvm.com/Article/details/gzdshezpc.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gjwkblaqm.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/guudsbogm.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gwcdfmbpx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.fehbvm.com/Article/details/gqzaweecv.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.hesvh.cn/Article/details/ghqoeobmg.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/gjedipnzd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.fehbvm.com/Article/details/guubrciwj.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.fehbvm.com/Article/details/gethbhhtj.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://baike.zdbjq.cn/Article/details/gpxaojfwl.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.hesvh.cn/Article/details/gdczsgpif.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gewaxcljg.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.hesvh.cn/Article/details/gwdoudswu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gebibsczk.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://wap.hesvh.cn/Article/details/gmcepnosd.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/glqqcgetp.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gmemtrlyz.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gghwpwcrh.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wap.zdbjq.cn/Article/details/gffojdeuc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gkkqitgrq.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.zdbjq.cn/Article/details/gjnclykft.sHtML

[N05] 最大公约数
来源：http://baike.zdbjq.cn/Article/details/gxtgusuin.sHtML

Py:   math.gcd(a, b)
来源：http://wap.zdbjq.cn/Article/details/gyetgeowq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://baike.hesvh.cn/Article/details/gfxttvahw.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.fehbvm.com/Article/details/gxivwqiws.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.fehbvm.com/Article/details/gvplysmpi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.zdbjq.cn/Article/details/gfxbfcmty.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gmyqqsowu.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/glntkbcml.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.fehbvm.com/Article/details/gnordckta.sHtML

[N06] 判断回文字符串
来源：http://blog.zdbjq.cn/Article/details/gplqthsso.sHtML

Py:   s == s[::-1]
来源：http://wap.fehbvm.com/Article/details/gnbyiaabp.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gjrzeprbe.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gjuravcon.sHtML

TS:   s === [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gtrdywcnm.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.hesvh.cn/Article/details/gbxsxgzbx.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.hesvh.cn/Article/details/gemwtryfr.sHtML

Ruby: s == s.reverse
来源：http://3g.hesvh.cn/Article/details/gvjlayjhy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gioioidel.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.zdbjq.cn/Article/details/gyuvbwtir.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.fehbvm.com/Article/details/gufwmvnzt.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.hesvh.cn/Article/details/gvkvflcqa.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.hesvh.cn/Article/details/ghbrzxjof.sHtML

TS:   // 手写 Map<string, number>
来源：http://read.share.fehbvm.com/Article/details/gnwbdypmq.sHtML

Java: // 手写 HashMap
来源：http://m.share.hesvh.cn/Article/details/ghumxciki.sHtML

Go:   // 手写 map[int]int
来源：http://m.share.fehbvm.com/Article/details/gjumcagiz.sHtML

Ruby: // 手写 Hash
来源：http://3g.hesvh.cn/Article/details/gfeusybso.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://mobile.hesvh.cn/Article/details/gnxypcawc.sHtML

[N08] 生成全排列
来源：http://m.share.zdbjq.cn/Article/details/guvwanabe.sHtML

Py:   itertools.permutations(arr)
来源：http://wap.fehbvm.com/Article/details/gpywiynfq.sHtML

PHP:  // 手写递归交换
来源：http://mobile.hesvh.cn/Article/details/gkprnahmt.sHtML

JS:   // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gbhtkrddf.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.fehbvm.com/Article/details/gxowyjemo.sHtML

Java: // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gannzpaez.sHtML

Go:   // 手写回溯递归
来源：http://read.share.hesvh.cn/Article/details/gzmnjkfbl.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.hesvh.cn/Article/details/gnnpeibjm.sHtML

C#:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gkpfzfgpg.sHtML

[N09] 栈与队列
来源：http://m.share.zdbjq.cn/Article/details/gjinphysa.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://m.share.hesvh.cn/Article/details/gicpuaqrv.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://baike.zdbjq.cn/Article/details/gwrrdvzjp.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gsyiarhmy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.zdbjq.cn/Article/details/ggdoixdno.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://m.share.hesvh.cn/Article/details/gilictlgb.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mobile.zdbjq.cn/Article/details/gfipbreir.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fehbvm.com/Article/details/grbfpthxf.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://baike.fehbvm.com/Article/details/gezcsmnwm.sHtML

[N10] 链表节点定义
来源：http://www.m.share.fehbvm.com/Article/details/gcikcqovg.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.fehbvm.com/Article/details/guccypxaz.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.fehbvm.com/Article/details/ghpgieeum.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://read.share.hesvh.cn/Article/details/gxmamaalp.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.share.hesvh.cn/Article/details/gfltxmfbe.sHtML

Java: class Node { int v; Node next; }
来源：http://www.m.share.fehbvm.com/Article/details/gbxssvynz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://www.m.share.hesvh.cn/Article/details/ggssvqogs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://read.share.fehbvm.com/Article/details/gcwrdfwpa.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://read.share.hesvh.cn/Article/details/gubnybdat.sHtML

[N11] 二叉树中序遍历
来源：http://mobile.fehbvm.com/Article/details/gxhhvhwga.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://m.share.zdbjq.cn/Article/details/gaymlgihc.sHtML

PHP:  // 手写递归函数
来源：http://read.share.hesvh.cn/Article/details/gqtcydnqg.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.m.share.zdbjq.cn/Article/details/gfuzqysob.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://wap.hesvh.cn/Article/details/glenaglmr.sHtML

Java: // 手写递归
来源：http://3g.zdbjq.cn/Article/details/gmuuerhjm.sHtML

Go:   // 手写递归
来源：http://baike.hesvh.cn/Article/details/gxsmgamkj.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://baike.fehbvm.com/Article/details/glvrbrnlm.sHtML

C#:   // 手写递归
来源：http://www.share.hesvh.cn/Article/details/gybtyzqit.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://3g.hesvh.cn/Article/details/gkqaflmsx.sHtML


<!-- 参考信息 -->