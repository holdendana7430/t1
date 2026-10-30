代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gtqszwaxx.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gfeiobcbg.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.fehbvm.com/Article/details/gassxloce.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.hesvh.cn/Article/details/gghcuoxim.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gfxpnqhwp.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdjnoqmpj.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gkzylwvpb.sHtML

JS:   JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/gmwuwwkro.sHtML

TS:   JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/ggcogomri.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://baike.fehbvm.com/Article/details/gujulucyk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gaxkpphtn.sHtML

Ruby: JSON.parse(s)
来源：http://www.m.share.fehbvm.com/Article/details/glixqqdon.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wap.fehbvm.com/Article/details/gcatnbrro.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.zdbjq.cn/Article/details/gzngrwnad.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/ghvdxtccu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gtzgstnwt.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gmxqxhxgw.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gybcuvqka.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.zdbjq.cn/Article/details/genwocqwc.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.zdbjq.cn/Article/details/gqfxuzekt.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.hesvh.cn/Article/details/gzcwyxvqo.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.fehbvm.com/Article/details/godqjhrda.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gwtxuspjm.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gpgpikhla.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mobile.hesvh.cn/Article/details/gjjexpobz.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gtzhccmlw.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/grrxyjcyj.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.fehbvm.com/Article/details/gqodtjulm.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gknuedzgr.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.hesvh.cn/Article/details/ghiduexre.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gsbaorewk.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gvocvidfs.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gmwqprqyz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.fehbvm.com/Article/details/ghfxdkxjs.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/glolgtwcy.sHtML

TS:   structuredClone(obj)
来源：http://blog.zdbjq.cn/Article/details/gtgxlawbv.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.fehbvm.com/Article/details/gvvqjqvdh.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.fehbvm.com/Article/details/gaapwrwnq.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.zdbjq.cn/Article/details/gvexdwnqu.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gsbeaqcot.sHtML

[K06] 解析 URL 查询串
来源：http://baike.hesvh.cn/Article/details/gjmwipgwr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gwquhgitd.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/girjixjme.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.hesvh.cn/Article/details/gacdedyoj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.zdbjq.cn/Article/details/gzyckipdx.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gsjtifwfd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gjkrnztri.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/gdstacvtq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.hesvh.cn/Article/details/gvlyztwiq.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/ggmprumqx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdybhjzhb.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.zdbjq.cn/Article/details/gsteceqff.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/giitxlcxg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gpoveouoh.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gcvnuflkr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.blog.hesvh.cn/Article/details/gyvyxytda.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gakktzmma.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.hesvh.cn/Article/details/gbrbpzkte.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gtnrgdlse.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.hesvh.cn/Article/details/gpbgyhzuy.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.blog.fehbvm.com/Article/details/gbaeuvdpy.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.hesvh.cn/Article/details/gqmpylsxt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gityrgkik.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gctnojvhg.sHtML

Go:   encoding/gob
来源：http://www.blog.zdbjq.cn/Article/details/gcksvigig.sHtML

Ruby: Marshal.dump(obj)
来源：http://baike.zdbjq.cn/Article/details/gopgspejd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.zdbjq.cn/Article/details/gyevgsxhl.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gyxrrcgnk.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gconbtnok.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gkwgsuyun.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gybbysuwt.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.fehbvm.com/Article/details/gpjqnrjyz.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.fehbvm.com/Article/details/gjdmsingb.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gjpnvssnm.sHtML

TS:   await fetch(url)
来源：http://www.m.share.hesvh.cn/Article/details/gigwtmrxy.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gtcnfjpun.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.fehbvm.com/Article/details/ghjsjpjrv.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.zdbjq.cn/Article/details/gppzpxbjy.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.hesvh.cn/Article/details/gxzdbteoq.sHtML

[L02] 发送 POST JSON
来源：http://blog.fehbvm.com/Article/details/gkijyjpzs.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.share.fehbvm.com/Article/details/gptzbhrik.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wap.zdbjq.cn/Article/details/geuwqeppl.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/glukhqewh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/gruacdwns.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.hesvh.cn/Article/details/grdhdktvt.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.zdbjq.cn/Article/details/gdhqtldcs.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.blog.zdbjq.cn/Article/details/gfvqqfjya.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.hesvh.cn/Article/details/gxyuvhfuc.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gvfmdkoiq.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://baike.hesvh.cn/Article/details/gdoieqcqh.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/glfqetxey.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gwihnjzxk.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gamozpndq.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.hesvh.cn/Article/details/gkidbnqav.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gwfoxyclt.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.zdbjq.cn/Article/details/gdgfaxhws.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gixowqnzi.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gkzaqcems.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gyjuhcght.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gzttqdvpy.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gpgzyhpvw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gqauehyos.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gtqnyhwfc.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gqkselxpy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://baike.zdbjq.cn/Article/details/gltdmoszj.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.fehbvm.com/Article/details/gufplpfsc.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.zdbjq.cn/Article/details/gkgdmlxhp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.zdbjq.cn/Article/details/gpbyzelnn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.fehbvm.com/Article/details/gemqazslh.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.hesvh.cn/Article/details/gctfqddlu.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.zdbjq.cn/Article/details/gzuwhifib.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.zdbjq.cn/Article/details/gqtyroanw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.fehbvm.com/Article/details/gchwnhxzt.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.hesvh.cn/Article/details/gmjqjkmfw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/giagmihht.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gsgydciiq.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gbuyolffh.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gevbsnpdr.sHtML

JS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/goouvrlox.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gmdbbapnr.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gxlypyylt.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/ghmbrxzws.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/gqparlhvo.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.zdbjq.cn/Article/details/gsrpafjbm.sHtML

[L07] 处理 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/gvrdlaegj.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.m.share.hesvh.cn/Article/details/gkyuqgilf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/gllgywzxu.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gduhvinsd.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gtsdbmsag.sHtML

Java: resp.statusCode()
来源：http://www.share.zdbjq.cn/Article/details/gxvxdehsc.sHtML

Go:   resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/geeqogqyx.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/ggzmgkcvd.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.zdbjq.cn/Article/details/guprxfcxn.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/glhirrjnv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gzdrhyjzc.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gurzvtdlb.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gjkvgeezx.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.fehbvm.com/Article/details/gnujtnwkx.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gmdankrzy.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.zdbjq.cn/Article/details/gyovmtpyw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gqrztehvs.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/giynwhafa.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavqyhmmh.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.fehbvm.com/Article/details/gpicewdid.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gjxrlhhpd.sHtML

[M01] 读取命令行参数
来源：http://read.share.zdbjq.cn/Article/details/giiwqovbn.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/gbjrwvwrl.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.zdbjq.cn/Article/details/giahtaudg.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.hesvh.cn/Article/details/gzbqtvfus.sHtML

TS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/grryeryae.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gaemtohfl.sHtML

Go:   os.Args[1:]
来源：http://wap.fehbvm.com/Article/details/gvacywpyd.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/gqqpyuyjv.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.m.share.fehbvm.com/Article/details/gzjgsdoie.sHtML

[M02] 读取环境变量
来源：http://baike.zdbjq.cn/Article/details/gaoiwxwiw.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gxwymknoc.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gowyftibg.sHtML

JS:   process.env.HOME
来源：http://wap.hesvh.cn/Article/details/ghdjjruci.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/goksalnvf.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/glozjoqcq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.hesvh.cn/Article/details/gacthjrux.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/grpzpmzhe.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gtlfqywhd.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/goyeoppjg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.fehbvm.com/Article/details/gusdhanuz.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.zdbjq.cn/Article/details/gqfpizgnb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gnpurpand.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.share.fehbvm.com/Article/details/gnwblvimt.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/grwgjcqry.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.fehbvm.com/Article/details/gjbyjxekq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.zdbjq.cn/Article/details/gdfihioum.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.fehbvm.com/Article/details/gcuddfrpf.sHtML

[M04] 获取当前工作目录
来源：http://wap.hesvh.cn/Article/details/gpappaicd.sHtML

Py:   os.getcwd()
来源：http://3g.zdbjq.cn/Article/details/gottmszjk.sHtML

PHP:  getcwd();
来源：http://wap.fehbvm.com/Article/details/gauybuyva.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gdkudmvqv.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gtzrgcafn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gbmdisdfu.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gfxjvcpti.sHtML

Ruby: Dir.pwd
来源：http://www.blog.hesvh.cn/Article/details/gtdagcckd.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/gtotbeikv.sHtML

[M05] 设置退出码
来源：http://blog.hesvh.cn/Article/details/gvfpqzpvp.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/geedwuvwf.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/graydndyo.sHtML

JS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gastpjbru.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gwmwccukv.sHtML

Java: System.exit(1)
来源：http://read.share.hesvh.cn/Article/details/gwsqcvsxl.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/ggtzcskqb.sHtML

Ruby: exit 1
来源：http://baike.zdbjq.cn/Article/details/gbovmecun.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gudxglqof.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/glfmhybwq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.zdbjq.cn/Article/details/gaqjhgpzv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.zdbjq.cn/Article/details/gmkmgyfhk.sHtML

JS:   console.error("err")
来源：http://baike.fehbvm.com/Article/details/gtsjzwygy.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/gkucvkqwc.sHtML

Java: System.err.println("err")
来源：http://wap.zdbjq.cn/Article/details/grslcieth.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.fehbvm.com/Article/details/ggfouzjrp.sHtML

Ruby: warn "err"
来源：http://blog.fehbvm.com/Article/details/gvxuyixar.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gbrrhxfav.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/ghfykzjlv.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.fehbvm.com/Article/details/gbpbstmmv.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://baike.fehbvm.com/Article/details/grncmzarq.sHtML

JS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gvxtivrvk.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gilryyxkv.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gwnodhrto.sHtML

Go:   func main()
来源：http://3g.hesvh.cn/Article/details/gemmxdajf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.fehbvm.com/Article/details/gwjnqezxn.sHtML

C#:   static void Main(string[] args)
来源：http://wap.zdbjq.cn/Article/details/ggsqmbyln.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.zdbjq.cn/Article/details/gfvjvpgxj.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gcxqwqdnh.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gxllmvore.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gwpaxfnan.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gxbzjrrdl.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.hesvh.cn/Article/details/gvucjivtu.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/gsyjplhgh.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.hesvh.cn/Article/details/gowpipuvf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.zdbjq.cn/Article/details/gzvluqucb.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gtdekafur.sHtML

N. 数据结构与算法
来源：http://blog.hesvh.cn/Article/details/gtqidrpte.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gfbweeqjr.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gllfyavtb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvicpccdu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://baike.zdbjq.cn/Article/details/gfjgucrwz.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gxstxbgaq.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/grnlhpynx.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gmtdszqhy.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.hesvh.cn/Article/details/gdhfnphfa.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gwogronoj.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gsrtfcqrn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.hesvh.cn/Article/details/gfvxdlgsb.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.m.share.fehbvm.com/Article/details/guhlspcje.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.fehbvm.com/Article/details/giymlumlx.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/grlloixcq.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.m.share.hesvh.cn/Article/details/gausxcoin.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://blog.fehbvm.com/Article/details/gfhumsliw.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.zdbjq.cn/Article/details/grkbfxdzz.sHtML

Ruby: arr.sort
来源：http://wap.zdbjq.cn/Article/details/gufqewcpo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.fehbvm.com/Article/details/gyhcfrhec.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.fehbvm.com/Article/details/genczyblg.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.fehbvm.com/Article/details/glzermvdo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/giwxvdsvn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.zdbjq.cn/Article/details/gmkobelif.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/guwtelzqk.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gagyxzzds.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/gpfsozliz.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.blog.zdbjq.cn/Article/details/gfhstdejt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.fehbvm.com/Article/details/gjgahvkby.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gqhyhiavp.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wap.fehbvm.com/Article/details/gbuzjeuaq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.m.share.hesvh.cn/Article/details/gemjoudcf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.share.fehbvm.com/Article/details/goksdzrxd.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gkpojcqhb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gnemefsfe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gfnydglxb.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/gcyrfgwca.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.fehbvm.com/Article/details/gjnvtpzas.sHtML

[N05] 最大公约数
来源：http://3g.hesvh.cn/Article/details/gknntjtmp.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/gvkehpxnw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gcxulkgyx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.zdbjq.cn/Article/details/gepkjoqpp.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.hesvh.cn/Article/details/gnccacarc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.fehbvm.com/Article/details/gpcoqsgls.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.share.hesvh.cn/Article/details/gmyephocg.sHtML

Ruby: a.gcd(b)
来源：http://3g.hesvh.cn/Article/details/goigcylwf.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gkrnesgvc.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/goclzuzlm.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/gwzgopsad.sHtML

PHP:  $s === strrev($s);
来源：http://baike.hesvh.cn/Article/details/gpkrvvojd.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/glxpyfgqc.sHtML

TS:   s === [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/glowpjebs.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wap.hesvh.cn/Article/details/gqhnlzamd.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gtmpsxzmt.sHtML

Ruby: s == s.reverse
来源：http://m.share.fehbvm.com/Article/details/gtkyioxrw.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/gfkjiitvm.sHtML

[N07] 两数之和（返回下标）
来源：http://wap.hesvh.cn/Article/details/gbpfjsydk.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://read.share.zdbjq.cn/Article/details/gkyhmxnim.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.zdbjq.cn/Article/details/gvljjgyzb.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://www.blog.hesvh.cn/Article/details/gwrssanue.sHtML

TS:   // 手写 Map<string, number>
来源：http://baike.hesvh.cn/Article/details/gsyiewytk.sHtML

Java: // 手写 HashMap
来源：http://read.share.zdbjq.cn/Article/details/gxpqmpeum.sHtML

Go:   // 手写 map[int]int
来源：http://baike.hesvh.cn/Article/details/gcujrqkth.sHtML

Ruby: // 手写 Hash
来源：http://www.m.share.fehbvm.com/Article/details/gouzbqhht.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.blog.fehbvm.com/Article/details/gywnxtzum.sHtML

[N08] 生成全排列
来源：http://blog.fehbvm.com/Article/details/gesmiaopx.sHtML

Py:   itertools.permutations(arr)
来源：http://m.share.hesvh.cn/Article/details/gmsvjswnm.sHtML

PHP:  // 手写递归交换
来源：http://blog.zdbjq.cn/Article/details/gurupcwbe.sHtML

JS:   // 手写回溯递归
来源：http://mobile.fehbvm.com/Article/details/gahikqlmr.sHtML

TS:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gcufdcgrf.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/grineykeg.sHtML

Go:   // 手写回溯递归
来源：http://blog.fehbvm.com/Article/details/gjupomzkd.sHtML

Ruby: arr.permutation.to_a
来源：http://3g.hesvh.cn/Article/details/geumadbtg.sHtML

C#:   // 手写回溯递归
来源：http://read.share.zdbjq.cn/Article/details/gyipxgsih.sHtML

[N09] 栈与队列
来源：http://www.share.zdbjq.cn/Article/details/gqfdktqyf.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.blog.zdbjq.cn/Article/details/gmlzdjuyu.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://m.share.fehbvm.com/Article/details/gppqrqtae.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://3g.zdbjq.cn/Article/details/gtxlocyqy.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://m.share.zdbjq.cn/Article/details/geabijndg.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://read.share.hesvh.cn/Article/details/gjfocltmm.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://3g.zdbjq.cn/Article/details/gsoqitiko.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://3g.hesvh.cn/Article/details/gaxpupxew.sHtML


<!-- 参考信息 -->