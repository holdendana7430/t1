代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.hesvh.cn/Article/details/gjahfxeda.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gwdynjlkm.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.zdbjq.cn/Article/details/gvhuconsy.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gzejjeaat.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/groqkykpc.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gzyaikhpn.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://read.share.fehbvm.com/Article/details/gxfembodq.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.zdbjq.cn/Article/details/gtgowsonn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gsatdxvay.sHtML

K. JSON 与序列化
来源：http://www.share.zdbjq.cn/Article/details/gtvxtcneu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gxkbheyoh.sHtML

[K01] 对象转 JSON 字符串
来源：http://blog.hesvh.cn/Article/details/gvmcdvyod.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.share.fehbvm.com/Article/details/gqufguqkl.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/ggzrisnnt.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.fehbvm.com/Article/details/ggqantwsb.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.zdbjq.cn/Article/details/grtabfbsb.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.zdbjq.cn/Article/details/gwjmvaylr.sHtML

Go:   json.Marshal(obj)
来源：http://m.share.hesvh.cn/Article/details/gilzllmdt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gxmcbmsuu.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.zdbjq.cn/Article/details/goaoprfxf.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.fehbvm.com/Article/details/gmjkgcddn.sHtML

Py:   json.loads(s)
来源：http://read.share.fehbvm.com/Article/details/gzuxkxkjx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wap.fehbvm.com/Article/details/gwwrnyrdh.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/golydtocf.sHtML

TS:   JSON.parse(s)
来源：http://blog.fehbvm.com/Article/details/goghbdmml.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://read.share.fehbvm.com/Article/details/gdcjbljyd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.hesvh.cn/Article/details/gdhnfsuui.sHtML

Ruby: JSON.parse(s)
来源：http://read.share.zdbjq.cn/Article/details/gqlfgpyec.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmoerjlpk.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/geamdscyk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gnkzijipf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gauwdoznw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gxxmhgapp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.hesvh.cn/Article/details/gxoycbgfn.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.fehbvm.com/Article/details/gcrhqseyl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://blog.hesvh.cn/Article/details/gntdulhnf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gbcbbrvpa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wap.zdbjq.cn/Article/details/gvptonxfl.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.hesvh.cn/Article/details/gehxbqbmc.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.fehbvm.com/Article/details/gtzeuxwgi.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.zdbjq.cn/Article/details/gqbxfcmvl.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gjdlmjjwu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.m.share.fehbvm.com/Article/details/glzaggdcd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.fehbvm.com/Article/details/gssoqpgil.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gpdcimeox.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://3g.fehbvm.com/Article/details/gvgrmjque.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.hesvh.cn/Article/details/gtruwrxyl.sHtML

[K05] 深拷贝对象
来源：http://www.blog.hesvh.cn/Article/details/gmspxnmka.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.m.share.hesvh.cn/Article/details/geumnlljx.sHtML

PHP:  unserialize(serialize($obj));
来源：http://read.share.zdbjq.cn/Article/details/ghaooswnu.sHtML

JS:   structuredClone(obj)
来源：http://m.share.hesvh.cn/Article/details/gkyfwntww.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gpfpegndu.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.zdbjq.cn/Article/details/gaphtgtxs.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://3g.hesvh.cn/Article/details/gqjkqzksh.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.fehbvm.com/Article/details/gujpzhaug.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.hesvh.cn/Article/details/gofekruyg.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.fehbvm.com/Article/details/gtyoygqbw.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mobile.hesvh.cn/Article/details/ggpfmcquc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gnrgoosbn.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/griipaphi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.hesvh.cn/Article/details/getxklstl.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.fehbvm.com/Article/details/gqghiqemi.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/guckcytrk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/gxttrjgdr.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gbplpnwrs.sHtML

[K07] 进制转换
来源：http://www.blog.zdbjq.cn/Article/details/gpkwiawog.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gtctyecdt.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/grororsgg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/ggtzjpfba.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ggvrgladn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gwvcpqwii.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/ggxhcbrzm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.hesvh.cn/Article/details/glwewobwk.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.zdbjq.cn/Article/details/gcfzzsfpo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gmgcetytp.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gwsykppgj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.hesvh.cn/Article/details/gitemcdvt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.zdbjq.cn/Article/details/gdznogmdr.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.zdbjq.cn/Article/details/gvjulxkbg.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.fehbvm.com/Article/details/gtgdcyrtq.sHtML

Go:   encoding/gob
来源：http://wap.hesvh.cn/Article/details/gwobtyjsb.sHtML

Ruby: Marshal.dump(obj)
来源：http://wap.fehbvm.com/Article/details/ggnkbsbqd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://read.share.hesvh.cn/Article/details/gseipjwhm.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gcsvllzxl.sHtML

L. 网络请求
来源：http://baike.fehbvm.com/Article/details/gcpaoptji.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmtirpdcp.sHtML

[L01] 发送 GET 请求
来源：http://m.share.zdbjq.cn/Article/details/gzibjfgqi.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.zdbjq.cn/Article/details/gabgmvhub.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gqdedadit.sHtML

JS:   await fetch(url)
来源：http://3g.fehbvm.com/Article/details/gbkphdpjl.sHtML

TS:   await fetch(url)
来源：http://www.m.share.fehbvm.com/Article/details/gzkjgcfvi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.hesvh.cn/Article/details/gddkbxrcq.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.share.fehbvm.com/Article/details/gdzqpejmx.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.hesvh.cn/Article/details/gmrgzzfsv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://m.share.fehbvm.com/Article/details/gxjsdjylo.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gauejyhtp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.zdbjq.cn/Article/details/gposjhbhy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gzfkspjdh.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gqsqihgud.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.fehbvm.com/Article/details/ggyfevbrc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.zdbjq.cn/Article/details/ggeiulfir.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.zdbjq.cn/Article/details/gligalhlb.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wap.zdbjq.cn/Article/details/gyzqpprtj.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gdtepznfi.sHtML

[L03] 设置自定义请求头
来源：http://mobile.fehbvm.com/Article/details/gzexlrbvk.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.hesvh.cn/Article/details/ghtlfiyor.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.hesvh.cn/Article/details/gvzuvbpmh.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gdiplyiix.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/gujusdkkt.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gvbietcwj.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gjlxcodwe.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wap.hesvh.cn/Article/details/glsrdvuea.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gsdduxvtd.sHtML

[L04] 设置超时
来源：http://www.blog.fehbvm.com/Article/details/gddivsfth.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.fehbvm.com/Article/details/gddpfjwgo.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://baike.fehbvm.com/Article/details/gvhrxqfgd.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gmkqexbyj.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gaefdnquj.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.fehbvm.com/Article/details/gzpnifolf.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gyypoflkx.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.hesvh.cn/Article/details/gweilxtjs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/gqqfuvhpw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gmbkrecnj.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gttqreqvz.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gadizybcz.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gaitdqaku.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gcnycajxb.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://read.share.fehbvm.com/Article/details/gzuegexaf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.fehbvm.com/Article/details/gfknrpbjc.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.m.share.zdbjq.cn/Article/details/ggnvzrbay.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.hesvh.cn/Article/details/gxsrtwzaz.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/glxagrtzt.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gifeajpto.sHtML

PHP:  json_decode($body, true);
来源：http://blog.zdbjq.cn/Article/details/glrnxznsf.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gcobbygff.sHtML

TS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gieqbfszp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gwlbjxdlo.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.zdbjq.cn/Article/details/gblikylha.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gpawizlvr.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gvgdobrsm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gxlgbhwep.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.zdbjq.cn/Article/details/gifuiwkum.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gkdiiylfk.sHtML

JS:   resp.ok;  resp.status
来源：http://m.share.zdbjq.cn/Article/details/gamzwwnyw.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.fehbvm.com/Article/details/gztodqjrr.sHtML

Java: resp.statusCode()
来源：http://www.m.share.fehbvm.com/Article/details/gestoeipi.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gjyeqyvjv.sHtML

Ruby: resp.code.to_i
来源：http://m.share.fehbvm.com/Article/details/gdgzwbikq.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gpamruvme.sHtML

[L08] 并发请求多个地址
来源：http://wap.fehbvm.com/Article/details/gzeiqkpwz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.fehbvm.com/Article/details/gbgyvfedv.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gfkmspcbv.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gjiyjaxvf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/ghmpuihji.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.zdbjq.cn/Article/details/giaznxqqu.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.fehbvm.com/Article/details/gdvicljls.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.fehbvm.com/Article/details/gtcrqvmda.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gxqymxosu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcozfcxfn.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gmvtulzpc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnkznyqhi.sHtML

[M01] 读取命令行参数
来源：http://baike.zdbjq.cn/Article/details/gdckckopv.sHtML

Py:   sys.argv[1:]
来源：http://blog.fehbvm.com/Article/details/gdqjyqdxe.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gasfuctpo.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.hesvh.cn/Article/details/gkiclpeiw.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.zdbjq.cn/Article/details/gymbbhifq.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gclqoodvc.sHtML

Go:   os.Args[1:]
来源：http://read.share.fehbvm.com/Article/details/gzufieygi.sHtML

Ruby: ARGV
来源：http://3g.zdbjq.cn/Article/details/gfsxyzzbg.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/grpwxzekn.sHtML

[M02] 读取环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gcgqqgmdx.sHtML

Py:   os.environ.get("HOME")
来源：http://mobile.hesvh.cn/Article/details/gnvijugep.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.fehbvm.com/Article/details/gizvxpgca.sHtML

JS:   process.env.HOME
来源：http://baike.hesvh.cn/Article/details/gigbsuqtb.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gmtdhdojj.sHtML

Java: System.getenv("HOME")
来源：http://www.blog.hesvh.cn/Article/details/gutashvgs.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.hesvh.cn/Article/details/gmeevwosb.sHtML

Ruby: ENV["HOME"]
来源：http://blog.zdbjq.cn/Article/details/gzoembhxu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.fehbvm.com/Article/details/gyicpyttb.sHtML

[M03] 执行外部命令
来源：http://www.m.share.zdbjq.cn/Article/details/gldzsqcjm.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.hesvh.cn/Article/details/gihfrfeoc.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gwklxeffe.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gsdugvpbh.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gqydcdhyx.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.hesvh.cn/Article/details/gjkobqysu.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/grrkxbxtb.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/gvxcxxzih.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.zdbjq.cn/Article/details/gxkkxvwjc.sHtML

[M04] 获取当前工作目录
来源：http://wap.fehbvm.com/Article/details/gvlmthbjy.sHtML

Py:   os.getcwd()
来源：http://www.m.share.fehbvm.com/Article/details/gjpmbsvpg.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/grlzgzhhv.sHtML

JS:   process.cwd()
来源：http://mobile.zdbjq.cn/Article/details/gfekxeepe.sHtML

TS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/giysdmibb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gigveguty.sHtML

Go:   os.Getwd()
来源：http://www.blog.fehbvm.com/Article/details/ganhuveia.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/gjadquccu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.zdbjq.cn/Article/details/gimwxinnr.sHtML

[M05] 设置退出码
来源：http://blog.fehbvm.com/Article/details/gpcsejpfk.sHtML

Py:   sys.exit(1)
来源：http://wap.fehbvm.com/Article/details/gldfdgxno.sHtML

PHP:  exit(1);
来源：http://blog.zdbjq.cn/Article/details/gcshzfxcx.sHtML

JS:   process.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/glkvdaatu.sHtML

TS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gfqupjggn.sHtML

Java: System.exit(1)
来源：http://wap.hesvh.cn/Article/details/gkysgnifp.sHtML

Go:   os.Exit(1)
来源：http://3g.hesvh.cn/Article/details/ghrryrlct.sHtML

Ruby: exit 1
来源：http://3g.fehbvm.com/Article/details/gqfiarksg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gggopexmo.sHtML

[M06] 向标准错误输出
来源：http://m.share.fehbvm.com/Article/details/gukvffday.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.fehbvm.com/Article/details/gcsvdpjdt.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.hesvh.cn/Article/details/gvlfpfqmu.sHtML

JS:   console.error("err")
来源：http://baike.zdbjq.cn/Article/details/gzcytpcrf.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gfldcojkx.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/grlzldqhl.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.hesvh.cn/Article/details/gzvmyqrzy.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gbekxqcms.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/gdjqrhqoz.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gwwnpfyba.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gfaqxsjrt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.m.share.zdbjq.cn/Article/details/gcgxongcf.sHtML

JS:   require.main === module
来源：http://read.share.hesvh.cn/Article/details/gyycsrtkz.sHtML

TS:   require.main === module
来源：http://m.share.zdbjq.cn/Article/details/gmpbswjbo.sHtML

Java: public static void main(String[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gqbkfpkxb.sHtML

Go:   func main()
来源：http://read.share.fehbvm.com/Article/details/gpacyvdos.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/ggcdyqurl.sHtML

C#:   static void Main(string[] args)
来源：http://blog.fehbvm.com/Article/details/ghbiiwphu.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gzjcftvsn.sHtML

Py:   platform.system();  platform.python_version()
来源：http://blog.fehbvm.com/Article/details/gqujmaupj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.hesvh.cn/Article/details/gvdfoytid.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gjokduwwh.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gelhpvynn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/glhdicvdz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gwjkwywbw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gcllmcozl.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.zdbjq.cn/Article/details/gdumhbswn.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gigpmbodm.sHtML

N. 数据结构与算法
来源：http://blog.fehbvm.com/Article/details/gcquxazme.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gnaqtkezt.sHtML

[N01] 二分查找（有序数组）
来源：http://www.m.share.fehbvm.com/Article/details/geqggljin.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.fehbvm.com/Article/details/gqjexaaoa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gamxxnmaa.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.share.hesvh.cn/Article/details/gyzcwogsh.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.fehbvm.com/Article/details/geelsbmps.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gpclaqyqk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.fehbvm.com/Article/details/gqyaldpio.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gtulezqfv.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gggzhylly.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.zdbjq.cn/Article/details/gicooemjm.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.hesvh.cn/Article/details/giicoezwv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://blog.hesvh.cn/Article/details/gukzmkqus.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.fehbvm.com/Article/details/gjscrqwiw.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.zdbjq.cn/Article/details/ghndhujro.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.zdbjq.cn/Article/details/gsyhjehau.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.hesvh.cn/Article/details/gbowxakky.sHtML

Ruby: arr.sort
来源：http://3g.hesvh.cn/Article/details/gagbfhvoq.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://wap.zdbjq.cn/Article/details/galcnhltk.sHtML

[N03] 快速排序（分治示例）
来源：http://www.m.share.zdbjq.cn/Article/details/ghrjhclob.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.zdbjq.cn/Article/details/gtbxelwhf.sHtML

PHP:  // 递归实现，或用 usort
来源：http://m.share.fehbvm.com/Article/details/gdtaoxpzn.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wap.hesvh.cn/Article/details/gaxwsjlwd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/gdoaicfkt.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gaoxivdfc.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.zdbjq.cn/Article/details/gvquurnoy.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.hesvh.cn/Article/details/gsiibwxwg.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.fehbvm.com/Article/details/ghlurhiof.sHtML

[N04] 斐波那契数列
来源：http://m.share.zdbjq.cn/Article/details/gdweggdmy.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://read.share.fehbvm.com/Article/details/gnwqhhewl.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://3g.fehbvm.com/Article/details/gxtlhxwvx.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.zdbjq.cn/Article/details/ghodvxuut.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/gmerqrycp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fehbvm.com/Article/details/gjokhxwfe.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mobile.zdbjq.cn/Article/details/gatvwsqwr.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.zdbjq.cn/Article/details/gpnmnvshm.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mobile.hesvh.cn/Article/details/gdhsgsvhq.sHtML

[N05] 最大公约数
来源：http://wap.hesvh.cn/Article/details/gvbbkmolq.sHtML

Py:   math.gcd(a, b)
来源：http://mobile.zdbjq.cn/Article/details/gbmtbnlom.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://3g.hesvh.cn/Article/details/gybbflncy.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.zdbjq.cn/Article/details/gcxicjnfl.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.zdbjq.cn/Article/details/gjhfrkjrc.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://3g.fehbvm.com/Article/details/gfvpnplvf.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://read.share.zdbjq.cn/Article/details/guapujkeq.sHtML

Ruby: a.gcd(b)
来源：http://baike.hesvh.cn/Article/details/geuhzfrgb.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.hesvh.cn/Article/details/gyphvqwra.sHtML

[N06] 判断回文字符串
来源：http://www.share.hesvh.cn/Article/details/gwpmhjits.sHtML

Py:   s == s[::-1]
来源：http://baike.fehbvm.com/Article/details/ggzpeuphj.sHtML

PHP:  $s === strrev($s);
来源：http://read.share.fehbvm.com/Article/details/gcfwlvxzb.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/grfwakhhh.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gajwaikkq.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.zdbjq.cn/Article/details/gqqpojwuy.sHtML

Go:   // 双指针从两端比较
来源：http://www.blog.hesvh.cn/Article/details/goqdnhbnu.sHtML

Ruby: s == s.reverse
来源：http://baike.zdbjq.cn/Article/details/gjtbtqtpe.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/geyiqdiyx.sHtML

[N07] 两数之和（返回下标）
来源：http://www.share.fehbvm.com/Article/details/gpctjbysh.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gfxcdhmis.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://blog.fehbvm.com/Article/details/gejomsgwi.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://read.share.fehbvm.com/Article/details/gfzpsqzbk.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.hesvh.cn/Article/details/gbkbzfvjb.sHtML

Java: // 手写 HashMap
来源：http://3g.zdbjq.cn/Article/details/gcuukqccr.sHtML

Go:   // 手写 map[int]int
来源：http://3g.fehbvm.com/Article/details/gafwwuypg.sHtML

Ruby: // 手写 Hash
来源：http://m.share.zdbjq.cn/Article/details/gvgymdikw.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.share.hesvh.cn/Article/details/gawtnzttf.sHtML

[N08] 生成全排列
来源：http://read.share.zdbjq.cn/Article/details/ghmeismlr.sHtML


<!-- 参考信息 -->