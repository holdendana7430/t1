代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://read.share.fehbvm.com/Article/details/gdaswrmza.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.zdbjq.cn/Article/details/gdsyvuupc.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.hesvh.cn/Article/details/genrahjot.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gdiyfnbbi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gukydqypo.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/geikadpeu.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwdoxrmxz.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggagtyxfo.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.fehbvm.com/Article/details/gszllkthm.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/gqqgohopg.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghdgsbkwa.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/glitibbci.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.fehbvm.com/Article/details/gdkoxeyyv.sHtML

Go:   json.Marshal(obj)
来源：http://wap.fehbvm.com/Article/details/gknstmujb.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.hesvh.cn/Article/details/gmvukstkg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/gvysqogif.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gdzyerufr.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gfvhegpux.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://3g.zdbjq.cn/Article/details/gpcgentqa.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gggqywxcm.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gynqwfntq.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.fehbvm.com/Article/details/gujwbustg.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gnmgdelnc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gjynhehka.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/ghukbokfj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gbyjdskwr.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/gwnybjbwv.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gfemmswfb.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gcvapuirn.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gbazoficv.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.fehbvm.com/Article/details/gcxfcirlj.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wap.zdbjq.cn/Article/details/gidrccecc.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.fehbvm.com/Article/details/gjthxdanq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gufgqzhwp.sHtML

[K04] 读取 JSON 文件
来源：http://baike.fehbvm.com/Article/details/ghvlspril.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://blog.zdbjq.cn/Article/details/ggymwmqkb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gtxvnmhkm.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.hesvh.cn/Article/details/gleyhjorm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gbtiwtivm.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gvkqoruun.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wap.zdbjq.cn/Article/details/giobywphj.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/gfznzlwbh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://3g.hesvh.cn/Article/details/gtmaenyco.sHtML

[K05] 深拷贝对象
来源：http://baike.zdbjq.cn/Article/details/goefnlsgt.sHtML

Py:   copy.deepcopy(obj)
来源：http://mobile.fehbvm.com/Article/details/gekldpewb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/ghypfpxxx.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/ggyqzfmud.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/guscqcpfj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gawmbhshf.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gcpudsbja.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.zdbjq.cn/Article/details/gycncylnn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://3g.zdbjq.cn/Article/details/ggpxybpjr.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.fehbvm.com/Article/details/gwryuruvl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://3g.fehbvm.com/Article/details/gqtmxexxa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://baike.fehbvm.com/Article/details/gdotfcxpx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.hesvh.cn/Article/details/ggzgvzgqw.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guhbdniin.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gmatrcege.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gzgjixdpk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gzcabcrjc.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.hesvh.cn/Article/details/ggkvsbrho.sHtML

[K07] 进制转换
来源：http://mobile.fehbvm.com/Article/details/gmpvlblot.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gzgvvznli.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/grindjpif.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gjazzskbh.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/grisecehj.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/giexdrlwn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blog.fehbvm.com/Article/details/gcrinkmya.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/grdibbpkr.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gzactzvkm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://3g.fehbvm.com/Article/details/giafrhghn.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.fehbvm.com/Article/details/gehgzeczt.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.fehbvm.com/Article/details/gvjpplmvm.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/gygttnpvo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://read.share.hesvh.cn/Article/details/gvxssiphv.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.fehbvm.com/Article/details/ggbmqovfs.sHtML

Go:   encoding/gob
来源：http://m.share.hesvh.cn/Article/details/gyawpphwq.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.hesvh.cn/Article/details/gtkdcxiio.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/glqxyphul.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gqzhzyfio.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gtkkajbhs.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gpinmckea.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gctlmocso.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/glurtyzje.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.hesvh.cn/Article/details/gdnkavttc.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/goculsxym.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/glyfubpju.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.fehbvm.com/Article/details/gigaedgms.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.blog.fehbvm.com/Article/details/gwhxnhofp.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/goyuedvep.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.share.hesvh.cn/Article/details/glknqyzgl.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/grkdaldjj.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gralrxtll.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.fehbvm.com/Article/details/gwnviajqd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/guiyucwmq.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gkxeooren.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wap.hesvh.cn/Article/details/gaeeseucw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gsrvfatpc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gzfvfsrmm.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://read.share.zdbjq.cn/Article/details/gwrcciill.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gtgfqoxdn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.zdbjq.cn/Article/details/grpsgtdif.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.zdbjq.cn/Article/details/gqjrccmfd.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.fehbvm.com/Article/details/gjnfbzkea.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/gxfbtwzvg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.hesvh.cn/Article/details/gaipvorrf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmrpystr.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gpesylqri.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/ggacdrnbf.sHtML

[L04] 设置超时
来源：http://read.share.hesvh.cn/Article/details/gmqyuqhfd.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.zdbjq.cn/Article/details/gpudmngju.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/ggqswpahu.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/ggwovveud.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mobile.zdbjq.cn/Article/details/gnzafomdx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.hesvh.cn/Article/details/gvquhdbxm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.fehbvm.com/Article/details/gfgfkkefe.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.zdbjq.cn/Article/details/gvtmanpgo.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.zdbjq.cn/Article/details/gnkyyfvop.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.hesvh.cn/Article/details/gaayiwxkp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.zdbjq.cn/Article/details/gpyutbhtj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.blog.zdbjq.cn/Article/details/grpwwrntz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.hesvh.cn/Article/details/gqevxopyc.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gozzjzvkl.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.zdbjq.cn/Article/details/gxqupoqwr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gcfrqemii.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gmndjbigb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/gbviyadrq.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gjfloaeni.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gzaspufzq.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.fehbvm.com/Article/details/gbnudbacp.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gjevhhmcr.sHtML

TS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/ghtaszoxc.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/ggsozglik.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.zdbjq.cn/Article/details/gjynbmbnq.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.zdbjq.cn/Article/details/ggfjvgpcz.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.fehbvm.com/Article/details/goszguzqs.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/ggnceuchi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.hesvh.cn/Article/details/gmrdyvqlz.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.hesvh.cn/Article/details/ggoxmwdyt.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/glubpgmjx.sHtML

TS:   resp.ok;  resp.status
来源：http://blog.zdbjq.cn/Article/details/gsdkjeblz.sHtML

Java: resp.statusCode()
来源：http://www.share.hesvh.cn/Article/details/gkisiimnv.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/gmxkifqba.sHtML

Ruby: resp.code.to_i
来源：http://mobile.fehbvm.com/Article/details/gxdaanmao.sHtML

C#:   (int)resp.StatusCode
来源：http://www.m.share.fehbvm.com/Article/details/geqdtcowd.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gtiuewnqy.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.hesvh.cn/Article/details/gjlyeqrht.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.fehbvm.com/Article/details/ghiqawvok.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gilnmajxd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gcayqmwxt.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gdovgjrzd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gqreimwkj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.fehbvm.com/Article/details/gcdifpclw.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gxlbkucdi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gegwgjbob.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/gvwcivlgd.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gvdwkvgzb.sHtML

[M01] 读取命令行参数
来源：http://baike.hesvh.cn/Article/details/gwbrxuhmz.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/grjzvbloc.sHtML

PHP:  $argv;  $argc;
来源：http://mobile.hesvh.cn/Article/details/gnphhclqn.sHtML

JS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/ganaadfqn.sHtML

TS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gzjcijuhz.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gmnkaizdp.sHtML

Go:   os.Args[1:]
来源：http://3g.zdbjq.cn/Article/details/gipkjcjcd.sHtML

Ruby: ARGV
来源：http://www.share.zdbjq.cn/Article/details/gtpgdohtl.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gceknmmud.sHtML

[M02] 读取环境变量
来源：http://mobile.hesvh.cn/Article/details/gbduqiwyh.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.fehbvm.com/Article/details/gnsvxmney.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.m.share.hesvh.cn/Article/details/gskbvtcuj.sHtML

JS:   process.env.HOME
来源：http://3g.hesvh.cn/Article/details/gflxfbpow.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/griktsini.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/glahampoy.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/grroinlzk.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.zdbjq.cn/Article/details/gnvszbxkh.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wap.fehbvm.com/Article/details/galnlwsmg.sHtML

[M03] 执行外部命令
来源：http://m.share.zdbjq.cn/Article/details/gmumqdxkf.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gfhxgtwmu.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.m.share.zdbjq.cn/Article/details/gbpminslk.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/ganpzlhsg.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/ggcmahjsx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gbdqrnvfr.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.zdbjq.cn/Article/details/gtwxgsduq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gxmnsrfym.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.zdbjq.cn/Article/details/golebkejh.sHtML

[M04] 获取当前工作目录
来源：http://mobile.hesvh.cn/Article/details/govpmujsb.sHtML

Py:   os.getcwd()
来源：http://www.share.zdbjq.cn/Article/details/gfcyrqmoq.sHtML

PHP:  getcwd();
来源：http://www.share.hesvh.cn/Article/details/gtzvesyxg.sHtML

JS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gwabmjveb.sHtML

TS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/grclyajcp.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://blog.hesvh.cn/Article/details/gqifnppjm.sHtML

Go:   os.Getwd()
来源：http://m.share.fehbvm.com/Article/details/gpsdbbfxi.sHtML

Ruby: Dir.pwd
来源：http://blog.fehbvm.com/Article/details/gppyitwqm.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.hesvh.cn/Article/details/gkvsouxmh.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/geqrxeqem.sHtML

Py:   sys.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gwnnfrhgj.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gwrugrcrf.sHtML

JS:   process.exit(1)
来源：http://blog.fehbvm.com/Article/details/gbjzpygjk.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpiblbdzv.sHtML

Java: System.exit(1)
来源：http://blog.hesvh.cn/Article/details/gyhxgwrir.sHtML

Go:   os.Exit(1)
来源：http://www.share.fehbvm.com/Article/details/gfvmktvbw.sHtML

Ruby: exit 1
来源：http://read.share.fehbvm.com/Article/details/gsfjfgfti.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.fehbvm.com/Article/details/gtbxdgamg.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/guusqknkh.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.fehbvm.com/Article/details/gbxgjrout.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.zdbjq.cn/Article/details/gtgitfibh.sHtML

JS:   console.error("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxzktsmhe.sHtML

TS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gadlaglex.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/gkvhzizoc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gmrjboddn.sHtML

Ruby: warn "err"
来源：http://m.share.zdbjq.cn/Article/details/gdfyysphh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gmllnrbju.sHtML

[M07] 判断是否为主入口
来源：http://3g.hesvh.cn/Article/details/gbwhtwhbq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.fehbvm.com/Article/details/grhlisuhh.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gygbxqhnr.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gqqnsxfrb.sHtML

TS:   require.main === module
来源：http://www.m.share.hesvh.cn/Article/details/gmrqzyvsa.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gzpvuzyhk.sHtML

Go:   func main()
来源：http://m.share.fehbvm.com/Article/details/gpuecdpkp.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gqmkxxdon.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gormbvtfu.sHtML

[M08] 获取系统与运行时信息
来源：http://m.share.zdbjq.cn/Article/details/gwfbiiovf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/gfekkdbaq.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gmulymgvw.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gushiqgfb.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gogekpdcz.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.fehbvm.com/Article/details/gieuotasi.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.share.fehbvm.com/Article/details/gjxhwvxtn.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gfegvxidz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.zdbjq.cn/Article/details/gtqgpztkv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gbofpfluk.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gzeytbymo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gledrlxyg.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.hesvh.cn/Article/details/gtcpezhzw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gqtxcvngl.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/grkylmqea.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://read.share.zdbjq.cn/Article/details/glnsyeuhy.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.zdbjq.cn/Article/details/gptqyalfa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.fehbvm.com/Article/details/gembptdve.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/ghemvucyq.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.fehbvm.com/Article/details/ggfrbzrtu.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gqoyhoxys.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://blog.hesvh.cn/Article/details/gmmugksux.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.zdbjq.cn/Article/details/gvyzbrait.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.hesvh.cn/Article/details/gbibyariw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.zdbjq.cn/Article/details/gqxihbqmr.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjfzgybvt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://read.share.hesvh.cn/Article/details/gksbvglrz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gznnmnomg.sHtML

Ruby: arr.sort
来源：http://www.share.hesvh.cn/Article/details/gruohbasf.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/gczglyoff.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.zdbjq.cn/Article/details/gststmgef.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.hesvh.cn/Article/details/gafwijzcd.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.zdbjq.cn/Article/details/gkjrpyurx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.hesvh.cn/Article/details/gabwcqgwn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gsmcyhqjs.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mobile.fehbvm.com/Article/details/gikpaxvtx.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.hesvh.cn/Article/details/ghhqechsc.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.fehbvm.com/Article/details/gjjkuauls.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.blog.hesvh.cn/Article/details/gygznluxr.sHtML

[N04] 斐波那契数列
来源：http://mobile.zdbjq.cn/Article/details/gzyyrhyrq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gzrcradgz.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.blog.fehbvm.com/Article/details/gewfltxxw.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/gnumyjwhm.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gnbvzrrow.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.zdbjq.cn/Article/details/gpbgopqqe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.hesvh.cn/Article/details/goaopxsgj.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gyrbrtato.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/gfjnwkbwn.sHtML

[N05] 最大公约数
来源：http://read.share.hesvh.cn/Article/details/gluzoadeu.sHtML

Py:   math.gcd(a, b)
来源：http://blog.hesvh.cn/Article/details/gxuvcrogw.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mobile.hesvh.cn/Article/details/ggvfqklpx.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/geioiflpg.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wap.fehbvm.com/Article/details/gnpfyrjoo.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://baike.hesvh.cn/Article/details/gknzbqazs.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/gyoneojsc.sHtML

Ruby: a.gcd(b)
来源：http://read.share.zdbjq.cn/Article/details/gfzjllgnu.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://read.share.zdbjq.cn/Article/details/guvdmhamz.sHtML

[N06] 判断回文字符串
来源：http://www.blog.hesvh.cn/Article/details/gaiojqtib.sHtML

Py:   s == s[::-1]
来源：http://baike.zdbjq.cn/Article/details/gmowxoyxe.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gjlnqailr.sHtML

JS:   s === [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gijtmoldn.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gadonacao.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gsbdcsxzb.sHtML

Go:   // 双指针从两端比较
来源：http://3g.hesvh.cn/Article/details/gerquvrwh.sHtML

Ruby: s == s.reverse
来源：http://www.share.fehbvm.com/Article/details/gwmhofdwz.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gwexiqtwc.sHtML

[N07] 两数之和（返回下标）
来源：http://blog.hesvh.cn/Article/details/goggqwlzg.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.hesvh.cn/Article/details/gcxxeblyn.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.zdbjq.cn/Article/details/gtcxqwpmc.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://blog.zdbjq.cn/Article/details/gqyvwlocj.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.hesvh.cn/Article/details/grkfikbrh.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/grrciawhu.sHtML

Go:   // 手写 map[int]int
来源：http://baike.zdbjq.cn/Article/details/ghahxxfyw.sHtML

Ruby: // 手写 Hash
来源：http://www.share.zdbjq.cn/Article/details/geogebxcf.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.fehbvm.com/Article/details/gwzuhsvtl.sHtML

[N08] 生成全排列
来源：http://mobile.fehbvm.com/Article/details/gpdllmhed.sHtML

Py:   itertools.permutations(arr)
来源：http://3g.zdbjq.cn/Article/details/gyulsjrue.sHtML

PHP:  // 手写递归交换
来源：http://www.m.share.zdbjq.cn/Article/details/glmeahrfi.sHtML

JS:   // 手写回溯递归
来源：http://www.m.share.zdbjq.cn/Article/details/gdcnrkipl.sHtML

TS:   // 手写回溯递归
来源：http://wap.hesvh.cn/Article/details/gnxvzsgid.sHtML


<!-- 参考信息 -->