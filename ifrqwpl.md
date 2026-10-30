代发 wailian999

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gtpzxezkp.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/gpolyzhrz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/ghoutucjb.sHtML

JS:   JSON.parse(s)
来源：http://read.share.hesvh.cn/Article/details/guhtymxfm.sHtML

TS:   JSON.parse(s)
来源：http://m.share.zdbjq.cn/Article/details/gximhmvas.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.fehbvm.com/Article/details/gdbovvsdh.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.hesvh.cn/Article/details/gghhwmcyv.sHtML

Ruby: JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/govfchgpp.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.hesvh.cn/Article/details/gwlayvxaa.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gevncabrs.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gszlmgeic.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gglpjlgnm.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.fehbvm.com/Article/details/gqbyrjuys.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://baike.hesvh.cn/Article/details/gelvjtmcv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gmagqvoxs.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.hesvh.cn/Article/details/gejpdwwrg.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.zdbjq.cn/Article/details/gjqskksqp.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.zdbjq.cn/Article/details/gvsdrmxcf.sHtML

[K04] 读取 JSON 文件
来源：http://3g.fehbvm.com/Article/details/grnwzfpac.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gyafzryjp.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.hesvh.cn/Article/details/gdosuzmdp.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gtysauakn.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.zdbjq.cn/Article/details/gvfjrzdoy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gnmhlpmrh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gcwmzbhlx.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gbtexxmew.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gwtgrcvnj.sHtML

[K05] 深拷贝对象
来源：http://m.share.fehbvm.com/Article/details/gywpckcqj.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.fehbvm.com/Article/details/gdqqzchsz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://mobile.zdbjq.cn/Article/details/gzssgryoo.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/guxdgjakj.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gzuiyxtim.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gjbufhqrq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/gpbanderf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gtbmzpqut.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.share.fehbvm.com/Article/details/ggbenmlne.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gvdbenewh.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.zdbjq.cn/Article/details/gcndusojj.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gatguojzq.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.hesvh.cn/Article/details/gzdjowjzn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.fehbvm.com/Article/details/glvslwazc.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.hesvh.cn/Article/details/gliatebhi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gobccilbj.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gtgdlskit.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gogmgghnh.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gtqvtqong.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gqdwunuex.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gmneeizxu.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gxhuofeth.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/ghlzexngs.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grzvqnabh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gtebbziac.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gudxonpoj.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gwacozrec.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/grfqwpnif.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.zdbjq.cn/Article/details/gemfapqlf.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gfttjzfgc.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gcalsrrdg.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gtskjkdid.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gcsoqqoky.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gvzsnbzfb.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gsbkiqliy.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gimjzvbpz.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/guccuraeh.sHtML

L. 网络请求
来源：http://www.m.share.hesvh.cn/Article/details/gdrycfkto.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gywiijfwx.sHtML

[L01] 发送 GET 请求
来源：http://www.share.fehbvm.com/Article/details/gcxojtjys.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.zdbjq.cn/Article/details/gqslmprsr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/gfzrnujlx.sHtML

JS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/guxzkivhn.sHtML

TS:   await fetch(url)
来源：http://blog.fehbvm.com/Article/details/ggwroxojn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.m.share.fehbvm.com/Article/details/glraypqze.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.hesvh.cn/Article/details/gjkvipimp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.hesvh.cn/Article/details/gxguajtoj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/gwhztbhww.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gpudilncm.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gsxomsqmq.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/glzydfnop.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gwwegeoeh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gaenajkbj.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.blog.hesvh.cn/Article/details/gssrdfveq.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://baike.hesvh.cn/Article/details/glpsbjjcu.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.zdbjq.cn/Article/details/getoxebzm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.fehbvm.com/Article/details/gzupqtwjd.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/goprqverx.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gkpgzwsvi.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/goylebuzu.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gllursdpr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.hesvh.cn/Article/details/gelxwtrba.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gtrairysg.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gvreldicl.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.hesvh.cn/Article/details/gxrcgwuea.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://read.share.hesvh.cn/Article/details/gojqnxxly.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gtkuhiine.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gqjcvtdxm.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.hesvh.cn/Article/details/guxnswxiz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/glpppkgwl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gujkavezy.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/gmjeyxgxn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.fehbvm.com/Article/details/gfwcvzkrm.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gwjibwqef.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.zdbjq.cn/Article/details/gxcmojdkq.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gxamcehih.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gavjjtqkz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gogggaygr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/gbmfmzfcx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/gmlkozfua.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gyqcvrdua.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/gibxkqsfh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/grykildqd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ggvpwrauh.sHtML

[L06] 解析响应为 JSON
来源：http://blog.zdbjq.cn/Article/details/gseylpcog.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gojbcptry.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.hesvh.cn/Article/details/glkrddcmq.sHtML

JS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/guttmogsv.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gsfjqtujy.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.fehbvm.com/Article/details/gvpvyrdtc.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.fehbvm.com/Article/details/gobuwbevt.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/glefxcucu.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.blog.fehbvm.com/Article/details/gdfkhveok.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gkcncazzi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gguyjibvm.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.zdbjq.cn/Article/details/gcupooomj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.fehbvm.com/Article/details/gtcfxmobl.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.zdbjq.cn/Article/details/gmhstedup.sHtML

Java: resp.statusCode()
来源：http://wap.hesvh.cn/Article/details/grjkdqxft.sHtML

Go:   resp.StatusCode
来源：http://www.blog.hesvh.cn/Article/details/gfcvosmui.sHtML

Ruby: resp.code.to_i
来源：http://baike.hesvh.cn/Article/details/gogfsdjxk.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/guxoahiay.sHtML

[L08] 并发请求多个地址
来源：http://read.share.hesvh.cn/Article/details/guaowiwmw.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.fehbvm.com/Article/details/gqbzmbvfc.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.hesvh.cn/Article/details/gruuojzuj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gqufhkrcz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gvavvkdhk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.fehbvm.com/Article/details/gxkpprvfp.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gloqeffch.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gnxjvdujy.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.hesvh.cn/Article/details/garlkfvsc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxbyufqkl.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gtfgdsphz.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/grahufcxb.sHtML

[M01] 读取命令行参数
来源：http://3g.zdbjq.cn/Article/details/golstvrri.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.zdbjq.cn/Article/details/gghtjvalz.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gxgastcsb.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gckxfdbbd.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gdkjephuv.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gmzmicnzj.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gmeynugsc.sHtML

Ruby: ARGV
来源：http://www.share.hesvh.cn/Article/details/gywotsqry.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.hesvh.cn/Article/details/gwasddpam.sHtML

[M02] 读取环境变量
来源：http://m.share.hesvh.cn/Article/details/grdfhyynk.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gwuwchmsm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/grcbumabq.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gxsbiogph.sHtML

TS:   process.env.HOME
来源：http://www.share.hesvh.cn/Article/details/gxiritjho.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/gyryjjjdw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gncgcjsbb.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gcdspdlef.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.hesvh.cn/Article/details/gjlxgyjtp.sHtML

[M03] 执行外部命令
来源：http://baike.zdbjq.cn/Article/details/gmgcpwrkp.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.fehbvm.com/Article/details/gfbanirvo.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://3g.hesvh.cn/Article/details/gkqjcouol.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.fehbvm.com/Article/details/gfjjdjipc.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gncsxrlyi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gfzlvenow.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.hesvh.cn/Article/details/gthiolopl.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.fehbvm.com/Article/details/ggzgcucgn.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.fehbvm.com/Article/details/gebnlkpak.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.zdbjq.cn/Article/details/ghxyprhwo.sHtML

Py:   os.getcwd()
来源：http://mobile.fehbvm.com/Article/details/gtbnoheex.sHtML

PHP:  getcwd();
来源：http://www.blog.hesvh.cn/Article/details/gkjshzbpp.sHtML

JS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gxwfrytds.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gsprozuuw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gkvikxovu.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gidydkbvi.sHtML

Ruby: Dir.pwd
来源：http://read.share.zdbjq.cn/Article/details/ghgwxlidm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.share.hesvh.cn/Article/details/gavfeehss.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/ghyofcpbt.sHtML

Py:   sys.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gakpmogqq.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gjxxquhqe.sHtML

JS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/glhnjpihy.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/gfghrydlo.sHtML

Java: System.exit(1)
来源：http://3g.zdbjq.cn/Article/details/gkmrqzord.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gxhmipycb.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/grvnwiatt.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.m.share.hesvh.cn/Article/details/gsvpprjpx.sHtML

[M06] 向标准错误输出
来源：http://wap.hesvh.cn/Article/details/gohvgfjsd.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.zdbjq.cn/Article/details/gmbpfucrb.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/gmrjdmuil.sHtML

JS:   console.error("err")
来源：http://3g.fehbvm.com/Article/details/gkrprbrxh.sHtML

TS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/gypmnhicu.sHtML

Java: System.err.println("err")
来源：http://baike.zdbjq.cn/Article/details/glmvnemvq.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gmxeusbyq.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gazaytxjt.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.hesvh.cn/Article/details/gfjevuvqz.sHtML

[M07] 判断是否为主入口
来源：http://m.share.hesvh.cn/Article/details/gsrtqaxrg.sHtML

Py:   if __name__ == "__main__":
来源：http://mobile.fehbvm.com/Article/details/guoisebqr.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.fehbvm.com/Article/details/gkevihejg.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gbfqiosyz.sHtML

TS:   require.main === module
来源：http://www.share.hesvh.cn/Article/details/ghvsuvhft.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.hesvh.cn/Article/details/gsalhlgxi.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gqgzfzlya.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.hesvh.cn/Article/details/gnmzjkihz.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/gdvlajkpl.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/ghztvnkgh.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.fehbvm.com/Article/details/gkeigxyxp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.hesvh.cn/Article/details/gyvbwcybx.sHtML

JS:   process.platform;  process.version
来源：http://3g.fehbvm.com/Article/details/ghwhblhgu.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gjvoxxsla.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/giicyjyes.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.zdbjq.cn/Article/details/gqufmcggg.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.zdbjq.cn/Article/details/gboakmjgk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gbaepvhpf.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gelrusycr.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gzykgvsol.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gadpvgvav.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gwkkarojh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gdijsswqp.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://m.share.zdbjq.cn/Article/details/guzwekmbg.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gcrtgxbtx.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gersdsggt.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.zdbjq.cn/Article/details/gvnbovdgo.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.fehbvm.com/Article/details/gxwidyzdr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/gxfcsfccq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gravcowew.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://m.share.hesvh.cn/Article/details/gmfzijeba.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.fehbvm.com/Article/details/gzuqtbmaz.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/glqjbybzb.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gaamxglex.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.hesvh.cn/Article/details/gphphmswj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.share.fehbvm.com/Article/details/glxdwfgpv.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/glhyksgrv.sHtML

Ruby: arr.sort
来源：http://mobile.zdbjq.cn/Article/details/gvwqwvcuz.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://3g.hesvh.cn/Article/details/gupfwbdhs.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.zdbjq.cn/Article/details/gusxtsbgx.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://3g.fehbvm.com/Article/details/gkgtsfjpb.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.fehbvm.com/Article/details/gwufdpnsy.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gychrwipe.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.m.share.fehbvm.com/Article/details/ghrlgfyqq.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.zdbjq.cn/Article/details/gzjmvqcri.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gjirhywfa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.fehbvm.com/Article/details/gkwhnjhyo.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://mobile.hesvh.cn/Article/details/gxiytufpu.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gdisoiqrv.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://blog.fehbvm.com/Article/details/ggobxkjvj.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gmgfdntra.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.zdbjq.cn/Article/details/gyjjunkyz.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/gqtgqadii.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gcgfrwqzz.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gninuhdwy.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.zdbjq.cn/Article/details/grnciotui.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gvvsljbfs.sHtML

[N05] 最大公约数
来源：http://www.share.zdbjq.cn/Article/details/gyqbtfgcc.sHtML

Py:   math.gcd(a, b)
来源：http://blog.fehbvm.com/Article/details/gwkafmvbx.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.m.share.hesvh.cn/Article/details/ggdhltgik.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://read.share.fehbvm.com/Article/details/guoxhnune.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.fehbvm.com/Article/details/gqwuffbpv.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.fehbvm.com/Article/details/gdvmcxfcr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://baike.fehbvm.com/Article/details/gkzooqkqa.sHtML

Ruby: a.gcd(b)
来源：http://www.share.zdbjq.cn/Article/details/gnoweemcw.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gedjsnkrr.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gcmtrprbh.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gpwxlavqh.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gdqfcdgnf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/golxrzrbm.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gpmpoxghs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://3g.fehbvm.com/Article/details/gkdckmgzl.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.fehbvm.com/Article/details/grqwzytjr.sHtML

Ruby: s == s.reverse
来源：http://www.share.zdbjq.cn/Article/details/gzulzjsuo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/ghpowzoer.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.fehbvm.com/Article/details/grruclobw.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gmtpjehlq.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://baike.hesvh.cn/Article/details/gwhrxcpuw.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.m.share.fehbvm.com/Article/details/grzvpctpw.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/gizmngqzd.sHtML

Java: // 手写 HashMap
来源：http://baike.zdbjq.cn/Article/details/gnekeyolp.sHtML

Go:   // 手写 map[int]int
来源：http://wap.fehbvm.com/Article/details/gortbtimz.sHtML

Ruby: // 手写 Hash
来源：http://mobile.fehbvm.com/Article/details/gudbsqser.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://m.share.fehbvm.com/Article/details/gtiiesbmv.sHtML

[N08] 生成全排列
来源：http://www.share.fehbvm.com/Article/details/gpedwpkpi.sHtML

Py:   itertools.permutations(arr)
来源：http://blog.hesvh.cn/Article/details/gydnfeiim.sHtML

PHP:  // 手写递归交换
来源：http://mobile.zdbjq.cn/Article/details/gvplwvrfb.sHtML

JS:   // 手写回溯递归
来源：http://m.share.fehbvm.com/Article/details/gnbjczvqo.sHtML

TS:   // 手写回溯递归
来源：http://3g.zdbjq.cn/Article/details/gyfkbwelr.sHtML

Java: // 手写回溯递归
来源：http://baike.hesvh.cn/Article/details/gcgfmjszm.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.zdbjq.cn/Article/details/gxfxxeeyy.sHtML

Ruby: arr.permutation.to_a
来源：http://mobile.zdbjq.cn/Article/details/gsmcwarjz.sHtML

C#:   // 手写回溯递归
来源：http://wap.zdbjq.cn/Article/details/gpyobxtlj.sHtML

[N09] 栈与队列
来源：http://baike.hesvh.cn/Article/details/gfvqpbgpq.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.zdbjq.cn/Article/details/guqtpokwy.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gcjqiansd.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://mobile.zdbjq.cn/Article/details/grninlxto.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.zdbjq.cn/Article/details/giviwxvtu.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wap.fehbvm.com/Article/details/gnhcziozn.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.m.share.fehbvm.com/Article/details/gwgxgbzyn.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wap.zdbjq.cn/Article/details/gnpkqfxlx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.m.share.hesvh.cn/Article/details/gykvaagcx.sHtML

[N10] 链表节点定义
来源：http://www.blog.zdbjq.cn/Article/details/ghjtexmic.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://www.share.hesvh.cn/Article/details/gbseukisx.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://m.share.hesvh.cn/Article/details/gdkmokbfk.sHtML


<!-- 参考信息 -->