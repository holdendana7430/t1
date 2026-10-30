代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.zdbjq.cn/Article/details/gxtmstjfn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.fehbvm.com/Article/details/gyemboalz.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/gkninsnek.sHtML

[J10] 取今天 / 本月第一天
来源：http://read.share.fehbvm.com/Article/details/ggimdumav.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://baike.fehbvm.com/Article/details/gfxdptoth.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/guhkiztvx.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://blog.zdbjq.cn/Article/details/gyoigulpt.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gugyaampo.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://blog.fehbvm.com/Article/details/gdaqxqnhr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gyjmumcmd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wap.hesvh.cn/Article/details/gdcijrrbz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.hesvh.cn/Article/details/gqikigfek.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/ghoamxdqe.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gdhskijon.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gythrtpug.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.hesvh.cn/Article/details/gyxkylrgt.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/geuzkifay.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/ghrkpokvh.sHtML

JS:   JSON.stringify(obj)
来源：http://baike.hesvh.cn/Article/details/glkxoqpve.sHtML

TS:   JSON.stringify(obj)
来源：http://blog.zdbjq.cn/Article/details/ggrjzbpih.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.fehbvm.com/Article/details/gyifogdem.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gthmrrozk.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gjajpkpyr.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gurthlaqv.sHtML

[K02] JSON 字符串转对象
来源：http://3g.zdbjq.cn/Article/details/ghpdlcvht.sHtML

Py:   json.loads(s)
来源：http://www.m.share.fehbvm.com/Article/details/gmrbaxnwa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/gcxuufsbv.sHtML

JS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gyzmxxrfx.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gacbnshlm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/gfigthidc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://wap.fehbvm.com/Article/details/gvreonjrf.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.zdbjq.cn/Article/details/glvupmktk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.fehbvm.com/Article/details/glksymkup.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://wap.hesvh.cn/Article/details/gnbdccoxj.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.zdbjq.cn/Article/details/gsbuqotnp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gbusjplyd.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gczzxmtyb.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/ggyywnzpd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.hesvh.cn/Article/details/ghuhdrquf.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.fehbvm.com/Article/details/gqxkggkhy.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.share.zdbjq.cn/Article/details/gvjbfeeaw.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gwdsftkka.sHtML

[K04] 读取 JSON 文件
来源：http://www.blog.zdbjq.cn/Article/details/gsjevigyw.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.hesvh.cn/Article/details/gvtwgxmmg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/glcsirpub.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.zdbjq.cn/Article/details/gfcbynfzl.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.zdbjq.cn/Article/details/gqzpvzeus.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gazzrbuwl.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gworzdohq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.fehbvm.com/Article/details/gctgmxqmz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/guwjdqzru.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/ghadjjepx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.blog.fehbvm.com/Article/details/goiirepxb.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gqiujzqyc.sHtML

JS:   structuredClone(obj)
来源：http://baike.hesvh.cn/Article/details/gxfvcqzif.sHtML

TS:   structuredClone(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gbrwtkihi.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.zdbjq.cn/Article/details/gdqbwapmq.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gzmlzzixd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wap.hesvh.cn/Article/details/gmhjvyase.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/ghwhqutei.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gprrcjwix.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.hesvh.cn/Article/details/gjnpswcuc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.fehbvm.com/Article/details/gbbpfqyfx.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.zdbjq.cn/Article/details/gulafnbce.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gccfaumjv.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/ghingxcpx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gfbkozsxz.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/glgzxmrdn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/gkqeybrik.sHtML

[K07] 进制转换
来源：http://www.blog.fehbvm.com/Article/details/gqomtazcw.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gsyevigjo.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gzyofznuz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/grsgtamal.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gnosjyshl.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gkbkskgvj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://mobile.hesvh.cn/Article/details/ggihocumw.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.zdbjq.cn/Article/details/gjajmoghq.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gbyuayeal.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gbwqfoewz.sHtML

Py:   pickle.dumps(obj)
来源：http://read.share.hesvh.cn/Article/details/ghqlfvydw.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://read.share.fehbvm.com/Article/details/gfajyyobr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://mobile.hesvh.cn/Article/details/grgaljufa.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gokoyrhhy.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.blog.fehbvm.com/Article/details/ggisegfgw.sHtML

Go:   encoding/gob
来源：http://www.blog.fehbvm.com/Article/details/gskqjkyxr.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.fehbvm.com/Article/details/gbctxrdfe.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gbpavbejm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvlscbmgi.sHtML

L. 网络请求
来源：http://m.share.hesvh.cn/Article/details/gurkutiht.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/ggiovhssg.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gsebzrssx.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gcabwhhxr.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://blog.zdbjq.cn/Article/details/gtaameodt.sHtML

JS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gpioapkme.sHtML

TS:   await fetch(url)
来源：http://www.blog.fehbvm.com/Article/details/gtkkziiig.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gfjzwtlnj.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.fehbvm.com/Article/details/gkgdpeybt.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gsiuicxgt.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/glwfqcefo.sHtML

[L02] 发送 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gzaygaszq.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://read.share.zdbjq.cn/Article/details/gmrztqmxe.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://3g.zdbjq.cn/Article/details/gotbodafg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/guvxykhhh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/ghgxhljkq.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.fehbvm.com/Article/details/goamigbxx.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.fehbvm.com/Article/details/gflztcwbi.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.fehbvm.com/Article/details/ghqiqrbkv.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gazitexxb.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gwizfyyvc.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.hesvh.cn/Article/details/ggmpmzhgn.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.share.hesvh.cn/Article/details/ggaltyuiy.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.zdbjq.cn/Article/details/goeluxlfw.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gghtwekoo.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gkmrymzwz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://baike.fehbvm.com/Article/details/gagbudgzc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.hesvh.cn/Article/details/gjrbosaly.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.hesvh.cn/Article/details/gsleuhjbc.sHtML

[L04] 设置超时
来源：http://baike.zdbjq.cn/Article/details/gesjmnxyw.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gudlpgdwb.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://blog.zdbjq.cn/Article/details/gksrzdsym.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gdexvxtlp.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gfwmhwswv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.fehbvm.com/Article/details/gusbbqtxq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gskssbuqy.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wap.zdbjq.cn/Article/details/gmuzvshuq.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.zdbjq.cn/Article/details/gpfymouki.sHtML

[L05] 上传文件（multipart）
来源：http://read.share.hesvh.cn/Article/details/gzdlrwcui.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gpnpzqzyt.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.zdbjq.cn/Article/details/gzzjmetly.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.fehbvm.com/Article/details/gjwyelvly.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.fehbvm.com/Article/details/goxfjwtuq.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gwtxxxyhr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gqxwtypyp.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/gslvsphpa.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gbryxcuid.sHtML

[L06] 解析响应为 JSON
来源：http://3g.zdbjq.cn/Article/details/gibduzjny.sHtML

Py:   resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gtoialfna.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.zdbjq.cn/Article/details/gbswwajat.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gyolvufrl.sHtML

TS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/gehdurpqw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.hesvh.cn/Article/details/gswuzhyoi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/ghkgqevmi.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/grhrscgfp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.fehbvm.com/Article/details/gkjquumuj.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gzxuloutr.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://blog.zdbjq.cn/Article/details/gbnnuvabf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gyhrzyvll.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.hesvh.cn/Article/details/gjdmncumq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.hesvh.cn/Article/details/gfsqsngak.sHtML

Java: resp.statusCode()
来源：http://mobile.zdbjq.cn/Article/details/gcskcwjaa.sHtML

Go:   resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gqfbrzrcu.sHtML

Ruby: resp.code.to_i
来源：http://baike.fehbvm.com/Article/details/gxjzgubtp.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.fehbvm.com/Article/details/gjczjmfdi.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gkdpwafud.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.hesvh.cn/Article/details/gsqkyaian.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.blog.zdbjq.cn/Article/details/gzirfvdmz.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/golukhspv.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.hesvh.cn/Article/details/gquzkjbti.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mobile.fehbvm.com/Article/details/gglfpkaey.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gvwazcrex.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://read.share.zdbjq.cn/Article/details/gpffreons.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gpdhofkzj.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gjveluhun.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/gmxfcvmea.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxgylmbso.sHtML

[M01] 读取命令行参数
来源：http://wap.hesvh.cn/Article/details/gpxczhijr.sHtML

Py:   sys.argv[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gmnfmmuxv.sHtML

PHP:  $argv;  $argc;
来源：http://3g.hesvh.cn/Article/details/goxgpocya.sHtML

JS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gvbxkiwja.sHtML

TS:   process.argv.slice(2)
来源：http://m.share.fehbvm.com/Article/details/gqtvgnzss.sHtML

Java: args 数组（main 方法参数）
来源：http://baike.fehbvm.com/Article/details/gbyrcikju.sHtML

Go:   os.Args[1:]
来源：http://read.share.zdbjq.cn/Article/details/gnltwzhdl.sHtML

Ruby: ARGV
来源：http://mobile.zdbjq.cn/Article/details/gakyemcbd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gjgmwnvwb.sHtML

[M02] 读取环境变量
来源：http://read.share.hesvh.cn/Article/details/gihxqvmuz.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gvcvcacwq.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.blog.hesvh.cn/Article/details/gjiihlmcd.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gmsbvmyyp.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gzvvntpdy.sHtML

Java: System.getenv("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gprzacmwj.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gasibmicq.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.zdbjq.cn/Article/details/gghjpejgf.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/ggimhkidn.sHtML

[M03] 执行外部命令
来源：http://baike.hesvh.cn/Article/details/gpadpefcx.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.zdbjq.cn/Article/details/gfqhodfga.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/ggrwixwjj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/gpxyyhxxk.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.hesvh.cn/Article/details/goxtayzcu.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.zdbjq.cn/Article/details/gpaxkrnoi.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://read.share.zdbjq.cn/Article/details/guvuddlng.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.zdbjq.cn/Article/details/grjhblwas.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.hesvh.cn/Article/details/gisvytbhx.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.hesvh.cn/Article/details/glwiblaih.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/gyhrvlewc.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/gcliyxmyq.sHtML

JS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/gzindgjro.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gjpivnbcw.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://read.share.hesvh.cn/Article/details/gzifsyfqo.sHtML

Go:   os.Getwd()
来源：http://www.m.share.zdbjq.cn/Article/details/gfsmcahmw.sHtML

Ruby: Dir.pwd
来源：http://m.share.zdbjq.cn/Article/details/gacbudasi.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.zdbjq.cn/Article/details/giuzmpnjp.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gcgqkxvfu.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghfiyvwoc.sHtML

PHP:  exit(1);
来源：http://www.blog.fehbvm.com/Article/details/gypnxtlfw.sHtML

JS:   process.exit(1)
来源：http://www.share.hesvh.cn/Article/details/gdsqtugda.sHtML

TS:   process.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gygxjwmbb.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gelktsfmd.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gqevegweh.sHtML

Ruby: exit 1
来源：http://www.blog.fehbvm.com/Article/details/gqcxxobcv.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wap.hesvh.cn/Article/details/glbcyoplv.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gobbzextx.sHtML

Py:   print("err", file=sys.stderr)
来源：http://wap.fehbvm.com/Article/details/gzavdtgzp.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/ghivqzvuj.sHtML

JS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gmsjccdkr.sHtML

TS:   console.error("err")
来源：http://read.share.zdbjq.cn/Article/details/gntudrikq.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gzvisuccj.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gtzpjclkj.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/ggdykowuo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.hesvh.cn/Article/details/gtvrlpdyf.sHtML

[M07] 判断是否为主入口
来源：http://blog.zdbjq.cn/Article/details/gwptddnjm.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/guagkgrrw.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.fehbvm.com/Article/details/gnysnwahn.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gmhudzrrr.sHtML

TS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/gyzgqwsik.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/gmjrvmgnj.sHtML

Go:   func main()
来源：http://m.share.zdbjq.cn/Article/details/gnykxnvet.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/guvfbasfu.sHtML

C#:   static void Main(string[] args)
来源：http://wap.fehbvm.com/Article/details/ghvjzfvda.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/gntaeuvcy.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.fehbvm.com/Article/details/guasnices.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gtxwyjyek.sHtML

JS:   process.platform;  process.version
来源：http://www.m.share.hesvh.cn/Article/details/gksuugoik.sHtML

TS:   process.platform;  process.version
来源：http://m.share.zdbjq.cn/Article/details/gtsofmjhh.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gpcyqtixx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://blog.zdbjq.cn/Article/details/gbxjlmcgb.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gqxueclhz.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gsoahygrd.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpmovzsnw.sHtML

N. 数据结构与算法
来源：http://read.share.zdbjq.cn/Article/details/gybkaetxw.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/grldpphkk.sHtML

[N01] 二分查找（有序数组）
来源：http://read.share.fehbvm.com/Article/details/gtwtqmryb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://wap.fehbvm.com/Article/details/gbpxuznss.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wap.zdbjq.cn/Article/details/grxvswtww.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gmeynrxuu.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gdokbqbxz.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.hesvh.cn/Article/details/gqlhcaaxg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://m.share.hesvh.cn/Article/details/gpdpjilyl.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/guidspowc.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gavuazedv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/giiavtaez.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://blog.hesvh.cn/Article/details/gtvromcyo.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.fehbvm.com/Article/details/gmrkfiktw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gdgfusefl.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gjmsdynru.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://baike.fehbvm.com/Article/details/gqudtxjuc.sHtML

Go:   slices.Sort(arr)
来源：http://baike.hesvh.cn/Article/details/gmsomzjej.sHtML

Ruby: arr.sort
来源：http://mobile.fehbvm.com/Article/details/ggtuwmaqs.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.zdbjq.cn/Article/details/gyierzyjy.sHtML

[N03] 快速排序（分治示例）
来源：http://m.share.fehbvm.com/Article/details/gnnjvtxjr.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gwjoaegry.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.zdbjq.cn/Article/details/gtlstltbu.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gimbwxcyn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.zdbjq.cn/Article/details/grpdjnwoe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://baike.zdbjq.cn/Article/details/gwlxcrrln.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mobile.hesvh.cn/Article/details/gsncbhlxa.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.hesvh.cn/Article/details/gjzdwbkpr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://wap.fehbvm.com/Article/details/ginblfpbk.sHtML

[N04] 斐波那契数列
来源：http://wap.fehbvm.com/Article/details/grcnfsfxf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.fehbvm.com/Article/details/gsrypydxv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.hesvh.cn/Article/details/gqnivvdmo.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://m.share.zdbjq.cn/Article/details/gacosjpvu.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.fehbvm.com/Article/details/ginmagaxb.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.hesvh.cn/Article/details/gxkpfgodk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/ghifkajfw.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gaeidnsob.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.m.share.zdbjq.cn/Article/details/ghbakyeao.sHtML

[N05] 最大公约数
来源：http://mobile.hesvh.cn/Article/details/ghdugavzb.sHtML

Py:   math.gcd(a, b)
来源：http://m.share.fehbvm.com/Article/details/glpqhvwmk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.hesvh.cn/Article/details/gsalryber.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.zdbjq.cn/Article/details/gyjnveaaz.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.blog.fehbvm.com/Article/details/ghrnzllrw.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.fehbvm.com/Article/details/gajyxjcce.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.fehbvm.com/Article/details/gyarmsyyi.sHtML

Ruby: a.gcd(b)
来源：http://mobile.fehbvm.com/Article/details/gadwbdbpg.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.zdbjq.cn/Article/details/gumevulmy.sHtML

[N06] 判断回文字符串
来源：http://3g.zdbjq.cn/Article/details/gvygywbvi.sHtML

Py:   s == s[::-1]
来源：http://blog.fehbvm.com/Article/details/gthsbtcjl.sHtML

PHP:  $s === strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/gybwrlhjy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gemxiwbvx.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gzinbrrgn.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.share.fehbvm.com/Article/details/gidkjszsn.sHtML

Go:   // 双指针从两端比较
来源：http://read.share.hesvh.cn/Article/details/gpobjftcc.sHtML

Ruby: s == s.reverse
来源：http://3g.fehbvm.com/Article/details/grfwcbbzp.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gegsktjib.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.hesvh.cn/Article/details/gndftolex.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.zdbjq.cn/Article/details/gphhykuso.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://read.share.fehbvm.com/Article/details/gdaneqqro.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://wap.zdbjq.cn/Article/details/gcrkpjvrh.sHtML

TS:   // 手写 Map<string, number>
来源：http://www.share.zdbjq.cn/Article/details/ginflnsey.sHtML

Java: // 手写 HashMap
来源：http://m.share.fehbvm.com/Article/details/gmvpgzfpn.sHtML


<!-- 参考信息 -->