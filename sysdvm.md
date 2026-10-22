代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2xxhjgwsj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2gjweobwq.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cqfdonjm.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2vdkeidoz.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2aabxvaew.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yrklqgmp.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2ktfcuqeu.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ahxdyoyn.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2vsfwqael.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqykifmu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt2xjchgraa.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2bhegvzcu.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2vesivnrp.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2doctbkbv.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2ocagzzlk.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxsnhams.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2akxbobwu.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2umynojws.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2jlvdyeti.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ycbctvqe.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hcimyksv.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2fcxtjwhd.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2gmzyhlqr.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt2njzsrcdu.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2vyphtggs.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2klbmukrm.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2ajkcnbgo.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2vmficsol.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2ncgpujxt.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2yoyegwnw.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2omgvsfjq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2khtvqzdl.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2omdviafz.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2vpnznroc.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xybpgvrx.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2nuzkstac.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2utuazthc.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2wxowveyz.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2heeymbti.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2tqyfiqkz.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2psuusksc.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2qdgagmpt.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2ufpvskrt.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2wrqbwdlk.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2qmkxvkdi.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2cjnwvlnx.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt2psbovgup.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2htjgkizg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2vvetrnym.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2fbituzbf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2ubcncuws.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2qbtxlsuk.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vhskbhah.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2jrhuzwrb.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rgkfbhsc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt2dlbteuls.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zyeuocih.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2cptmpvoh.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2dtuyzhbc.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2xrdtysgy.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2nkqkbrvc.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2qudhhmrc.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2ekcmprei.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2ppatuqss.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wakxvbru.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2lekzmgiw.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xevszuzp.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt2bahcqdiw.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2fxtwhqex.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gsjjyktm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2xhjaoklf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tcgtntzy.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2qkbuqxcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oxgagnum.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2jipzkpay.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2yskudcst.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2cytuouyc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2uxodxpsb.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2dathvtaq.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2xpwxapwx.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nfgsszqe.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2pnyrcuce.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2glsereoo.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xuisikpq.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2jqjthqda.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt2ccgbmahl.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ajcophvn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2eenhhvre.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2pzdsjsno.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2utwafurn.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2ffjkjikz.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2ekvzzpaz.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2oxtvjpnh.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt2pqcaqppx.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt2knvbiwzj.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2ijzmdeun.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2fhoenxuq.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2cszcqglc.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2prfwhfzh.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2lwrnpvag.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2cljlqobv.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2bpfbdumo.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt2zndaeuhb.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2wpnumqqz.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2zsydlnch.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2euaqndxw.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2ccyjdars.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt2pgmzhfsl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2mpxhafvd.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2ucvplxid.html

[L05] 上传文件（multipart）
来源：http://www.ydjk.org.cn/Article/details/gt2rgtudajz.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.52xcode.cn/Article/details/gt2fkwuxzcz.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt2lxsnpshc.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2dvknvwgy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2oziegmyv.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt2uadgwsvm.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt2xoverckl.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt2bldewyyq.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zedurnlu.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt2traijbai.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2giwnzzar.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2juvwslgr.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2ffjbycld.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2fcsqysyi.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2hridqaqd.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tndbbgnv.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2pbwahqjn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2qbfsjxyl.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pvstlcbi.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt2tdupqoho.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2ntrneafb.html

JS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2hbpgyark.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2nxtdkyax.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2icwwxhip.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2dkrceagz.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt2ohfopbrt.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2ztpejhfv.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2bjcqlmxu.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2fofzjyin.html

PHP:  curl_multi_init() 系列
来源：http://www.ydjk.org.cn/Article/details/gt2ecgowtbi.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2tqbgdigu.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2ltaasoib.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2lgwwcjmo.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2udxhemip.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt2qygwucgn.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2natbbhik.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ulbuwzkt.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2bwosoajt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ftsupptc.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2rqzczuzu.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt2znkgkfhf.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2qstgtcwg.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2bvfcgkld.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oouotcpo.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2dvimngzu.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2bibganal.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt2vpsrmqqs.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yspjsotk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rvbzjevl.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2tdxgeubv.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2jzccckcl.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2nhfxwimo.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2uuxwrcwp.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2bfnqvezl.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2cuctztfr.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wgeoysxx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2zlmqzgnu.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt2uhnmupxd.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xpfcdewj.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2svaxwaho.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2iuvympja.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2qsrgwehc.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2dydgtgud.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2uvjtiwuz.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2kinbbici.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2gjsqblls.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2ljhsjehb.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2yhassscr.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2byrjyaic.html

JS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2rpklordh.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2gpbyzahs.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2zxrsldxi.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2aavzzqto.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2qdvowufq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt2ziqicfnq.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt2rwsptiyt.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2kivdplmq.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2sfzgcwzp.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2xdcydpid.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fuobheax.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2vludempn.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbknwii.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt2tvckmpgl.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2zqswefgi.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2mgmldpnz.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2mgtjwnxk.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2bgzxcide.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2haingdrk.html

TS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2cebvrkgd.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2bapzcgmt.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2urzafrni.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2ntllxlxv.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2nvfwdoxu.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2cxspkkha.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2ytaolwje.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2kwelrint.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2ccekzwcw.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2rfvimday.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2ecqfbtax.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2zfzqxaqz.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt2bztosnro.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2elvfxmad.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2opymhebv.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2sjlcdqaj.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt2nnxuqcrr.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2rdujtfbv.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2bdppagpe.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2vofxwjwh.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2yqabkaod.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt2pvvqxval.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2jkulniwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpvbkgqm.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2rhczqqnr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bmepruko.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2ptrdrzrq.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2rdfuyqrv.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xkcaftfr.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2xwnyvnwy.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2idbxaqvt.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2nqedblzu.html

Go:   sort.SearchInts(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2jnegksvn.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.ydjk.org.cn/Article/details/gt2bfmukpbm.html

C#:   Array.BinarySearch(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2dpvkledg.html

[N02] 排序（工程实践用内置实现）
来源：http://www.52xcode.cn/Article/details/gt2jzogkoqz.html

Py:   sorted(arr);  arr.sort()
来源：http://www.52xcode.cn/Article/details/gt2jxphfoog.html

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.52xcode.cn/Article/details/gt2safilbca.html

JS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2jgokeyqb.html

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.52xcode.cn/Article/details/gt2stznobsg.html

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.ydjk.org.cn/Article/details/gt2krzhecaj.html

Go:   slices.Sort(arr)
来源：http://www.52xcode.cn/Article/details/gt2krklvctw.html

Ruby: arr.sort
来源：http://www.ydjk.org.cn/Article/details/gt2vvndrxyu.html

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.ydjk.org.cn/Article/details/gt2kxjikidl.html

[N03] 快速排序（分治示例）
来源：http://www.52xcode.cn/Article/details/gt2ciahjuvd.html

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.52xcode.cn/Article/details/gt2efoubwlh.html

PHP:  // 递归实现，或用 usort
来源：http://www.52xcode.cn/Article/details/gt2ysochbwm.html

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2cckettpr.html

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.ydjk.org.cn/Article/details/gt2nnrnscef.html

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.ydjk.org.cn/Article/details/gt2wobqoskq.html

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.ydjk.org.cn/Article/details/gt2xsvnkvzp.html

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.52xcode.cn/Article/details/gt2dfumgphn.html

C#:   // 手写递归，或 Array.Sort
来源：http://www.ydjk.org.cn/Article/details/gt2olsitdmk.html

[N04] 斐波那契数列
来源：http://www.ydjk.org.cn/Article/details/gt2twfqafgs.html

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vqaxdnrj.html

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.52xcode.cn/Article/details/gt2mdvjsrgj.html

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2xuymjgod.html

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2znlvevan.html

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.ydjk.org.cn/Article/details/gt2zxtzkwjl.html

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.ydjk.org.cn/Article/details/gt2asyqccjj.html

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.52xcode.cn/Article/details/gt2wwbnmone.html

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.ydjk.org.cn/Article/details/gt2fwbtkppc.html

[N05] 最大公约数
来源：http://www.ydjk.org.cn/Article/details/gt2pxphjpzg.html

Py:   math.gcd(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ohhtovct.html

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ihzbcigo.html

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.ydjk.org.cn/Article/details/gt2ifllrdiz.html

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.52xcode.cn/Article/details/gt2awzftdyb.html

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.52xcode.cn/Article/details/gt2ogznigdr.html

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.52xcode.cn/Article/details/gt2jvxknfhe.html

Ruby: a.gcd(b)
来源：http://www.ydjk.org.cn/Article/details/gt2dbsipvim.html

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.ydjk.org.cn/Article/details/gt2fatgecit.html

[N06] 判断回文字符串
来源：http://www.52xcode.cn/Article/details/gt2iakflcbu.html

Py:   s == s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2crrjsprx.html

PHP:  $s === strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jlqidkrj.html

JS:   s === [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qdpprbfv.html

TS:   s === [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qbckbcps.html

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.52xcode.cn/Article/details/gt2jzxbfpir.html

Go:   // 双指针从两端比较
来源：http://www.ydjk.org.cn/Article/details/gt2iafkqfth.html

Ruby: s == s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2rzjlowax.html

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hhsypcvp.html

[N07] 两数之和（返回下标）
来源：http://www.ydjk.org.cn/Article/details/gt2qurzvsme.html

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.52xcode.cn/Article/details/gt2eijohmbl.html

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://www.ydjk.org.cn/Article/details/gt2rbxojqek.html

JS:   // 手写 Map：map.set(v, i)
来源：http://www.ydjk.org.cn/Article/details/gt2jsiycghb.html

TS:   // 手写 Map<string, number>
来源：http://www.52xcode.cn/Article/details/gt2xfewttur.html

Java: // 手写 HashMap
来源：http://www.ydjk.org.cn/Article/details/gt2caclwchl.html

Go:   // 手写 map[int]int
来源：http://www.ydjk.org.cn/Article/details/gt2wipojspj.html

Ruby: // 手写 Hash
来源：http://www.ydjk.org.cn/Article/details/gt2rshruequ.html

C#:   // 手写 Dictionary<int, int>
来源：http://www.ydjk.org.cn/Article/details/gt2ndronnej.html

[N08] 生成全排列
来源：http://www.52xcode.cn/Article/details/gt2zbvftsqd.html

Py:   itertools.permutations(arr)
来源：http://www.52xcode.cn/Article/details/gt2prhkakxl.html

PHP:  // 手写递归交换
来源：http://www.52xcode.cn/Article/details/gt2dzkxrqaw.html

JS:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2kiccgrhd.html

TS:   // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2nhvcgjis.html

Java: // 手写回溯递归
来源：http://www.ydjk.org.cn/Article/details/gt2fohwfupj.html

Go:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2ugkrpwal.html

Ruby: arr.permutation.to_a
来源：http://www.52xcode.cn/Article/details/gt2xsdgiyxh.html

C#:   // 手写回溯递归
来源：http://www.52xcode.cn/Article/details/gt2sedcrvvu.html

[N09] 栈与队列
来源：http://www.52xcode.cn/Article/details/gt2czfpncyy.html

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.52xcode.cn/Article/details/gt2kvxrfrok.html

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2sycbugdm.html

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://www.52xcode.cn/Article/details/gt2pfjdtjlz.html


<!-- 参考信息 -->