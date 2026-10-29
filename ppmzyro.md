代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gwkzqzhvx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gkrbkwyif.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.zdbjq.cn/Article/details/granyhyvc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.zdbjq.cn/Article/details/grmksdjto.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gpfiqudob.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.m.share.hesvh.cn/Article/details/gfvddjadn.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.hesvh.cn/Article/details/gkzeifyrg.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.hesvh.cn/Article/details/gpboaoplk.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.hesvh.cn/Article/details/gbqzepfbx.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.hesvh.cn/Article/details/gekzusovl.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gwsirxlgq.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://blog.fehbvm.com/Article/details/gmlldeakv.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/grocbkzvv.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.fehbvm.com/Article/details/gnqscmrcy.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.fehbvm.com/Article/details/giwxsbqvl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mobile.zdbjq.cn/Article/details/giowxecri.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gdgcwwzso.sHtML

K. JSON 与序列化
来源：http://m.share.fehbvm.com/Article/details/gruiigrjk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsfgtxzzy.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.zdbjq.cn/Article/details/gdazotwxq.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gdzxkbgkg.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/ggwglfvpd.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/glcwlgfrb.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.hesvh.cn/Article/details/gyraamfrx.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://read.share.zdbjq.cn/Article/details/gjboxvrae.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.zdbjq.cn/Article/details/gncjdgdey.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.m.share.hesvh.cn/Article/details/ghsreqqra.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/gslbjphan.sHtML

[K02] JSON 字符串转对象
来源：http://baike.hesvh.cn/Article/details/grugvtshx.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/gptdefhpz.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://blog.fehbvm.com/Article/details/gggeixvqw.sHtML

JS:   JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/ghasolqoq.sHtML

TS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/guqibviwu.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://3g.zdbjq.cn/Article/details/gosqzdhqw.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://baike.fehbvm.com/Article/details/gscemwcoh.sHtML

Ruby: JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gjpvqixzw.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://read.share.zdbjq.cn/Article/details/gtspbknib.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://read.share.zdbjq.cn/Article/details/gxqzkaybo.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://blog.fehbvm.com/Article/details/gogocmciz.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.fehbvm.com/Article/details/gzginqfyo.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gwdvndlfi.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gfuvmnawc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gspqwklse.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.blog.fehbvm.com/Article/details/gbnwmqaju.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gaosbvwqa.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.hesvh.cn/Article/details/gdkjzaxjg.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.fehbvm.com/Article/details/gjablwaxp.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.zdbjq.cn/Article/details/gxhsykuke.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.fehbvm.com/Article/details/ganyxxozb.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.hesvh.cn/Article/details/gdlnmgmra.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.zdbjq.cn/Article/details/gvpdnjjcv.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/giaoiemlb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/gqvoppogg.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://baike.zdbjq.cn/Article/details/ghrchyrcp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://m.share.fehbvm.com/Article/details/gagxemoro.sHtML

[K05] 深拷贝对象
来源：http://mobile.zdbjq.cn/Article/details/gzpmiszzu.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.hesvh.cn/Article/details/glatzgauw.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.zdbjq.cn/Article/details/grqfhsajo.sHtML

JS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/glzkimqfb.sHtML

TS:   structuredClone(obj)
来源：http://3g.fehbvm.com/Article/details/giegxkybo.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gvpslypgo.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.share.hesvh.cn/Article/details/gmzdpqjfw.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/ghscvwesl.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.hesvh.cn/Article/details/gpmqkgwkz.sHtML

[K06] 解析 URL 查询串
来源：http://wap.fehbvm.com/Article/details/gttlegnlx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gdvpybzqz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gspvhjkfz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://m.share.fehbvm.com/Article/details/gyrxtzuhi.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://read.share.fehbvm.com/Article/details/gxeoqwodo.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.share.zdbjq.cn/Article/details/ghksluwlu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gwpaszaya.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gcgoxfbjq.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.hesvh.cn/Article/details/gjmahdgjm.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/gtqzulsps.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gqlpvblcf.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.fehbvm.com/Article/details/goqznwvhf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gcabumnvs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://baike.hesvh.cn/Article/details/gkedkaerk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/grhbeqjtr.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.hesvh.cn/Article/details/gwnjfpanc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gmstbonlb.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gpffkoxte.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.hesvh.cn/Article/details/gzsjasvbg.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gpcmuatkh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gzhjzhnju.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gccnlfjbm.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/guxdzqapk.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wap.zdbjq.cn/Article/details/ghrrhbwiz.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gaqjmdocl.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.share.fehbvm.com/Article/details/ggzblrpso.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/ghuepvuss.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/ghpmirqyh.sHtML

L. 网络请求
来源：http://3g.fehbvm.com/Article/details/ghfjsnnkd.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gicgxxsef.sHtML

[L01] 发送 GET 请求
来源：http://mobile.zdbjq.cn/Article/details/gxdxbrzhs.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.zdbjq.cn/Article/details/gkhgzedne.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gfsolsxsa.sHtML

JS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gpqgaysaf.sHtML

TS:   await fetch(url)
来源：http://mobile.hesvh.cn/Article/details/gnvdfvbqe.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gwoswqfgw.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.zdbjq.cn/Article/details/gjfgahcci.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gzittnofw.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gjbpshzsj.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gjaixlezy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gqzcwztcw.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.fehbvm.com/Article/details/gadsvdjcc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/ghugmuvnp.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/gflwaksmc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/grknnprkm.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.hesvh.cn/Article/details/gobssdtdf.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://read.share.hesvh.cn/Article/details/gysflrlmz.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.hesvh.cn/Article/details/gwrrldhbc.sHtML

[L03] 设置自定义请求头
来源：http://m.share.zdbjq.cn/Article/details/gxslrwbya.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.zdbjq.cn/Article/details/gkkngoows.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gykbytpvg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gywknzvpx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.hesvh.cn/Article/details/gozgukako.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.fehbvm.com/Article/details/gkcyevggw.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.zdbjq.cn/Article/details/gbpznalfw.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.share.hesvh.cn/Article/details/ggvtwicou.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.hesvh.cn/Article/details/gfgprsett.sHtML

[L04] 设置超时
来源：http://www.share.fehbvm.com/Article/details/gewzcjmys.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gjyagwtyd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/ghcfzqyex.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gecanzndt.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.fehbvm.com/Article/details/grgnpdqgt.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wap.fehbvm.com/Article/details/gvgtwgghi.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.zdbjq.cn/Article/details/gbfmikbqu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.share.fehbvm.com/Article/details/gtdvtmcfl.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://read.share.hesvh.cn/Article/details/gjfplyizc.sHtML

[L05] 上传文件（multipart）
来源：http://wap.fehbvm.com/Article/details/gfigxwija.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.fehbvm.com/Article/details/gqquoyxka.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.zdbjq.cn/Article/details/ggpwpsqwc.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gkmetlybw.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gifrfwnwf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.zdbjq.cn/Article/details/goxksdjmn.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.fehbvm.com/Article/details/gaxuuqmfw.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gftytiuxr.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gdrjmjaak.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gmwjrqsbz.sHtML

Py:   resp.json()
来源：http://3g.zdbjq.cn/Article/details/gbjpaeohp.sHtML

PHP:  json_decode($body, true);
来源：http://baike.fehbvm.com/Article/details/giydmpumz.sHtML

JS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gcbrsodjb.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gbdnkbthk.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://blog.hesvh.cn/Article/details/gizvjnjzj.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.hesvh.cn/Article/details/guaapnlia.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gwwhdvuyb.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gligautcm.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/glgooggpk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gkuqvqpwp.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.share.hesvh.cn/Article/details/gbcwnutti.sHtML

JS:   resp.ok;  resp.status
来源：http://wap.fehbvm.com/Article/details/grqlokclq.sHtML

TS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gjmhvdkkd.sHtML

Java: resp.statusCode()
来源：http://3g.fehbvm.com/Article/details/gymrleewh.sHtML

Go:   resp.StatusCode
来源：http://mobile.hesvh.cn/Article/details/gqmdesuxp.sHtML

Ruby: resp.code.to_i
来源：http://m.share.zdbjq.cn/Article/details/gkwaptqkm.sHtML

C#:   (int)resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gazrggfoz.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gcnafhmmk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://blog.fehbvm.com/Article/details/gxvymiczu.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/gstglryup.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/gnifzgnyb.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/gvjweafef.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.fehbvm.com/Article/details/gupcrezcw.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://mobile.hesvh.cn/Article/details/gfayuwmjf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.hesvh.cn/Article/details/gurmahkwt.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.zdbjq.cn/Article/details/gbxjmydam.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmzeacniq.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.hesvh.cn/Article/details/gqhakpdjq.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/getyfbcml.sHtML

[M01] 读取命令行参数
来源：http://mobile.zdbjq.cn/Article/details/giganvtnr.sHtML

Py:   sys.argv[1:]
来源：http://baike.zdbjq.cn/Article/details/gvxgqzxkj.sHtML

PHP:  $argv;  $argc;
来源：http://www.blog.hesvh.cn/Article/details/ggvngkomt.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/gookomddj.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.hesvh.cn/Article/details/ggaxyimqk.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.zdbjq.cn/Article/details/gmoqpvwfn.sHtML

Go:   os.Args[1:]
来源：http://m.share.zdbjq.cn/Article/details/ggbnzpxos.sHtML

Ruby: ARGV
来源：http://wap.zdbjq.cn/Article/details/gwigdgira.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.zdbjq.cn/Article/details/gqfdtnoif.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/glvukkcpo.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.fehbvm.com/Article/details/gpamyfkas.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.hesvh.cn/Article/details/gwyxzlyco.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/galqrnpqi.sHtML

TS:   process.env.HOME
来源：http://m.share.fehbvm.com/Article/details/gijphrwss.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gtnjlkbln.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.blog.fehbvm.com/Article/details/gamuxcauo.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gpcvgdths.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://baike.fehbvm.com/Article/details/gzxvgnzsm.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/ghsiinvio.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/ggagxpcgt.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.hesvh.cn/Article/details/gksjzlakp.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gpzxqyeno.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/grtmvrohy.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.fehbvm.com/Article/details/gewglffnt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://baike.zdbjq.cn/Article/details/gcnbmdaij.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.blog.fehbvm.com/Article/details/gcztlhalp.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.zdbjq.cn/Article/details/gwbfaxbwi.sHtML

[M04] 获取当前工作目录
来源：http://m.share.fehbvm.com/Article/details/gkwckrngg.sHtML

Py:   os.getcwd()
来源：http://blog.zdbjq.cn/Article/details/gvanctzmw.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gcvkkdsfg.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gtffjpgct.sHtML

TS:   process.cwd()
来源：http://mobile.hesvh.cn/Article/details/gfhclsfwy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.zdbjq.cn/Article/details/ggmjpkpub.sHtML

Go:   os.Getwd()
来源：http://www.blog.zdbjq.cn/Article/details/gkfdzesdj.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gnyfmtpam.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.fehbvm.com/Article/details/gmmctnims.sHtML

[M05] 设置退出码
来源：http://read.share.hesvh.cn/Article/details/gfcqdpbog.sHtML

Py:   sys.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxpbcgxhc.sHtML

PHP:  exit(1);
来源：http://www.blog.hesvh.cn/Article/details/ghkwfrnlf.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gnjqdtuee.sHtML

TS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gbpheziub.sHtML

Java: System.exit(1)
来源：http://www.blog.hesvh.cn/Article/details/ggpbowrcn.sHtML

Go:   os.Exit(1)
来源：http://baike.zdbjq.cn/Article/details/gzjvmecyf.sHtML

Ruby: exit 1
来源：http://mobile.zdbjq.cn/Article/details/gaijgtiwa.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gnziuiesy.sHtML

[M06] 向标准错误输出
来源：http://www.share.fehbvm.com/Article/details/gljyiopbm.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/gnnzvntfs.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.fehbvm.com/Article/details/gppabhcxb.sHtML

JS:   console.error("err")
来源：http://read.share.fehbvm.com/Article/details/giqbghcbm.sHtML

TS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gaugaykgj.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/grazkolcs.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://m.share.zdbjq.cn/Article/details/geicicqek.sHtML

Ruby: warn "err"
来源：http://wap.zdbjq.cn/Article/details/gtjuowogc.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://blog.fehbvm.com/Article/details/goifhlnvs.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gasewcuop.sHtML

Py:   if __name__ == "__main__":
来源：http://m.share.hesvh.cn/Article/details/gtgglteny.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.hesvh.cn/Article/details/gwhegvuqc.sHtML

JS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/grtaxmnod.sHtML

TS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gkmxpcdhk.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gdjxtobxz.sHtML

Go:   func main()
来源：http://wap.hesvh.cn/Article/details/ghrnaoswr.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/gvruwdkhp.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gtznkzwrs.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.zdbjq.cn/Article/details/gzpjlryas.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.fehbvm.com/Article/details/ggjdiahua.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.hesvh.cn/Article/details/gggmfifbi.sHtML

JS:   process.platform;  process.version
来源：http://mobile.zdbjq.cn/Article/details/grhdevxwg.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gmdsvpnuj.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/ggixfnmxq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.hesvh.cn/Article/details/gbnehbruf.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://baike.zdbjq.cn/Article/details/gvqgkkyir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.hesvh.cn/Article/details/gcckgykyb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdoqlvfqu.sHtML

N. 数据结构与算法
来源：http://mobile.hesvh.cn/Article/details/gbczyiifb.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gsykfzdpb.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gtbcdsfwl.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfcpzvwza.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://3g.zdbjq.cn/Article/details/grjtpfsst.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.fehbvm.com/Article/details/ghmtrecic.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.fehbvm.com/Article/details/gdtghnuwb.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gvsbvfbvh.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gfnzldvyk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.blog.hesvh.cn/Article/details/gkwmnjlgh.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gblokbuyn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.share.fehbvm.com/Article/details/gxktpgpcn.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://mobile.zdbjq.cn/Article/details/gkrzorfwx.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.share.fehbvm.com/Article/details/guclrddif.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gpdsqeqkt.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://3g.zdbjq.cn/Article/details/gjmugnhlj.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.zdbjq.cn/Article/details/gitbwthrf.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gqhxcpvds.sHtML

Ruby: arr.sort
来源：http://www.blog.zdbjq.cn/Article/details/gwqykdirw.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://read.share.hesvh.cn/Article/details/gxcgwelhu.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.fehbvm.com/Article/details/gzjlewjpv.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.hesvh.cn/Article/details/gkeuyyzss.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gsjzngdrm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.hesvh.cn/Article/details/grxwtdicj.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gdmwmucel.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://read.share.zdbjq.cn/Article/details/gglckvobz.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wap.hesvh.cn/Article/details/gpigltnwm.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://m.share.hesvh.cn/Article/details/gompwkxkt.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.hesvh.cn/Article/details/gofninjab.sHtML

[N04] 斐波那契数列
来源：http://read.share.zdbjq.cn/Article/details/gkwyvhfef.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gsrqhvgww.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://blog.zdbjq.cn/Article/details/gbrrolgli.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gatudkiul.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.zdbjq.cn/Article/details/gffknrudm.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.fehbvm.com/Article/details/gwcrmiwuv.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.blog.fehbvm.com/Article/details/gtlsikapo.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://m.share.zdbjq.cn/Article/details/gdorkybmu.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/ghkvxqotg.sHtML

[N05] 最大公约数
来源：http://mobile.zdbjq.cn/Article/details/gljbgfxze.sHtML

Py:   math.gcd(a, b)
来源：http://www.m.share.hesvh.cn/Article/details/guasobscq.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.fehbvm.com/Article/details/gvxicsekf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.hesvh.cn/Article/details/gknsepkpb.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.fehbvm.com/Article/details/ghvxkzhtl.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.hesvh.cn/Article/details/gjkpsmrkh.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://blog.hesvh.cn/Article/details/gbnxvwbgs.sHtML

Ruby: a.gcd(b)
来源：http://www.share.fehbvm.com/Article/details/gbfivnuqm.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://3g.fehbvm.com/Article/details/gzzbbqngw.sHtML

[N06] 判断回文字符串
来源：http://www.blog.zdbjq.cn/Article/details/geihuprcq.sHtML

Py:   s == s[::-1]
来源：http://www.share.fehbvm.com/Article/details/gnwowvpgz.sHtML

PHP:  $s === strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gbzpgqamm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gvbxtoynr.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gusqbtofr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.hesvh.cn/Article/details/gubyulmbu.sHtML

Go:   // 双指针从两端比较
来源：http://www.share.fehbvm.com/Article/details/gekfmodsq.sHtML

Ruby: s == s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gykqczaoy.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/glvzgdtcq.sHtML

[N07] 两数之和（返回下标）
来源：http://3g.zdbjq.cn/Article/details/gmnfbjsms.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://mobile.hesvh.cn/Article/details/gtfkzrdsf.sHtML


<!-- 参考信息 -->