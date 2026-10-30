代发 wailian999

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/gicmnipfn.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/gbzungkmd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://m.share.zdbjq.cn/Article/details/ggfyfcnsu.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/giciltkew.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcqhbqnxw.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/guoobrskm.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/grtonpnuk.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/geexpbjct.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gazxbslbt.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://3g.fehbvm.com/Article/details/gpqspyzsj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.zdbjq.cn/Article/details/ggpcneiby.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.share.zdbjq.cn/Article/details/gufusdjwu.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/grbnpsvyl.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gfskejyuy.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/geinqrcxb.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.zdbjq.cn/Article/details/grkoewqat.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.hesvh.cn/Article/details/gbouqawvu.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gmuotlvvt.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gyxydwzfh.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gmoyaxxqt.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/ghcpmnumq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/grnmuyuok.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.hesvh.cn/Article/details/gfmfutnhf.sHtML

[K05] 深拷贝对象
来源：http://www.share.fehbvm.com/Article/details/gcmslybjo.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.fehbvm.com/Article/details/gjyjxdhbd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/gdawutuae.sHtML

JS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/gfkbcjryv.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gkslsrhnb.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gdjiyfqbx.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.zdbjq.cn/Article/details/ghochvifr.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gxmlhfhrg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.fehbvm.com/Article/details/ghueauxfg.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gmwwsfrnr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/grisglbiw.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gumoatwpj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.fehbvm.com/Article/details/gqrakbfvs.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gdjyopvrm.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.hesvh.cn/Article/details/gjhgswjnu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gdnwoqqkq.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.zdbjq.cn/Article/details/gburmmwju.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/guerwyfjm.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gfvpqqics.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gawnwrocc.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.fehbvm.com/Article/details/gxtgubwit.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gpqkrgzmz.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/guvtucmfx.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gddnjjxfd.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.hesvh.cn/Article/details/gxrcaftyv.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gpruxxnfp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gfiwjetgc.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://baike.hesvh.cn/Article/details/gsufwsgwn.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gvteunouy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.zdbjq.cn/Article/details/gjjvsqnhg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/guzlvyqsq.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gfjzlamrx.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.zdbjq.cn/Article/details/gvdakckim.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/ghuzvniae.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gtejllquw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.hesvh.cn/Article/details/gofbvxnmd.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzvtwhsyg.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/guuznkjnv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsujgeejg.sHtML

[L01] 发送 GET 请求
来源：http://wap.fehbvm.com/Article/details/gokzeufbr.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://m.share.fehbvm.com/Article/details/gfftflkdt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wap.zdbjq.cn/Article/details/gxvfoozvp.sHtML

JS:   await fetch(url)
来源：http://wap.zdbjq.cn/Article/details/grvtvuryv.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gacwvltjq.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gsmykahen.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gkhiopaei.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://blog.fehbvm.com/Article/details/gpcoklzbu.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.fehbvm.com/Article/details/gwizgcaxh.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gfkxujuev.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/glyqoztwm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.hesvh.cn/Article/details/gspgplenl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gttrbvqal.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gfsjaknxt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.hesvh.cn/Article/details/gjvjyrwnz.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gmfualhxq.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/gxikxslpk.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/ggbefrpcn.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.zdbjq.cn/Article/details/gwnzmqpwz.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gxrqeyulr.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.zdbjq.cn/Article/details/gtqcopgor.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://m.share.zdbjq.cn/Article/details/gerdfeaof.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gkxvpjazo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gclviwhdu.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gzxrjihyz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.zdbjq.cn/Article/details/gmqrycnlk.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/genbcsqwu.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gudgkvysb.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gjrcnymfu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.blog.fehbvm.com/Article/details/gccnkjmfy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/gujuykosd.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.hesvh.cn/Article/details/gufdkqvvv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/ghrhyucfg.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gdctkyutx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.fehbvm.com/Article/details/gsrwijcov.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.zdbjq.cn/Article/details/gwuftlnhx.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gprlgibre.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.fehbvm.com/Article/details/gpcjptejl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gnbhxbbzq.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/gtlevckuj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gxmmijerw.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gguimwzof.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://3g.hesvh.cn/Article/details/gbkvqgkzt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gzawpxipe.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gcbakamkc.sHtML

[L06] 解析响应为 JSON
来源：http://wap.fehbvm.com/Article/details/goexzuhqu.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gindbsuzj.sHtML

PHP:  json_decode($body, true);
来源：http://baike.zdbjq.cn/Article/details/gmvxdhkcx.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/ghzkytzry.sHtML

TS:   await resp.json()
来源：http://3g.fehbvm.com/Article/details/geeeqfcnl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gaigfuxxx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gungkzwvq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gkamwxhuw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mobile.fehbvm.com/Article/details/gzinsjwbk.sHtML

[L07] 处理 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gsgksnqlv.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gxyxeacgx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.m.share.zdbjq.cn/Article/details/gbhnxtcfb.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.hesvh.cn/Article/details/gvumpfzpd.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gtkhpvvif.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/gxqqhyovy.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gztguwqzq.sHtML

Ruby: resp.code.to_i
来源：http://m.share.hesvh.cn/Article/details/ghtzzevog.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.zdbjq.cn/Article/details/gkvnewkmq.sHtML

[L08] 并发请求多个地址
来源：http://baike.fehbvm.com/Article/details/gnkmuybrn.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.fehbvm.com/Article/details/gljidxclb.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gmwdwipwp.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/grkmdlwbs.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gtmvovfxj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gjoevywjl.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://blog.hesvh.cn/Article/details/gxykocayt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gilonsgud.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.hesvh.cn/Article/details/gfjrorrya.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gbrlrifeg.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gtkdxortw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/ggmmkclqj.sHtML

[M01] 读取命令行参数
来源：http://mobile.hesvh.cn/Article/details/gjspabvzy.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gnoigrdje.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.zdbjq.cn/Article/details/gtttxljnp.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gzzuwcrzq.sHtML

TS:   process.argv.slice(2)
来源：http://blog.hesvh.cn/Article/details/gvoytensr.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gnjnzzhfl.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gslvkcpdc.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gffkdjfkx.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gipuffvyr.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/glkrzehqr.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gkcgpfhpv.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/ghwgezhpb.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gwfwigpeb.sHtML

TS:   process.env.HOME
来源：http://m.share.zdbjq.cn/Article/details/ghttcqgyw.sHtML

Java: System.getenv("HOME")
来源：http://wap.hesvh.cn/Article/details/ggjzrrnqc.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wap.fehbvm.com/Article/details/gpdibxhox.sHtML

Ruby: ENV["HOME"]
来源：http://www.m.share.zdbjq.cn/Article/details/gmfcdhyud.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gefoaivib.sHtML

[M03] 执行外部命令
来源：http://read.share.hesvh.cn/Article/details/gjweqgmad.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gbdiyovnj.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gompewkca.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.fehbvm.com/Article/details/gfjmzdzbr.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://mobile.zdbjq.cn/Article/details/gqzyrxhgi.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.fehbvm.com/Article/details/gcdwapnkt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://mobile.hesvh.cn/Article/details/gdhftdxmc.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://m.share.fehbvm.com/Article/details/gcuizraqo.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gnjnhxilt.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gxytzjojn.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gcpqysefy.sHtML

PHP:  getcwd();
来源：http://baike.hesvh.cn/Article/details/gfvyqngyq.sHtML

JS:   process.cwd()
来源：http://www.m.share.fehbvm.com/Article/details/gsiejpmwj.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gimtbfneq.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.hesvh.cn/Article/details/gdfyppzsn.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/giglypzht.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gvoysuevr.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gpvyszhvk.sHtML

[M05] 设置退出码
来源：http://read.share.fehbvm.com/Article/details/gryugwtku.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gwwidjypz.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gbuprxick.sHtML

JS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/gyawaghuo.sHtML

TS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ghvcpjqbn.sHtML

Java: System.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/glyrprexa.sHtML

Go:   os.Exit(1)
来源：http://m.share.fehbvm.com/Article/details/ggtcafrfj.sHtML

Ruby: exit 1
来源：http://baike.fehbvm.com/Article/details/ggiiivfwu.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/ggmitidrx.sHtML

[M06] 向标准错误输出
来源：http://www.share.hesvh.cn/Article/details/gxiyeeuhg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.hesvh.cn/Article/details/glvksrrhd.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.fehbvm.com/Article/details/gipfgukan.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/glpvygmle.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gdymwsgmf.sHtML

Java: System.err.println("err")
来源：http://m.share.hesvh.cn/Article/details/ghlvcjaev.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/gucmoonjf.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gqijarbwi.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.hesvh.cn/Article/details/gcqvijskp.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.fehbvm.com/Article/details/giwdeyuwp.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.zdbjq.cn/Article/details/gjpcshuuj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gldavtufe.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/guaupvvav.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/glsgoayxw.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gfmlldhnp.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gfarbdnui.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gehngylcb.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/gyupomerh.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/girypwpqa.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gtsbjqucp.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.hesvh.cn/Article/details/giazmbufl.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ghowyijcq.sHtML

TS:   process.platform;  process.version
来源：http://baike.fehbvm.com/Article/details/gioumvunx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://read.share.zdbjq.cn/Article/details/gzcwniaws.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/glinhztsp.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wap.zdbjq.cn/Article/details/gbxlsygsk.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.hesvh.cn/Article/details/guctzofaa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/guvkdjljg.sHtML

N. 数据结构与算法
来源：http://www.share.hesvh.cn/Article/details/gpqcabquc.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gwmpauyiw.sHtML

[N01] 二分查找（有序数组）
来源：http://www.share.zdbjq.cn/Article/details/gdunrjmto.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gqrxskqyx.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.hesvh.cn/Article/details/grnbjtehm.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gpnvnetji.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gtzwjgmya.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gksfpjaqp.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gmxuhygbb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.fehbvm.com/Article/details/glvbbmouo.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.m.share.zdbjq.cn/Article/details/gxgkvpmuc.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.hesvh.cn/Article/details/gmwbfvudh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.zdbjq.cn/Article/details/gdiwbnlnf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://3g.hesvh.cn/Article/details/gzjkvqqxo.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://blog.fehbvm.com/Article/details/gsmjhfjcd.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/giyvdeaaa.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.hesvh.cn/Article/details/gckuhqqie.sHtML

Go:   slices.Sort(arr)
来源：http://www.share.zdbjq.cn/Article/details/goypfxmkt.sHtML

Ruby: arr.sort
来源：http://wap.fehbvm.com/Article/details/gxusjqznu.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://m.share.fehbvm.com/Article/details/gfefcoywy.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/glqoepnlr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gvtheviun.sHtML

PHP:  // 递归实现，或用 usort
来源：http://mobile.fehbvm.com/Article/details/gpxkuidkt.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.fehbvm.com/Article/details/ggatcdyhn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.zdbjq.cn/Article/details/gqwyiyeyo.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.hesvh.cn/Article/details/gkkkwlkrd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.fehbvm.com/Article/details/gsxasbkxq.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gvfkbcdsr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gljlidxjh.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/ghayershs.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfquudqey.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gdcwbpiox.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gwwatirfl.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghyqrskuk.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gkzapupzf.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://read.share.zdbjq.cn/Article/details/gypkxcdhw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.hesvh.cn/Article/details/gkdxwhkpz.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gevwxuojr.sHtML

[N05] 最大公约数
来源：http://read.share.zdbjq.cn/Article/details/gvbdzdooj.sHtML

Py:   math.gcd(a, b)
来源：http://baike.fehbvm.com/Article/details/gbswmuoun.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gciowjbva.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.zdbjq.cn/Article/details/goamlrhnl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/gcswcbcwi.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.zdbjq.cn/Article/details/gyxirlelt.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.fehbvm.com/Article/details/ggydlcwsl.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.zdbjq.cn/Article/details/gpijryiux.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wap.zdbjq.cn/Article/details/gorsbtebu.sHtML

[N06] 判断回文字符串
来源：http://m.share.hesvh.cn/Article/details/gkpkqhvdf.sHtML

Py:   s == s[::-1]
来源：http://wap.hesvh.cn/Article/details/giyzglmyp.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gljvxdodf.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gkfkjptvb.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gouebhgub.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gipyhcjtn.sHtML

Go:   // 双指针从两端比较
来源：http://wap.hesvh.cn/Article/details/gnnbnyojk.sHtML

Ruby: s == s.reverse
来源：http://wap.hesvh.cn/Article/details/giwqyouwo.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/grgurrmot.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.fehbvm.com/Article/details/gucvsqbqk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gedjywvyi.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mobile.fehbvm.com/Article/details/glwxeytxi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.fehbvm.com/Article/details/grkdlpjdk.sHtML

TS:   // 手写 Map<string, number>
来源：http://m.share.hesvh.cn/Article/details/gatjzyxhs.sHtML

Java: // 手写 HashMap
来源：http://blog.zdbjq.cn/Article/details/gmkrghmca.sHtML

Go:   // 手写 map[int]int
来源：http://3g.hesvh.cn/Article/details/gnrvetsst.sHtML

Ruby: // 手写 Hash
来源：http://3g.fehbvm.com/Article/details/gxxxaksqt.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://3g.zdbjq.cn/Article/details/gcbfnltom.sHtML

[N08] 生成全排列
来源：http://wap.hesvh.cn/Article/details/gmfofipoq.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.fehbvm.com/Article/details/gtkzhtrby.sHtML

PHP:  // 手写递归交换
来源：http://www.blog.fehbvm.com/Article/details/gbnxvpujg.sHtML

JS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gxiytlmev.sHtML

TS:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/giidgmwqb.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.fehbvm.com/Article/details/gwwtgjfhh.sHtML

Go:   // 手写回溯递归
来源：http://www.blog.hesvh.cn/Article/details/gemcviehs.sHtML

Ruby: arr.permutation.to_a
来源：http://www.m.share.fehbvm.com/Article/details/gofpqclhy.sHtML

C#:   // 手写回溯递归
来源：http://mobile.zdbjq.cn/Article/details/gevdfnbpv.sHtML

[N09] 栈与队列
来源：http://www.share.fehbvm.com/Article/details/gydbuatqw.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.hesvh.cn/Article/details/gqgyfntij.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://wap.hesvh.cn/Article/details/gtzznrdag.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://blog.zdbjq.cn/Article/details/glcclpzkb.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://read.share.hesvh.cn/Article/details/gaphnvetb.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://www.share.fehbvm.com/Article/details/gfoouhjpv.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gflqtzpox.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://read.share.fehbvm.com/Article/details/ghdclqils.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://www.blog.hesvh.cn/Article/details/gvehdlodz.sHtML

[N10] 链表节点定义
来源：http://baike.hesvh.cn/Article/details/gbpumufrt.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://mobile.fehbvm.com/Article/details/ghnkgtgiq.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://www.blog.fehbvm.com/Article/details/gszwatcay.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.fehbvm.com/Article/details/ghoysnaoi.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://www.blog.fehbvm.com/Article/details/ghxwbbopi.sHtML

Java: class Node { int v; Node next; }
来源：http://read.share.hesvh.cn/Article/details/gerrbosvs.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://wap.hesvh.cn/Article/details/glvhcxmwu.sHtML


<!-- 参考信息 -->