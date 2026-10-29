代发 wailian999

[J07] 比较两个日期
来源：http://www.m.share.fehbvm.com/Article/details/gzrmacvqi.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gptzxojzg.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.zdbjq.cn/Article/details/gixfvfbsr.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://baike.hesvh.cn/Article/details/ggbcmvahv.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/gsqdlszcd.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://m.share.hesvh.cn/Article/details/gcsmxmifv.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gtpmnqidj.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.zdbjq.cn/Article/details/gnhftmxnl.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.zdbjq.cn/Article/details/gobtwvvrr.sHtML

[J08] 提取年月日与星期
来源：http://blog.zdbjq.cn/Article/details/ghtjcrkan.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gbrgjsovt.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.blog.hesvh.cn/Article/details/gscvwnjro.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.blog.zdbjq.cn/Article/details/gyffuceln.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/ggjzqqpbj.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.blog.hesvh.cn/Article/details/gtpbufehh.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gflsrudfn.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.zdbjq.cn/Article/details/gqeswgoue.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.fehbvm.com/Article/details/goryvfyai.sHtML

[J09] 时区处理
来源：http://wap.fehbvm.com/Article/details/graxsbdhx.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gvuzqxumd.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://blog.fehbvm.com/Article/details/gwkwgzpbe.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.hesvh.cn/Article/details/gaazjtwpv.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/glhwwkdwh.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.fehbvm.com/Article/details/gxwhpjkls.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://baike.zdbjq.cn/Article/details/gwirzxijg.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gkngiayll.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.blog.hesvh.cn/Article/details/gbygjpkaw.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gcgidxcdr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://3g.zdbjq.cn/Article/details/gsxykmkzn.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gdjyehnvv.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.zdbjq.cn/Article/details/ghenjskcd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://read.share.fehbvm.com/Article/details/gwivvkgxe.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/glcavrqcb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.zdbjq.cn/Article/details/gkmtlmjhl.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.blog.zdbjq.cn/Article/details/grqvgjzuy.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gdctjafnx.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gtfkrgtuj.sHtML

K. JSON 与序列化
来源：http://wap.fehbvm.com/Article/details/gyvhvtceh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gotzqvsvu.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.zdbjq.cn/Article/details/gpwazuwwz.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://baike.hesvh.cn/Article/details/gemsiupux.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.fehbvm.com/Article/details/gygcbdaaw.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.hesvh.cn/Article/details/gakhnqnzl.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gkwuzotma.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.fehbvm.com/Article/details/guktfstvb.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.hesvh.cn/Article/details/gqrdkqhkm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://mobile.fehbvm.com/Article/details/guctitokk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.hesvh.cn/Article/details/grzpbiihx.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gahihxsnl.sHtML

Py:   json.loads(s)
来源：http://3g.hesvh.cn/Article/details/geyhsahns.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://read.share.hesvh.cn/Article/details/gokdiaayy.sHtML

JS:   JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gyfiebtyc.sHtML

TS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/gtrpsxmcc.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.fehbvm.com/Article/details/gqclabshl.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gdgiybgqu.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gdpfobhyk.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.fehbvm.com/Article/details/gdgqqhzhs.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.fehbvm.com/Article/details/grzaddppa.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gmemqkflt.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gvzbsbvvc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.hesvh.cn/Article/details/ggxeokpjl.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://read.share.hesvh.cn/Article/details/gwowlhilz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mobile.zdbjq.cn/Article/details/grteztnxp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.fehbvm.com/Article/details/growjnsry.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.zdbjq.cn/Article/details/goxkwotgv.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.share.fehbvm.com/Article/details/ggjlxqhci.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gletkwibt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://baike.zdbjq.cn/Article/details/gzlixnofb.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://baike.zdbjq.cn/Article/details/gidicbiea.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gzhbtqkgj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gdqqmuabp.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.hesvh.cn/Article/details/gktfipihy.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gcjbzqhbq.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.blog.fehbvm.com/Article/details/gnkknmmjm.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mobile.hesvh.cn/Article/details/gpkwdwyrc.sHtML

[K05] 深拷贝对象
来源：http://blog.fehbvm.com/Article/details/gzzuygmkr.sHtML

Py:   copy.deepcopy(obj)
来源：http://m.share.zdbjq.cn/Article/details/gtwztoafc.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gtmhpucdn.sHtML

JS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gkldhbjge.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gekdnkyxx.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.zdbjq.cn/Article/details/gommqnswa.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mobile.fehbvm.com/Article/details/glcfxvswk.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gqkyfcxem.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gpulorxer.sHtML

[K06] 解析 URL 查询串
来源：http://www.share.fehbvm.com/Article/details/gppfbodgt.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gtxbiffyl.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wap.zdbjq.cn/Article/details/gdwcxuoaf.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gobjxaact.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gfossbvgh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gdqmabdfx.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/gpkrbqfit.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://baike.zdbjq.cn/Article/details/ggkwwejjn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.blog.fehbvm.com/Article/details/gokvhfqmp.sHtML

[K07] 进制转换
来源：http://www.blog.hesvh.cn/Article/details/gwunolayt.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gxijglajh.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/gcxdazeex.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.fehbvm.com/Article/details/gjfmeojat.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gagdgbecg.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gtdloqpco.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.zdbjq.cn/Article/details/gavnfgvzf.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.zdbjq.cn/Article/details/gdlurgqoc.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gbaahtfkk.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.m.share.zdbjq.cn/Article/details/gfdoqrhwr.sHtML

Py:   pickle.dumps(obj)
来源：http://baike.hesvh.cn/Article/details/gnbjmoomu.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.m.share.hesvh.cn/Article/details/gxjjlawvl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.fehbvm.com/Article/details/gbvpfwndo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.blog.zdbjq.cn/Article/details/gtnrapkmq.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.hesvh.cn/Article/details/gstjnlewz.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gwvwdlemp.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmzhjcsdz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.m.share.zdbjq.cn/Article/details/gwyolvfcn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghqtipnft.sHtML

L. 网络请求
来源：http://www.share.zdbjq.cn/Article/details/gojsbjgls.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gkqsaiopg.sHtML

[L01] 发送 GET 请求
来源：http://baike.zdbjq.cn/Article/details/gkwwswgva.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wap.zdbjq.cn/Article/details/gegygblge.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.fehbvm.com/Article/details/grumzxmte.sHtML

JS:   await fetch(url)
来源：http://read.share.fehbvm.com/Article/details/gypepdvip.sHtML

TS:   await fetch(url)
来源：http://baike.fehbvm.com/Article/details/ggpikumqn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.hesvh.cn/Article/details/gybhugqkv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/ghmhjnwov.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gflwnpjbq.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwdmcirq.sHtML

[L02] 发送 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gozasspiw.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.zdbjq.cn/Article/details/gowwvjsfx.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.fehbvm.com/Article/details/gerxurloq.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gjnnpeajr.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/gbvvdbcgt.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.share.fehbvm.com/Article/details/gammvannn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.fehbvm.com/Article/details/geretaprp.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.hesvh.cn/Article/details/ggbgswvqt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/gaegnwzft.sHtML

[L03] 设置自定义请求头
来源：http://read.share.hesvh.cn/Article/details/gkkxqyyam.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.zdbjq.cn/Article/details/gbevsikwe.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://m.share.fehbvm.com/Article/details/ggszttqxg.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.zdbjq.cn/Article/details/ggkdsdtzj.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gkezykaey.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.hesvh.cn/Article/details/guzmtvwcz.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.hesvh.cn/Article/details/gpvsjyjfc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.hesvh.cn/Article/details/gtnkymnyw.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://baike.hesvh.cn/Article/details/gukjgylti.sHtML

[L04] 设置超时
来源：http://www.share.zdbjq.cn/Article/details/gkrziacqx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/gkwdcfhvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.zdbjq.cn/Article/details/gdjgcshfi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/gnrjcxhqw.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.hesvh.cn/Article/details/gkwveivcu.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/gdgekttyt.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://3g.zdbjq.cn/Article/details/gnwesgbaj.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.m.share.fehbvm.com/Article/details/gqmdnzyvg.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://m.share.fehbvm.com/Article/details/gwidvnbtm.sHtML

[L05] 上传文件（multipart）
来源：http://www.share.hesvh.cn/Article/details/gomhqfkqa.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.zdbjq.cn/Article/details/gioarqlvb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://m.share.zdbjq.cn/Article/details/gmuqlkuhs.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.fehbvm.com/Article/details/glholwnlx.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://m.share.zdbjq.cn/Article/details/gqrnkwljt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://3g.fehbvm.com/Article/details/gcxnjsatt.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wap.fehbvm.com/Article/details/geosfjpil.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gcqcskqmw.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.fehbvm.com/Article/details/gwtyltstc.sHtML

[L06] 解析响应为 JSON
来源：http://www.blog.zdbjq.cn/Article/details/gxnhlkybf.sHtML

Py:   resp.json()
来源：http://blog.zdbjq.cn/Article/details/gbkzkwigt.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gybiyxqwd.sHtML

JS:   await resp.json()
来源：http://www.blog.zdbjq.cn/Article/details/gjtcitfbu.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/gxabttjca.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.share.fehbvm.com/Article/details/gljaomuzg.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://read.share.hesvh.cn/Article/details/gbexsqtkg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.hesvh.cn/Article/details/gwjnhzsoe.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://3g.hesvh.cn/Article/details/gdeqklrno.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gnjleetkk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wap.fehbvm.com/Article/details/gxdwplxzw.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gxtwhzaud.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/gmfldxfns.sHtML

TS:   resp.ok;  resp.status
来源：http://3g.fehbvm.com/Article/details/gtnlitnxt.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gckhttkce.sHtML

Go:   resp.StatusCode
来源：http://wap.hesvh.cn/Article/details/gjtigzymd.sHtML

Ruby: resp.code.to_i
来源：http://www.share.hesvh.cn/Article/details/gkenyijsx.sHtML

C#:   (int)resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gcicukbme.sHtML

[L08] 并发请求多个地址
来源：http://3g.fehbvm.com/Article/details/ghfvanckk.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/gzqjwrimm.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.hesvh.cn/Article/details/ggzcstpbm.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.hesvh.cn/Article/details/gwasspjcd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gmvacokcu.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.hesvh.cn/Article/details/gxzqianxa.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.zdbjq.cn/Article/details/gjktmsqam.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.fehbvm.com/Article/details/grftyxdwh.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.hesvh.cn/Article/details/gokkgjjgf.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gsditedvh.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.hesvh.cn/Article/details/gatjsedil.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/ghduwdfcv.sHtML

[M01] 读取命令行参数
来源：http://wap.zdbjq.cn/Article/details/ggdczrgnr.sHtML

Py:   sys.argv[1:]
来源：http://baike.hesvh.cn/Article/details/glhnzelzl.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gehxiaoqe.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.zdbjq.cn/Article/details/gextrhkxa.sHtML

TS:   process.argv.slice(2)
来源：http://wap.fehbvm.com/Article/details/gnpuxuuwv.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.fehbvm.com/Article/details/gfperjikl.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.hesvh.cn/Article/details/gwpkydjfo.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/ggscvtrju.sHtML

C#:   args 数组（Main 方法参数）
来源：http://3g.zdbjq.cn/Article/details/guvikpbnu.sHtML

[M02] 读取环境变量
来源：http://3g.hesvh.cn/Article/details/gwafxueyr.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.fehbvm.com/Article/details/gfwcgdpbx.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://read.share.zdbjq.cn/Article/details/gdvpmhums.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gnjqpzihn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gvnzumaap.sHtML

Java: System.getenv("HOME")
来源：http://read.share.hesvh.cn/Article/details/gugcvypvi.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.zdbjq.cn/Article/details/gdojclvgu.sHtML

Ruby: ENV["HOME"]
来源：http://www.blog.fehbvm.com/Article/details/gaqfyzoin.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gejcxvyow.sHtML

[M03] 执行外部命令
来源：http://3g.hesvh.cn/Article/details/gbxtxvxeo.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.zdbjq.cn/Article/details/gbopcazzw.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://read.share.fehbvm.com/Article/details/gcsejpxpr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gyysigmps.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.zdbjq.cn/Article/details/gbraaikwh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gvxgmgncs.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.zdbjq.cn/Article/details/gfnprlugm.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gnbufzmwb.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gklympbkk.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gwezsgczh.sHtML

Py:   os.getcwd()
来源：http://baike.zdbjq.cn/Article/details/guwqeyzjd.sHtML

PHP:  getcwd();
来源：http://mobile.fehbvm.com/Article/details/gtfsxtwur.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/ghshxxnmv.sHtML

TS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gpytywtej.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.m.share.zdbjq.cn/Article/details/gfxbzmmbr.sHtML

Go:   os.Getwd()
来源：http://read.share.zdbjq.cn/Article/details/gdnkwogtw.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gxszxvkbf.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.hesvh.cn/Article/details/gjhqwmett.sHtML

[M05] 设置退出码
来源：http://wap.hesvh.cn/Article/details/geecwknnp.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gwqgifmxt.sHtML

PHP:  exit(1);
来源：http://read.share.zdbjq.cn/Article/details/goehpvwfk.sHtML

JS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gjuonblcd.sHtML

TS:   process.exit(1)
来源：http://wap.hesvh.cn/Article/details/guqndssod.sHtML

Java: System.exit(1)
来源：http://blog.zdbjq.cn/Article/details/gsbxxlbgp.sHtML

Go:   os.Exit(1)
来源：http://mobile.hesvh.cn/Article/details/gjyzdqtcd.sHtML

Ruby: exit 1
来源：http://www.m.share.hesvh.cn/Article/details/gsccomxcz.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://read.share.hesvh.cn/Article/details/gkavwecry.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gwenxakqt.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwkidqqv.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://blog.zdbjq.cn/Article/details/gkldunvdx.sHtML

JS:   console.error("err")
来源：http://m.share.hesvh.cn/Article/details/gnrhbflpn.sHtML

TS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/gxbxbhwhw.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gipejwacn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://blog.hesvh.cn/Article/details/grmlflngs.sHtML

Ruby: warn "err"
来源：http://www.m.share.zdbjq.cn/Article/details/gjsmjvfki.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gzqinsftj.sHtML

[M07] 判断是否为主入口
来源：http://wap.hesvh.cn/Article/details/gedfvdaeq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gbunfavmt.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gotxhfwyj.sHtML

JS:   require.main === module
来源：http://blog.fehbvm.com/Article/details/gvnvrwfxb.sHtML

TS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gnguanrrn.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gnlqcxkju.sHtML

Go:   func main()
来源：http://baike.zdbjq.cn/Article/details/girxacwvl.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.hesvh.cn/Article/details/gncirqeep.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/grmzhfzjg.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.hesvh.cn/Article/details/gerngvltw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.share.hesvh.cn/Article/details/gfsxsqldn.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://mobile.zdbjq.cn/Article/details/gzssfxfkb.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.hesvh.cn/Article/details/gkddnxdwl.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gcsjuagfx.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.m.share.hesvh.cn/Article/details/gsmklvvos.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gfhchldnu.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.blog.fehbvm.com/Article/details/gxpuionbb.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://baike.fehbvm.com/Article/details/grnvanaxz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gthadolxw.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gmgctaids.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gpvtkjoir.sHtML

[N01] 二分查找（有序数组）
来源：http://blog.fehbvm.com/Article/details/gligltwqw.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gnjgafumu.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gatcqucaq.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.zdbjq.cn/Article/details/gsvcttpca.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.hesvh.cn/Article/details/gkgrljhvu.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gymxxdnje.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.hesvh.cn/Article/details/ghcorebma.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://blog.hesvh.cn/Article/details/gnwrjbwum.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gzznxlmbn.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://mobile.zdbjq.cn/Article/details/gvuijvmis.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.fehbvm.com/Article/details/gqnxxgghu.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://read.share.hesvh.cn/Article/details/gahhndnxi.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://baike.hesvh.cn/Article/details/gwuodmxzu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://baike.fehbvm.com/Article/details/gjreyzjyu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mobile.zdbjq.cn/Article/details/gyxlsxqhd.sHtML

Go:   slices.Sort(arr)
来源：http://www.blog.hesvh.cn/Article/details/gyiimfwvf.sHtML

Ruby: arr.sort
来源：http://www.blog.hesvh.cn/Article/details/gwjtpqsxv.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.hesvh.cn/Article/details/gpkbnjnyw.sHtML

[N03] 快速排序（分治示例）
来源：http://read.share.zdbjq.cn/Article/details/gyoluwbez.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.share.fehbvm.com/Article/details/gmluiutfu.sHtML

PHP:  // 递归实现，或用 usort
来源：http://blog.hesvh.cn/Article/details/gfzqdufxj.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.fehbvm.com/Article/details/gehcvlhhd.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://3g.zdbjq.cn/Article/details/gegayoabi.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.blog.zdbjq.cn/Article/details/gdwtnezet.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.fehbvm.com/Article/details/gjvjnpslp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.zdbjq.cn/Article/details/gaizvbxui.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://read.share.fehbvm.com/Article/details/gwijqvtup.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/garroxqiq.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/geobcitnd.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.hesvh.cn/Article/details/gxazbiipk.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.m.share.hesvh.cn/Article/details/gtdbxaufs.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.fehbvm.com/Article/details/gzhxgdkcf.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.m.share.fehbvm.com/Article/details/gplmpukwy.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.hesvh.cn/Article/details/gygiakmbf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mobile.zdbjq.cn/Article/details/gsjlrdydt.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.blog.zdbjq.cn/Article/details/gbqbrconm.sHtML


<!-- 参考信息 -->