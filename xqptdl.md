代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2iaozynfi.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2skihzzku.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wdgpmfcj.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2quylingy.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2moryxlcy.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt2bgydiruo.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.52xcode.cn/Article/details/gt2eaabnadi.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gwujgflc.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2ueplhdui.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt2vhifazwk.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2llifmerl.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2erozijna.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2kfpgoxsy.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt2zvwgmjin.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2languaky.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2uamrfelu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2tvstugtg.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2bwdcqoyn.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2uuxzrwsh.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2qptzsewn.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2lgbkjalw.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2sddxqjid.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2ddyoiipg.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2ciofduwh.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2apxerrxh.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt2ekemxztq.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2okifqmlb.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2prhknxcd.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2zbjjvskq.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2hpyhnayt.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2vcdqbvof.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2bxjrjeqi.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2gmbmnpdk.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2gcuxxteb.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2lwqsqvvt.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2lxijopkc.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2hzxejulm.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2lgmqwltd.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yqstgpcr.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2cxfjpvnf.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2lxiduktz.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt2gonupisg.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2qvudjjqt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2jtfqagwf.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2cldwujnh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2zvlabxjz.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2xoofjyzw.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2telwliaz.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2efpwdown.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt2kngunmbw.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2kwrnzxtk.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2talmiqqk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2jjflctsb.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2xhhxgwzr.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2aamtkcqx.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2srijmguh.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2hpoebkog.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rkcyrkce.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qnqyjpyq.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2esqndtrp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2ofcflewz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wmwuobiz.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2pzvwxvea.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt2lahctsoi.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2drehfthm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2thcseyrc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2sjmpdtgh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2wayfghqz.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2slqqptvl.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt2yizdupro.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt2jothhfpp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zvfpvfsl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2smtbmrvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mfwkhrgl.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rnjhmkfr.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt2iotuvgub.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2bgwptnze.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2wkvkkrzd.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2momeolxa.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt2ufhbijxh.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2ppjsufgb.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2yrejcmiu.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2ntliphts.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jhjqjrpo.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2vjkpzkbi.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2avbcsuxf.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2vfssnncm.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2wfxovggj.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2yxqxbwuk.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xppsilmr.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2bgyqyrcw.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2htrwfyid.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2gjzyirbb.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2heykslxo.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2ktofyvpu.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2dvafguwa.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2oneepmyu.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2azfwhzjr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2myoqehhx.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2mdebdhpd.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2mokkbxoi.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2saanbift.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2wtijlttd.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2qctyvxtt.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2izdmsbol.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2aouhzykc.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2unxqpckj.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2ntcrlgbo.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.ydjk.org.cn/Article/details/gt2fqfjpevs.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2aofslleo.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2puxgaayb.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2yogppxrx.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2gkmdpcgr.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2nerhyels.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2pbhwhfcq.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2bavtqxvb.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2uagszdjf.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2ofgmhzum.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pgrycixu.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2qogedhja.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2caqtalfx.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt2urgbiknv.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hwdqkeow.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2ykbjhptf.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2bfyfcjwr.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2qihyiquh.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2hqrxjkof.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2mbnurbol.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xullgpbr.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2szlovdtr.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2nyasmlrd.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2gdpekiuj.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2cboecaih.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2uuonklus.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2hkwbsvcd.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2cxxmajub.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2mesprtqc.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2rawuvmaz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt2weffdevl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2jzxhivmw.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2emdshcsb.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2rduwegif.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2uonxhpxm.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt2miqsyghr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2whrmzlny.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2xbhryovy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vdsucvug.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2rczmrvtn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqqusjqt.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2pyqldcpp.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2mclqqdkt.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2mrwogqgc.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuilnfv.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lcniupxw.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mliorvza.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2fktetysv.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2eukpnohj.html

C#:   args 数组（Main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2mjavhkfv.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt2udrmkfxb.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bainzedv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2seggkodl.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2hluorsbu.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2zcnpvyyu.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lvbgsnog.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2cevyedke.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2xadtovik.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cmdwowht.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2htyefgyc.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2satopkfv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2zypspozd.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wbwbvdzf.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2wvrmpnpf.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lhiyzvgp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2roceaosf.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2gapqpuzn.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2ilmtaosv.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2yvymzlqs.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2avvgusqc.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2spsefbni.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2snvtgqii.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2irlsdddy.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt2nwsjerwz.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2qqtdyrqx.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ewzvjbpz.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2ejrkcewx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2xyvsrfcy.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mhjfbfei.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2gelxqhik.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ppuyqonf.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uzzwnann.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2gcjjlvdh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nxkhiofv.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2rqqrdbth.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2qbdzmuab.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2comfeppl.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2gceewdsn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2emkgknrv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2zvardxbu.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2kdjjgdeb.html

Java: System.err.println("err")
来源：http://www.52xcode.cn/Article/details/gt2cgadpgqc.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2frbrzhki.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2uqqnthfw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2isrrbjni.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2awvtqyfy.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2nyqruhem.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2lhbhgvmo.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ahtqqouk.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qoycirom.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2axkaxquz.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2jpwpqqxx.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2ppposkuh.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2kziovmup.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2dknerkes.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2glpsdkcz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2pomeupqa.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2vrwtqbup.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2kxckxxhj.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2harwkxwq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt2zxwqvdpv.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2fnwctjes.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2uclnihpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fevakffk.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2mipftrsv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pxbtgwln.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2euxkdllz.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ardlvuxo.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2frmoooae.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2jwnfytje.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2locictvj.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ocncxscm.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2lsoroepk.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt2wyvvdsiu.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ymiswsru.html

[N02] 排序（工程实践用内置实现）
来源：http://www.ydjk.org.cn/Article/details/gt2ijexmbbf.html

Py:   sorted(arr);  arr.sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kjhjydcp.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2kougrafl.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2pvjdurpk.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.ydjk.org.cn/Article/details/gt2ykayamrg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.52xcode.cn/Article/details/gt2ilvfpbnv.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2vhzvavxu.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2bxdhwfad.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2udbdujwz.html

[N03] 快速排序（分治示例）
来源：http://www.ydjk.org.cn/Article/details/gt2jnvlzivd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2elauhtjm.html

PHP:  // 递归实现，或用 usort
来源：http://www.ydjk.org.cn/Article/details/gt2jnajwsgb.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2sgsxfzff.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.52xcode.cn/Article/details/gt2miqanisf.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2yjtxyncd.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2zpiicljp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2cskiwjvb.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.52xcode.cn/Article/details/gt2miozsjsi.html

[N04] 斐波那契数列
来源：http://www.52xcode.cn/Article/details/gt2dztqjnua.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2xuhhqvtp.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2ngvdmtuh.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xrqmcixg.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2mbuhtzow.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2olxjcmec.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2dwczhfom.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2oykukzte.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.52xcode.cn/Article/details/gt2wbumajkd.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2obdvwwcl.html

Py:   math.gcd(a, b)
来源：http://www.52xcode.cn/Article/details/gt2evipigdr.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrfrfklr.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2fysticdw.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2qeckztoi.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2hsozvkyb.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2idjccprx.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2qbswtbvo.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2rytvwqwz.html

[N06] 判断回文字符串
来源：http://www.ydjk.org.cn/Article/details/gt2toiaisoy.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rxagvflx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2rcukiimr.html

JS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2adehynvg.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wkzddtts.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.ydjk.org.cn/Article/details/gt2cpcfgrbb.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2ctfzcewz.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dvilbfcd.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2cppqgpyz.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qpuxfphu.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2dkijfaaz.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.52xcode.cn/Article/details/gt2redvzcqc.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2izawsoem.html

TS:   // 手写 Map<string, number>
来源：http://www.ydjk.org.cn/Article/details/gt2bwrfelcv.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2cmhrswps.html

Go:   // 手写 map[int]int
来源：http://www.52xcode.cn/Article/details/gt2byteuaaq.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2wojbjkes.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2axykblxn.html

[N08] 生成全排列
来源：http://www.ydjk.org.cn/Article/details/gt2ddpfirrr.html

Py:   itertools.permutations(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2skmvwrsk.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2ieahgram.html

JS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tqesbjcf.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2bpfbgequ.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2tbqfokpm.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2xeqfkdin.html

Ruby: arr.permutation.to_a
来源：http://www.ydjk.org.cn/Article/details/gt2awrxoofv.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2onnskbld.html

[N09] 栈与队列
来源：http://www.ydjk.org.cn/Article/details/gt2mhlmszfl.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2eztxofax.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.ydjk.org.cn/Article/details/gt2oviquwlb.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2iqcnltul.html


<!-- 参考信息 -->