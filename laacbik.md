代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.zdbjq.cn/Article/details/gvahkgzkg.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.fehbvm.com/Article/details/gyxgkpsgm.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gwwpeqcug.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.fehbvm.com/Article/details/gtzwdemcx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.zdbjq.cn/Article/details/gaxbqvlqj.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.zdbjq.cn/Article/details/gcxvxhozm.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://read.share.zdbjq.cn/Article/details/gcienjatx.sHtML

[J10] 取今天 / 本月第一天
来源：http://wap.fehbvm.com/Article/details/gaskinxkb.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/grnblytgh.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.zdbjq.cn/Article/details/gzvvpldvz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.zdbjq.cn/Article/details/gfivdeika.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/grqrkgogh.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://mobile.hesvh.cn/Article/details/gvnxkchkn.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.blog.fehbvm.com/Article/details/gjwnpnjvm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/ghiwmozzu.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.blog.fehbvm.com/Article/details/gabyctije.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gajuiqbaq.sHtML

K. JSON 与序列化
来源：http://blog.hesvh.cn/Article/details/gywjnmtlw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gcfvgvooq.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/ggvgdupsv.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gfroieykz.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.zdbjq.cn/Article/details/gxezmiqnc.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.hesvh.cn/Article/details/grkxaxxig.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.zdbjq.cn/Article/details/gqiawgodw.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gnjdhmkeo.sHtML

Go:   json.Marshal(obj)
来源：http://3g.fehbvm.com/Article/details/gevcbptrh.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gehfxrkbg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.share.fehbvm.com/Article/details/gigaxrpao.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.zdbjq.cn/Article/details/gburqlyqz.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gbyrdzqul.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.share.hesvh.cn/Article/details/gwvvkzgga.sHtML

JS:   JSON.parse(s)
来源：http://baike.hesvh.cn/Article/details/gaaxxpego.sHtML

TS:   JSON.parse(s)
来源：http://baike.zdbjq.cn/Article/details/ggezhpuje.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.hesvh.cn/Article/details/guxwyewvd.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://mobile.fehbvm.com/Article/details/gksouxlzc.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gdooxzqjh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.hesvh.cn/Article/details/gpgvfgsxn.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.m.share.hesvh.cn/Article/details/gcczeruhq.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/ggxpbyapl.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gykflyrak.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gdaavhlhg.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gzybzsofe.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gjttlkyvm.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/gufnxyumf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gtrdmrydd.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/gllytibnf.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gnvhjugix.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wap.fehbvm.com/Article/details/gknaggfxn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.fehbvm.com/Article/details/gbfgrwbyb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gknwosbvz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.fehbvm.com/Article/details/ggfsthytx.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.hesvh.cn/Article/details/gdxtzvyng.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gdgpbgtry.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gqmhettnz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gohugfliy.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gtnjwyuuu.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.zdbjq.cn/Article/details/gjzxptqrg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.zdbjq.cn/Article/details/gdoiorhap.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/griruvure.sHtML

TS:   structuredClone(obj)
来源：http://baike.zdbjq.cn/Article/details/gnnxfitsx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://m.share.hesvh.cn/Article/details/gvbdbglev.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/gffwvecgd.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.fehbvm.com/Article/details/gyxkynzfi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/ggfsnlequ.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.fehbvm.com/Article/details/gdlaqxvwm.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.hesvh.cn/Article/details/gjmwfqxmt.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.zdbjq.cn/Article/details/gsycmhlbj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.zdbjq.cn/Article/details/gpgrtvrjn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gypctfyag.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.zdbjq.cn/Article/details/gbbkkiizn.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://m.share.zdbjq.cn/Article/details/gaylvjxsk.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/grfggmbgg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gifmjbxbs.sHtML

[K07] 进制转换
来源：http://wap.fehbvm.com/Article/details/gsyakgucx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://3g.fehbvm.com/Article/details/ghzsgxklu.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gbjbysrgz.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gdwjnhiwl.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gkrvbosrr.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gescscwqn.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/ggnnxuxgu.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://3g.hesvh.cn/Article/details/gazsmlusf.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/gdwvuryzz.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gghydjkjf.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.hesvh.cn/Article/details/gdosofohk.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.zdbjq.cn/Article/details/gyzsleiyv.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/geqaelmzt.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/geojyxnpi.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.fehbvm.com/Article/details/gszzcibbn.sHtML

Go:   encoding/gob
来源：http://baike.zdbjq.cn/Article/details/gzzjohtlv.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.hesvh.cn/Article/details/ggnowpgvs.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://3g.hesvh.cn/Article/details/gdddqbfbs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gblabwoyn.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gsetiqxaz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gvbtqensg.sHtML

[L01] 发送 GET 请求
来源：http://read.share.zdbjq.cn/Article/details/gbuyfqhvs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.hesvh.cn/Article/details/gveqqfgvd.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/guxuppgdn.sHtML

JS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/gbprdrano.sHtML

TS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/gahrpalxv.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://m.share.hesvh.cn/Article/details/gqdnseorq.sHtML

Go:   resp, err := http.Get(url)
来源：http://mobile.fehbvm.com/Article/details/gvliyyklq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://baike.hesvh.cn/Article/details/gpantaimj.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mobile.fehbvm.com/Article/details/grwmjtktl.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gdqoxbwem.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://3g.zdbjq.cn/Article/details/gsglqquob.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.hesvh.cn/Article/details/gqyrsvvmg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.hesvh.cn/Article/details/gbmhsjwiz.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.hesvh.cn/Article/details/gocehvyxs.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.zdbjq.cn/Article/details/gfxjiqiaw.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gjccpxptl.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gbuycfkys.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://m.share.zdbjq.cn/Article/details/gowjrhajx.sHtML

[L03] 设置自定义请求头
来源：http://m.share.fehbvm.com/Article/details/gpoefezck.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.fehbvm.com/Article/details/gnqfrklip.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.hesvh.cn/Article/details/gguhgyqko.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/grlholrhf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://3g.hesvh.cn/Article/details/gthosgbcg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.zdbjq.cn/Article/details/gcxoyajkv.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/guoktrjhp.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gtqcskjya.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.fehbvm.com/Article/details/gorpjjsei.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gbzpxqslh.sHtML

Py:   requests.get(url, timeout=5)
来源：http://mobile.fehbvm.com/Article/details/gqcuewafr.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gtfypruvz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.fehbvm.com/Article/details/gxhpjmwdi.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.fehbvm.com/Article/details/ggoqylwmv.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.hesvh.cn/Article/details/gvzacjeca.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.m.share.zdbjq.cn/Article/details/gnwhkjkdh.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.zdbjq.cn/Article/details/gyixlwljx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.hesvh.cn/Article/details/gqslhjjmk.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gneowjpbx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.fehbvm.com/Article/details/gxvoxbicd.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gwmcmhcez.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gubkcklnn.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/grugeagzp.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/gfpggguuf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://m.share.hesvh.cn/Article/details/gnrwqnxok.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.fehbvm.com/Article/details/gtkzzoghf.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://3g.zdbjq.cn/Article/details/gfialopme.sHtML

[L06] 解析响应为 JSON
来源：http://www.m.share.fehbvm.com/Article/details/gkbueviyr.sHtML

Py:   resp.json()
来源：http://3g.fehbvm.com/Article/details/gwudjhlya.sHtML

PHP:  json_decode($body, true);
来源：http://www.share.fehbvm.com/Article/details/gvpmlsxut.sHtML

JS:   await resp.json()
来源：http://www.m.share.hesvh.cn/Article/details/gzwlvokot.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/goxxrrzzu.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.fehbvm.com/Article/details/gjdglbjhx.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.zdbjq.cn/Article/details/gdhzwdonv.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.blog.zdbjq.cn/Article/details/gprcyfeby.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://baike.zdbjq.cn/Article/details/gwymkwdab.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gukltelvx.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.share.fehbvm.com/Article/details/gvoncoyzu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.zdbjq.cn/Article/details/gdebjbkfa.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gyloznecb.sHtML

TS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gasajyogy.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gvzannjuv.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gzklavjhu.sHtML

Ruby: resp.code.to_i
来源：http://read.share.zdbjq.cn/Article/details/gnfxgvfhp.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.fehbvm.com/Article/details/gtkypuanr.sHtML

[L08] 并发请求多个地址
来源：http://m.share.fehbvm.com/Article/details/gxeiampbb.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wap.zdbjq.cn/Article/details/gbfetypvo.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.share.fehbvm.com/Article/details/gwtuuhnzm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.zdbjq.cn/Article/details/gvuhlsgei.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.fehbvm.com/Article/details/gqrggdctg.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gzxrmrjai.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.hesvh.cn/Article/details/getmfplab.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/gxabobile.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gzwkpspth.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gvzjftlep.sHtML

M. 命令行 / 进程 / 环境
来源：http://m.share.zdbjq.cn/Article/details/gmfvulzbl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzanqgkeh.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gsyymxoxi.sHtML

Py:   sys.argv[1:]
来源：http://mobile.hesvh.cn/Article/details/gwccibbbw.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/gasgkbuzk.sHtML

JS:   process.argv.slice(2)
来源：http://baike.zdbjq.cn/Article/details/gnqpwxaak.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gkfxaghtb.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gppydknqs.sHtML

Go:   os.Args[1:]
来源：http://www.blog.hesvh.cn/Article/details/gkgdoabtr.sHtML

Ruby: ARGV
来源：http://blog.fehbvm.com/Article/details/gutjrvpxq.sHtML

C#:   args 数组（Main 方法参数）
来源：http://blog.hesvh.cn/Article/details/gikaicwxl.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gnjfbxitg.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/glcemabyt.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.zdbjq.cn/Article/details/gmdaeaxwp.sHtML

JS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gnzamjkuj.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/glzebbllo.sHtML

Java: System.getenv("HOME")
来源：http://baike.fehbvm.com/Article/details/gacykvsid.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.share.hesvh.cn/Article/details/gimqenfiz.sHtML

Ruby: ENV["HOME"]
来源：http://3g.fehbvm.com/Article/details/guahihyrw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gnojsaxrj.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/geqsnzrlg.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.hesvh.cn/Article/details/gulffgbag.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gdegxcttr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.zdbjq.cn/Article/details/gdefbrtgd.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/grsggutqn.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.share.hesvh.cn/Article/details/ggaconhuw.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.hesvh.cn/Article/details/gpogclrsw.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://mobile.zdbjq.cn/Article/details/gtawacluf.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/gesbjcxne.sHtML

[M04] 获取当前工作目录
来源：http://wap.zdbjq.cn/Article/details/gqxkyjxnf.sHtML

Py:   os.getcwd()
来源：http://www.blog.fehbvm.com/Article/details/gobqduncp.sHtML

PHP:  getcwd();
来源：http://mobile.hesvh.cn/Article/details/gujyxtneh.sHtML

JS:   process.cwd()
来源：http://read.share.fehbvm.com/Article/details/gzchpqqpe.sHtML

TS:   process.cwd()
来源：http://wap.zdbjq.cn/Article/details/gqzymxjwx.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.hesvh.cn/Article/details/gpsbpspbu.sHtML

Go:   os.Getwd()
来源：http://read.share.hesvh.cn/Article/details/gvdppmooz.sHtML

Ruby: Dir.pwd
来源：http://read.share.hesvh.cn/Article/details/gjcyoxzwz.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gurltogue.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gtnvuwzxx.sHtML

Py:   sys.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/grpblvhkn.sHtML

PHP:  exit(1);
来源：http://3g.hesvh.cn/Article/details/gjtbuwuii.sHtML

JS:   process.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gtxwdnsdj.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gvddxlujd.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gicaapmkw.sHtML

Go:   os.Exit(1)
来源：http://wap.fehbvm.com/Article/details/gjenodiws.sHtML

Ruby: exit 1
来源：http://blog.fehbvm.com/Article/details/gbfssachb.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mobile.hesvh.cn/Article/details/gemsniruy.sHtML

[M06] 向标准错误输出
来源：http://read.share.hesvh.cn/Article/details/gpwerpumj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://blog.fehbvm.com/Article/details/gvjuyawoq.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://3g.hesvh.cn/Article/details/geptnzgaj.sHtML

JS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gjpanxsdn.sHtML

TS:   console.error("err")
来源：http://blog.zdbjq.cn/Article/details/ghvibyipx.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/grmurdodn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/guzeydrob.sHtML

Ruby: warn "err"
来源：http://3g.fehbvm.com/Article/details/gkjylabel.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.hesvh.cn/Article/details/goqhdzqxh.sHtML

[M07] 判断是否为主入口
来源：http://www.blog.zdbjq.cn/Article/details/ghqzrdzyp.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gabhbsrhd.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.zdbjq.cn/Article/details/glxytiyxw.sHtML

JS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gwbyjluik.sHtML

TS:   require.main === module
来源：http://3g.hesvh.cn/Article/details/gsxcrohqd.sHtML

Java: public static void main(String[] args)
来源：http://www.share.hesvh.cn/Article/details/gtcouzavj.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/ghtvopyvn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.zdbjq.cn/Article/details/gjujyqzqy.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.hesvh.cn/Article/details/gzywsgbtb.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.fehbvm.com/Article/details/gjgxfipxr.sHtML

Py:   platform.system();  platform.python_version()
来源：http://wap.zdbjq.cn/Article/details/ggkjiyjts.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/glhlssosd.sHtML

JS:   process.platform;  process.version
来源：http://blog.hesvh.cn/Article/details/gcssceirh.sHtML

TS:   process.platform;  process.version
来源：http://baike.zdbjq.cn/Article/details/gaunagdix.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.hesvh.cn/Article/details/gwrczpiqr.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/gwzkcxmug.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://blog.hesvh.cn/Article/details/gntdoeaqa.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/grihdkems.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghwvhgiwr.sHtML

N. 数据结构与算法
来源：http://wap.hesvh.cn/Article/details/ghfuxdcry.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gfcdnxbhr.sHtML

[N01] 二分查找（有序数组）
来源：http://mobile.zdbjq.cn/Article/details/grffloaom.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://baike.hesvh.cn/Article/details/gpqjxkrpz.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.share.hesvh.cn/Article/details/gjauetrqy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.fehbvm.com/Article/details/ggjqecvnj.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.hesvh.cn/Article/details/gktuneuka.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gbylzepxl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gwpfixtyb.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.zdbjq.cn/Article/details/gvzwwkfiq.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gentqvwjn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gtvwyvbfx.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gohdcngjl.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gbzbebctf.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://wap.fehbvm.com/Article/details/gsukipmbi.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.hesvh.cn/Article/details/gsrxqwuwt.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gossgkpqz.sHtML

Go:   slices.Sort(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gbkgovyew.sHtML

Ruby: arr.sort
来源：http://www.share.zdbjq.cn/Article/details/gosfosctv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.hesvh.cn/Article/details/gyokavzmf.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gxdzldfxc.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wap.zdbjq.cn/Article/details/gtlomkjoo.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.hesvh.cn/Article/details/gehsudpmx.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.hesvh.cn/Article/details/gmisfywaw.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://read.share.zdbjq.cn/Article/details/goauuvreb.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://blog.hesvh.cn/Article/details/giiwcpfsd.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.m.share.hesvh.cn/Article/details/gjurhurqu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.share.zdbjq.cn/Article/details/gwcticbrn.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.fehbvm.com/Article/details/gapiohkop.sHtML

[N04] 斐波那契数列
来源：http://m.share.fehbvm.com/Article/details/gklgpfdjf.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.hesvh.cn/Article/details/grvklkdlf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gzjzslrsm.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gdoymzlcr.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.hesvh.cn/Article/details/guvumymim.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://m.share.zdbjq.cn/Article/details/gvjqwhhil.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.fehbvm.com/Article/details/gtbehbyso.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.blog.hesvh.cn/Article/details/gvxogzfpv.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://read.share.hesvh.cn/Article/details/gvysxseel.sHtML

[N05] 最大公约数
来源：http://www.m.share.hesvh.cn/Article/details/gjafulnta.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.zdbjq.cn/Article/details/gappvnxaj.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.blog.fehbvm.com/Article/details/gglklarps.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://blog.hesvh.cn/Article/details/gfttaeyct.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.fehbvm.com/Article/details/guyurxkto.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://read.share.hesvh.cn/Article/details/gfohogfgr.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://3g.hesvh.cn/Article/details/gxipejrkm.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gteivwfyh.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://www.share.zdbjq.cn/Article/details/godmmzyrf.sHtML

[N06] 判断回文字符串
来源：http://mobile.fehbvm.com/Article/details/gxjjpjfkp.sHtML

Py:   s == s[::-1]
来源：http://www.m.share.fehbvm.com/Article/details/gjzcwtqhw.sHtML

PHP:  $s === strrev($s);
来源：http://blog.fehbvm.com/Article/details/ggywknhjy.sHtML

JS:   s === [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/geccupcmg.sHtML

TS:   s === [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gvlnfphib.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://read.share.zdbjq.cn/Article/details/gjkdxzqzj.sHtML

Go:   // 双指针从两端比较
来源：http://3g.fehbvm.com/Article/details/gwfsdyarj.sHtML

Ruby: s == s.reverse
来源：http://read.share.fehbvm.com/Article/details/ggwkqxbiy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://read.share.zdbjq.cn/Article/details/gkouhyylj.sHtML

[N07] 两数之和（返回下标）
来源：http://www.m.share.fehbvm.com/Article/details/gupuwaeas.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://www.share.hesvh.cn/Article/details/gxjitwgyh.sHtML


<!-- 参考信息 -->