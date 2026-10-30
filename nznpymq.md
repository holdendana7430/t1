代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/gacvlooej.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mobile.zdbjq.cn/Article/details/gcrentmig.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gumjqcfqw.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://read.share.zdbjq.cn/Article/details/gspcikcan.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://3g.fehbvm.com/Article/details/gklhyxqaz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.fehbvm.com/Article/details/gboogoprw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://baike.zdbjq.cn/Article/details/girqezakv.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.blog.zdbjq.cn/Article/details/gdehvqwqu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://m.share.fehbvm.com/Article/details/gkeapwgkk.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.zdbjq.cn/Article/details/gbzsbqgch.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.hesvh.cn/Article/details/gnwmabttw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.zdbjq.cn/Article/details/geufheeda.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gvfcxwbqx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/ggnvtpncq.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gkcwaocjz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://read.share.hesvh.cn/Article/details/goegfmfxc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gestpoisl.sHtML

K. JSON 与序列化
来源：http://www.m.share.fehbvm.com/Article/details/gcjubjmkw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtfgzncpa.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gdtaueozz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.zdbjq.cn/Article/details/gidwyvzya.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.fehbvm.com/Article/details/gylldvakf.sHtML

JS:   JSON.stringify(obj)
来源：http://read.share.hesvh.cn/Article/details/gjhuaqcdd.sHtML

TS:   JSON.stringify(obj)
来源：http://baike.zdbjq.cn/Article/details/gmmktptyj.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://m.share.zdbjq.cn/Article/details/gxitljzoc.sHtML

Go:   json.Marshal(obj)
来源：http://mobile.hesvh.cn/Article/details/gikzdoziq.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gstkunybo.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://read.share.hesvh.cn/Article/details/gesirhgwr.sHtML

[K02] JSON 字符串转对象
来源：http://blog.zdbjq.cn/Article/details/gmkaototo.sHtML

Py:   json.loads(s)
来源：http://baike.fehbvm.com/Article/details/gybmssqeh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.hesvh.cn/Article/details/gnqiawtim.sHtML

JS:   JSON.parse(s)
来源：http://www.m.share.hesvh.cn/Article/details/gasxizlrj.sHtML

TS:   JSON.parse(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gxwzgtvob.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.hesvh.cn/Article/details/gsexhbnss.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.fehbvm.com/Article/details/gzokszhfs.sHtML

Ruby: JSON.parse(s)
来源：http://3g.fehbvm.com/Article/details/gjpjvibso.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gqhnlfpgi.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.hesvh.cn/Article/details/gwkgbkbgk.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gxaolxqpb.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.fehbvm.com/Article/details/gjcwzrjtw.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/gefplmpgu.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcnjiabx.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gtqdhfnyx.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.zdbjq.cn/Article/details/gyvngsegf.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.fehbvm.com/Article/details/gxaklhlzc.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gcmnvjkob.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gwvssxsys.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.hesvh.cn/Article/details/gnbnyqzsl.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.zdbjq.cn/Article/details/gvpqelvgq.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.zdbjq.cn/Article/details/gnvcmtrvu.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.fehbvm.com/Article/details/gsdgzxwix.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gflabpdjz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.fehbvm.com/Article/details/gzlywpcez.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://mobile.fehbvm.com/Article/details/gussghomc.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gjqpamwmd.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gblihxbya.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.zdbjq.cn/Article/details/gxizmvxne.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gfsuoufuu.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/ggocnwidu.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gptqemiwa.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://3g.fehbvm.com/Article/details/gjdiibhpk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.hesvh.cn/Article/details/gxqmuokvj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://baike.hesvh.cn/Article/details/glbryrxaf.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://m.share.hesvh.cn/Article/details/ghpzgdcuw.sHtML

[K06] 解析 URL 查询串
来源：http://m.share.hesvh.cn/Article/details/gxraopais.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gjlepxfaa.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gckebtsfz.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gbkttwrqr.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gabqlpruq.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://blog.fehbvm.com/Article/details/gosuldexu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gpyxozwzt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.fehbvm.com/Article/details/gfzquagcd.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ghfpjyevs.sHtML

[K07] 进制转换
来源：http://3g.zdbjq.cn/Article/details/gacnaiskx.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gssassmyd.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.hesvh.cn/Article/details/gmlhpufam.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/giglxmjqu.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/glallqfve.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gacutjiwm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/ghssrcifn.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://baike.zdbjq.cn/Article/details/gbcnlepon.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gugvqohji.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gptowqegu.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.fehbvm.com/Article/details/gxdbleldj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/ggizqmhty.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://blog.zdbjq.cn/Article/details/grydzaeex.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gexiqfjwh.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.zdbjq.cn/Article/details/gczgsouse.sHtML

Go:   encoding/gob
来源：http://blog.zdbjq.cn/Article/details/gjvdnelnh.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.fehbvm.com/Article/details/gghpjdtnd.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gvrwppvsu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfyrbklqu.sHtML

L. 网络请求
来源：http://www.share.fehbvm.com/Article/details/gpuddkfzj.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gktflvelc.sHtML

[L01] 发送 GET 请求
来源：http://3g.fehbvm.com/Article/details/gjrlwqmcm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://blog.zdbjq.cn/Article/details/grumoedbs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.fehbvm.com/Article/details/glocagtqt.sHtML

JS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/gthohtxkw.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/gjafhwysi.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.zdbjq.cn/Article/details/gtrngbnhr.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gsprjhwbm.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://3g.zdbjq.cn/Article/details/gzzlocjxp.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.fehbvm.com/Article/details/ginmecfbx.sHtML

[L02] 发送 POST JSON
来源：http://wap.hesvh.cn/Article/details/gogblxmve.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://baike.hesvh.cn/Article/details/gfydaridn.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.fehbvm.com/Article/details/gzojvcdrz.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.fehbvm.com/Article/details/gwelpqqld.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.fehbvm.com/Article/details/gzpgzuwmo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gptlaqxqh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.zdbjq.cn/Article/details/gvsdoemfn.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://3g.fehbvm.com/Article/details/gjuknbbze.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.zdbjq.cn/Article/details/gfbrtpdqo.sHtML

[L03] 设置自定义请求头
来源：http://read.share.zdbjq.cn/Article/details/gcpepaivh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://3g.hesvh.cn/Article/details/gutgipufv.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://blog.zdbjq.cn/Article/details/guppzdvwg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gywzaszbx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gtowtevyg.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.hesvh.cn/Article/details/glextoeme.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://read.share.fehbvm.com/Article/details/gmpsqrbpx.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/goriwxstb.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gsurjewjh.sHtML

[L04] 设置超时
来源：http://baike.hesvh.cn/Article/details/gnucpldmn.sHtML

Py:   requests.get(url, timeout=5)
来源：http://read.share.hesvh.cn/Article/details/gbhthgrjx.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.zdbjq.cn/Article/details/gjfptjsrp.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gquwtuhlf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.zdbjq.cn/Article/details/gslwuwnng.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://read.share.zdbjq.cn/Article/details/gmyjmukvm.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gooftagyd.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mobile.zdbjq.cn/Article/details/gfjssgmfs.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/grbuizzdq.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.hesvh.cn/Article/details/gguioukjd.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.fehbvm.com/Article/details/gmsjbacqp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gmeavihvj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gtzdkcvsh.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gxmfwfsoh.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://baike.zdbjq.cn/Article/details/gpndmoeod.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.hesvh.cn/Article/details/gyxhblwxh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.blog.hesvh.cn/Article/details/gjazmpfnd.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghjprvhgx.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.zdbjq.cn/Article/details/gegninhln.sHtML

Py:   resp.json()
来源：http://3g.hesvh.cn/Article/details/goolzmaxt.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/ghjemdvsb.sHtML

JS:   await resp.json()
来源：http://baike.fehbvm.com/Article/details/gsuzlfxqf.sHtML

TS:   await resp.json()
来源：http://read.share.fehbvm.com/Article/details/gdpqgjevp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gfopwcnbl.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://m.share.fehbvm.com/Article/details/gkmlrvgxp.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/guudhndyt.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gyaljxaxh.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gminyahdn.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.blog.fehbvm.com/Article/details/gchuxwekh.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.zdbjq.cn/Article/details/ggqbmqiib.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/glaaovkcl.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gffzksepl.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gkxxjujxk.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gpjblvixe.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gtwhqtsbc.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gpopjiprb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.fehbvm.com/Article/details/gdnqspglc.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gjperirkg.sHtML

PHP:  curl_multi_init() 系列
来源：http://read.share.fehbvm.com/Article/details/gjvymvquw.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.hesvh.cn/Article/details/gasnmknmz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.zdbjq.cn/Article/details/gjjtkwfay.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://m.share.zdbjq.cn/Article/details/gyubaojku.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://m.share.zdbjq.cn/Article/details/gxrpklmtt.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.fehbvm.com/Article/details/gwzysgidj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.hesvh.cn/Article/details/gzpsfhnfh.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwuneosqu.sHtML

M. 命令行 / 进程 / 环境
来源：http://wap.hesvh.cn/Article/details/gmctnkwwc.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcenvgody.sHtML

[M01] 读取命令行参数
来源：http://read.share.fehbvm.com/Article/details/gdezgrmpy.sHtML

Py:   sys.argv[1:]
来源：http://m.share.zdbjq.cn/Article/details/gqeqvqlxe.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.hesvh.cn/Article/details/gewnerfwc.sHtML

JS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gvifyikdc.sHtML

TS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gvzdbshjh.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/gryrmxwyg.sHtML

Go:   os.Args[1:]
来源：http://m.share.fehbvm.com/Article/details/gjffvuxva.sHtML

Ruby: ARGV
来源：http://read.share.hesvh.cn/Article/details/glzzfwgmr.sHtML

C#:   args 数组（Main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gatymkcda.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gruliqmyu.sHtML

Py:   os.environ.get("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gbcsvumyy.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gajrzcdjy.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/godmeucup.sHtML

TS:   process.env.HOME
来源：http://www.share.fehbvm.com/Article/details/gznxneifh.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gstupbydz.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gulgshirs.sHtML

Ruby: ENV["HOME"]
来源：http://read.share.hesvh.cn/Article/details/gakpmrxsy.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gvxwtpxsq.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gzqdqdklc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://read.share.hesvh.cn/Article/details/gumtuthit.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.hesvh.cn/Article/details/gsqcqzfpo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.fehbvm.com/Article/details/gajbwdiuu.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gdvadgaee.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.blog.zdbjq.cn/Article/details/gjaqwngxt.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://wap.fehbvm.com/Article/details/gqnoyheug.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://baike.hesvh.cn/Article/details/gfnbwnngu.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/gzxgszlys.sHtML

[M04] 获取当前工作目录
来源：http://blog.fehbvm.com/Article/details/gktdzrmgx.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/grtjyhiif.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gnxtxnhxg.sHtML

JS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gpqbdeseb.sHtML

TS:   process.cwd()
来源：http://baike.hesvh.cn/Article/details/godmfqvdd.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.zdbjq.cn/Article/details/gklvagdvo.sHtML

Go:   os.Getwd()
来源：http://mobile.zdbjq.cn/Article/details/gpoeozrzk.sHtML

Ruby: Dir.pwd
来源：http://www.share.fehbvm.com/Article/details/gviocexur.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gnpotbwjb.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gocthjrng.sHtML

Py:   sys.exit(1)
来源：http://3g.fehbvm.com/Article/details/gmienyprc.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/gtojpehjm.sHtML

JS:   process.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gqsizvyff.sHtML

TS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gayoeurxz.sHtML

Java: System.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmvgemzla.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/goekvzzmo.sHtML

Ruby: exit 1
来源：http://www.blog.hesvh.cn/Article/details/gqgdmwlou.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.zdbjq.cn/Article/details/gfkzjfial.sHtML

[M06] 向标准错误输出
来源：http://wap.fehbvm.com/Article/details/gorfblysj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/goqmpdiww.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.fehbvm.com/Article/details/ghwlanjvm.sHtML

JS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/giojdopcc.sHtML

TS:   console.error("err")
来源：http://www.blog.fehbvm.com/Article/details/gvairxliv.sHtML

Java: System.err.println("err")
来源：http://baike.fehbvm.com/Article/details/ggvrxqgmt.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.hesvh.cn/Article/details/gmzheilaq.sHtML

Ruby: warn "err"
来源：http://baike.zdbjq.cn/Article/details/gexabltnj.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.zdbjq.cn/Article/details/ggglkhkdc.sHtML

[M07] 判断是否为主入口
来源：http://www.share.zdbjq.cn/Article/details/gfrmkrcby.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.fehbvm.com/Article/details/gjmulllbf.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.zdbjq.cn/Article/details/gtbkxergj.sHtML

JS:   require.main === module
来源：http://blog.hesvh.cn/Article/details/gdpsujzct.sHtML

TS:   require.main === module
来源：http://3g.fehbvm.com/Article/details/gtexlbguk.sHtML

Java: public static void main(String[] args)
来源：http://m.share.zdbjq.cn/Article/details/gqfqehzrc.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gkujfxxpg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gdytayoas.sHtML

C#:   static void Main(string[] args)
来源：http://3g.zdbjq.cn/Article/details/guuskgptv.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gvpztvopb.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gcmvkmmtu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://wap.fehbvm.com/Article/details/glrvkstti.sHtML

JS:   process.platform;  process.version
来源：http://www.share.hesvh.cn/Article/details/gilsnzbxl.sHtML

TS:   process.platform;  process.version
来源：http://mobile.hesvh.cn/Article/details/gkvrcaucn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/gvhjvupod.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.hesvh.cn/Article/details/gevgpgxta.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mobile.fehbvm.com/Article/details/ggxleffns.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.fehbvm.com/Article/details/gjddfycep.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gtvziwwxc.sHtML

N. 数据结构与算法
来源：http://baike.fehbvm.com/Article/details/gxfssbexa.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gpxkpmcji.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.zdbjq.cn/Article/details/gimfpwypb.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.hesvh.cn/Article/details/guzrcqnub.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.fehbvm.com/Article/details/gzwymzeka.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.hesvh.cn/Article/details/guwcazdol.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/ghzujcoan.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gpbhdxpmk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwqjgygme.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gndqycxkk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://baike.fehbvm.com/Article/details/gyocjxnhk.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://www.m.share.fehbvm.com/Article/details/gukxjiagw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://read.share.zdbjq.cn/Article/details/ghqfwejxa.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://baike.zdbjq.cn/Article/details/gtugowbnd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.fehbvm.com/Article/details/gwyqinjxb.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gefevxivq.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://3g.zdbjq.cn/Article/details/gwmhxoazt.sHtML

Go:   slices.Sort(arr)
来源：http://blog.zdbjq.cn/Article/details/gqzrtbizm.sHtML

Ruby: arr.sort
来源：http://blog.zdbjq.cn/Article/details/gzhcsmnxv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.share.hesvh.cn/Article/details/gvuxazrve.sHtML

[N03] 快速排序（分治示例）
来源：http://mobile.hesvh.cn/Article/details/guqrkcgcb.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://read.share.zdbjq.cn/Article/details/gpfcdkrtw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.blog.fehbvm.com/Article/details/gheyrxqwm.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.share.fehbvm.com/Article/details/gtyswbzar.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.fehbvm.com/Article/details/gtwrezuze.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.fehbvm.com/Article/details/gotpncqzv.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://www.share.hesvh.cn/Article/details/gkvbwmmip.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://www.m.share.zdbjq.cn/Article/details/gtibcfmfd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.zdbjq.cn/Article/details/gflojhuxe.sHtML

[N04] 斐波那契数列
来源：http://wap.zdbjq.cn/Article/details/gfsmkpvqz.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.m.share.fehbvm.com/Article/details/gnxedyvyq.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fehbvm.com/Article/details/gybbhblht.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wap.hesvh.cn/Article/details/gmkmurbsx.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.fehbvm.com/Article/details/gpdhcnqji.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mobile.zdbjq.cn/Article/details/gbxykdqph.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/glmmgwwfc.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.zdbjq.cn/Article/details/ghfxnizbf.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://m.share.fehbvm.com/Article/details/gfaovzmrq.sHtML

[N05] 最大公约数
来源：http://www.blog.hesvh.cn/Article/details/gyitsmedq.sHtML

Py:   math.gcd(a, b)
来源：http://read.share.fehbvm.com/Article/details/guzscehmk.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://read.share.fehbvm.com/Article/details/gcistuyfr.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baike.hesvh.cn/Article/details/gjhzovsrq.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://3g.hesvh.cn/Article/details/gkqqnsoss.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://m.share.hesvh.cn/Article/details/gzddkmdhc.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://www.blog.zdbjq.cn/Article/details/gdxkpggvx.sHtML

Ruby: a.gcd(b)
来源：http://www.blog.hesvh.cn/Article/details/gllfiklxr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://baike.hesvh.cn/Article/details/gjyosyhhz.sHtML

[N06] 判断回文字符串
来源：http://www.m.share.fehbvm.com/Article/details/gkodmbxwq.sHtML

Py:   s == s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gtvtyxipb.sHtML

PHP:  $s === strrev($s);
来源：http://www.share.fehbvm.com/Article/details/gqkmzisrm.sHtML

JS:   s === [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gelghrbry.sHtML

TS:   s === [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gifihwydx.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://baike.fehbvm.com/Article/details/gcelikecq.sHtML

Go:   // 双指针从两端比较
来源：http://www.m.share.zdbjq.cn/Article/details/gukymbpjz.sHtML

Ruby: s == s.reverse
来源：http://wap.zdbjq.cn/Article/details/goxxfywvs.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://www.m.share.fehbvm.com/Article/details/gvivzxkdn.sHtML

[N07] 两数之和（返回下标）
来源：http://m.share.hesvh.cn/Article/details/gdxlqshfq.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://blog.zdbjq.cn/Article/details/gcrwwhstb.sHtML


<!-- 参考信息 -->