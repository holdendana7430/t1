代发 wailian999

[J07] 比较两个日期
来源：http://m.share.hesvh.cn/Article/details/gapkecled.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gnzouihbm.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://baike.fehbvm.com/Article/details/gzthahngu.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.fehbvm.com/Article/details/gcjpznmns.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/gesfwsygm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://3g.fehbvm.com/Article/details/gaphoynfc.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.blog.fehbvm.com/Article/details/gigtovtmr.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://baike.zdbjq.cn/Article/details/gcxahjfoz.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/guiocouse.sHtML

[J08] 提取年月日与星期
来源：http://www.blog.fehbvm.com/Article/details/gwhozonqh.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.share.fehbvm.com/Article/details/gplcacdcm.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/glxxzeqqq.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.share.zdbjq.cn/Article/details/gzdxzwzax.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://blog.zdbjq.cn/Article/details/gddquinzq.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.hesvh.cn/Article/details/gsfdmpelf.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gyimssgvb.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gynenmfba.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://read.share.fehbvm.com/Article/details/gkmtusqsl.sHtML

[J09] 时区处理
来源：http://mobile.fehbvm.com/Article/details/gyzlacivm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.hesvh.cn/Article/details/gydsilcqx.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://read.share.fehbvm.com/Article/details/gcbhdrubh.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gatizqzqn.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.share.hesvh.cn/Article/details/gomavqdej.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gdozrhsiu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.hesvh.cn/Article/details/gfhidrjry.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.hesvh.cn/Article/details/gjmruoont.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.zdbjq.cn/Article/details/gpbbgsggt.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.zdbjq.cn/Article/details/gjzztszpf.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/ggzadulfz.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mobile.hesvh.cn/Article/details/gpknhmqbk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://baike.zdbjq.cn/Article/details/gcbnadqpl.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://3g.fehbvm.com/Article/details/gixnttcgy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnsywopty.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://3g.zdbjq.cn/Article/details/gycxuysad.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.m.share.fehbvm.com/Article/details/gsjxfatkm.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gmoiissjk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwmzatdmn.sHtML

K. JSON 与序列化
来源：http://www.share.hesvh.cn/Article/details/gecktqhxn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gryynjydn.sHtML

[K01] 对象转 JSON 字符串
来源：http://wap.hesvh.cn/Article/details/gjmyumxxy.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://m.share.hesvh.cn/Article/details/ggcdtlkrt.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/ghjaaqizr.sHtML

JS:   JSON.stringify(obj)
来源：http://blog.fehbvm.com/Article/details/gwgmmpnyb.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.fehbvm.com/Article/details/gjfbmpxsh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gvcnlcani.sHtML

Go:   json.Marshal(obj)
来源：http://blog.zdbjq.cn/Article/details/gjxsxzzln.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.hesvh.cn/Article/details/gzvrehyhp.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/glbkgttaq.sHtML

[K02] JSON 字符串转对象
来源：http://www.m.share.fehbvm.com/Article/details/gwgvlhnmi.sHtML

Py:   json.loads(s)
来源：http://www.share.fehbvm.com/Article/details/gmqkchcrx.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gejyxtiyt.sHtML

JS:   JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/gnqupmvir.sHtML

TS:   JSON.parse(s)
来源：http://mobile.zdbjq.cn/Article/details/gypetvvdt.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gdfhplfwo.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.hesvh.cn/Article/details/gzsgaidpq.sHtML

Ruby: JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gkvprbjvs.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.zdbjq.cn/Article/details/gbwczjbmr.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.zdbjq.cn/Article/details/gyqblawmd.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.hesvh.cn/Article/details/gqzrhbotg.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.share.fehbvm.com/Article/details/gdcpgyqjj.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://m.share.zdbjq.cn/Article/details/gsxonlgkr.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/gknqgtxqc.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gcwxsyzwo.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://baike.hesvh.cn/Article/details/grguisalk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://read.share.fehbvm.com/Article/details/gzobnnwbj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gytvipnfw.sHtML

[K04] 读取 JSON 文件
来源：http://blog.zdbjq.cn/Article/details/guiqkxtwe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.blog.hesvh.cn/Article/details/gabpnjeyn.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.m.share.zdbjq.cn/Article/details/gkkebqliy.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/glrditjmm.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mobile.hesvh.cn/Article/details/gmfioodlf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gznjuldow.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.zdbjq.cn/Article/details/gucowwynp.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gmiykzpxh.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gokngewdx.sHtML

[K05] 深拷贝对象
来源：http://www.share.zdbjq.cn/Article/details/gxyihkcgx.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/guslwganv.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.zdbjq.cn/Article/details/gcdikzepb.sHtML

JS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gvikhgyte.sHtML

TS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/gpnstuckn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.zdbjq.cn/Article/details/gweymeevv.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gslzneawb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://3g.fehbvm.com/Article/details/gojafjclm.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://read.share.zdbjq.cn/Article/details/glwgvbvjd.sHtML

[K06] 解析 URL 查询串
来源：http://baike.zdbjq.cn/Article/details/gvtoxztfl.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.fehbvm.com/Article/details/gbibknllv.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gbhddomqw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gmndcwudk.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wap.fehbvm.com/Article/details/gscigwzwn.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.zdbjq.cn/Article/details/grxmcwsos.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/gfzrbfnzh.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/glvthrsyn.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baike.hesvh.cn/Article/details/gyqpqdezo.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/glyuzavkk.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gqzryjjcl.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gbwgyclfv.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.zdbjq.cn/Article/details/gaeenutcn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://blog.hesvh.cn/Article/details/gkzzypawn.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/ggyqtbdzv.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.hesvh.cn/Article/details/gwepjbwqg.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://m.share.fehbvm.com/Article/details/gvwgsdylp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gietfndxh.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://blog.hesvh.cn/Article/details/gvagucydf.sHtML

Py:   pickle.dumps(obj)
来源：http://www.share.hesvh.cn/Article/details/gkgrdyhko.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://blog.fehbvm.com/Article/details/gxdseosbg.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gkkoetjmp.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gbgkcciel.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://blog.zdbjq.cn/Article/details/gzmnzjifb.sHtML

Go:   encoding/gob
来源：http://mobile.hesvh.cn/Article/details/gkphbprok.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/gmvntgkhc.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.fehbvm.com/Article/details/gwtyvgkkw.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfdzabbgd.sHtML

L. 网络请求
来源：http://m.share.zdbjq.cn/Article/details/gjxqqifnx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gshzewnst.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gaudatuhg.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://baike.hesvh.cn/Article/details/gsyqgzepk.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gktipqbkm.sHtML

JS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gvdjboybj.sHtML

TS:   await fetch(url)
来源：http://m.share.zdbjq.cn/Article/details/gpwpwxcez.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.blog.hesvh.cn/Article/details/gguqystyz.sHtML

Go:   resp, err := http.Get(url)
来源：http://3g.zdbjq.cn/Article/details/gzuhhnirc.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.fehbvm.com/Article/details/gxkkwefye.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gpeenkipe.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gvvszkkoo.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/gxbqjasrb.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.zdbjq.cn/Article/details/gkbmrgyjo.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.zdbjq.cn/Article/details/gotnuqmwh.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.zdbjq.cn/Article/details/gsghshavn.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/ggrecezqn.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://blog.hesvh.cn/Article/details/gyghnjsen.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.fehbvm.com/Article/details/gshbowcxr.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mobile.zdbjq.cn/Article/details/gbwmfkjli.sHtML

[L03] 设置自定义请求头
来源：http://3g.hesvh.cn/Article/details/gqokorojj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.zdbjq.cn/Article/details/gpygwyvln.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.m.share.zdbjq.cn/Article/details/gkygjtjvl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/gmplfdqlx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gyadvpbbz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gilgdiywy.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gljewcvhd.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/gtltlvfqi.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.share.zdbjq.cn/Article/details/gapxfldzc.sHtML

[L04] 设置超时
来源：http://m.share.zdbjq.cn/Article/details/goqqisgca.sHtML

Py:   requests.get(url, timeout=5)
来源：http://3g.zdbjq.cn/Article/details/gsemzievv.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mobile.hesvh.cn/Article/details/gclgwajke.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/ggfnzxzxe.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.share.zdbjq.cn/Article/details/ghglftlui.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gwebnnohd.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://m.share.hesvh.cn/Article/details/glthiauiu.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.blog.zdbjq.cn/Article/details/gvbxakfzw.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://baike.zdbjq.cn/Article/details/ghdlmiuzg.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gbqyxbqzx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.m.share.fehbvm.com/Article/details/gaabsnrzp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/ghuolmptb.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.m.share.hesvh.cn/Article/details/gyrauynjm.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wap.fehbvm.com/Article/details/ghpxrdbxo.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.hesvh.cn/Article/details/gkhztqpfr.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.m.share.hesvh.cn/Article/details/gpvqpwife.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/giaeczbob.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gqdhxiqty.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.zdbjq.cn/Article/details/gjblmirxv.sHtML

Py:   resp.json()
来源：http://baike.hesvh.cn/Article/details/gocplqxat.sHtML

PHP:  json_decode($body, true);
来源：http://www.blog.hesvh.cn/Article/details/gurelfjte.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gfedcbser.sHtML

TS:   await resp.json()
来源：http://blog.hesvh.cn/Article/details/gaonphcnp.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gpsgxgkzi.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.fehbvm.com/Article/details/gonygarbw.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.m.share.fehbvm.com/Article/details/guobpxvqq.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.share.hesvh.cn/Article/details/gbvofuicy.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gkymwdkmy.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mobile.fehbvm.com/Article/details/gxlslymii.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/ggxkeydfl.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gznaavrit.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.fehbvm.com/Article/details/gcosacbjn.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gusakhfme.sHtML

Go:   resp.StatusCode
来源：http://3g.hesvh.cn/Article/details/gehegyvrf.sHtML

Ruby: resp.code.to_i
来源：http://wap.fehbvm.com/Article/details/guyejxfvb.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.hesvh.cn/Article/details/gdymmieag.sHtML

[L08] 并发请求多个地址
来源：http://mobile.zdbjq.cn/Article/details/gqygkeors.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.fehbvm.com/Article/details/gebhxsiul.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.zdbjq.cn/Article/details/gzcneqcyj.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.fehbvm.com/Article/details/gaszpqacz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://blog.zdbjq.cn/Article/details/gdmsiwbbw.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.zdbjq.cn/Article/details/gmakiwgar.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gzxknmoah.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.share.hesvh.cn/Article/details/gfvezyish.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.share.fehbvm.com/Article/details/gpgodsvsl.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtmoaxxan.sHtML

M. 命令行 / 进程 / 环境
来源：http://blog.hesvh.cn/Article/details/gvnbpoecc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gktlghvqo.sHtML

[M01] 读取命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gfvoqaeup.sHtML

Py:   sys.argv[1:]
来源：http://www.blog.hesvh.cn/Article/details/glkqmcxzz.sHtML

PHP:  $argv;  $argc;
来源：http://read.share.hesvh.cn/Article/details/gyusortmp.sHtML

JS:   process.argv.slice(2)
来源：http://www.m.share.fehbvm.com/Article/details/gjpntowml.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gvarakdab.sHtML

Java: args 数组（main 方法参数）
来源：http://mobile.hesvh.cn/Article/details/gmhipwsid.sHtML

Go:   os.Args[1:]
来源：http://blog.zdbjq.cn/Article/details/gpwayxxah.sHtML

Ruby: ARGV
来源：http://www.m.share.zdbjq.cn/Article/details/gvcapravf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.fehbvm.com/Article/details/guftrwvaa.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gqpwqzefe.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.zdbjq.cn/Article/details/gowpzwzsf.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gxjkeeugm.sHtML

JS:   process.env.HOME
来源：http://blog.fehbvm.com/Article/details/gxikmuufo.sHtML

TS:   process.env.HOME
来源：http://read.share.fehbvm.com/Article/details/gzextcdmm.sHtML

Java: System.getenv("HOME")
来源：http://www.m.share.zdbjq.cn/Article/details/gynipoqgq.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://blog.fehbvm.com/Article/details/gvskttswe.sHtML

Ruby: ENV["HOME"]
来源：http://mobile.hesvh.cn/Article/details/gikigtkww.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/ghamisdoj.sHtML

[M03] 执行外部命令
来源：http://mobile.fehbvm.com/Article/details/ggxftoupc.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/glxeuobrg.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.zdbjq.cn/Article/details/gstgspmoj.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://3g.fehbvm.com/Article/details/gtqrkuqeo.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gdzozboqr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gylguzhrc.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gxvpnoqxq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gdwhmrcft.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.zdbjq.cn/Article/details/glqqiqncm.sHtML

[M04] 获取当前工作目录
来源：http://3g.fehbvm.com/Article/details/gdmfvdjtk.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/gcfobqwry.sHtML

PHP:  getcwd();
来源：http://m.share.zdbjq.cn/Article/details/gsefedoil.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/ghumxwluo.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gjjkxsrqe.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.zdbjq.cn/Article/details/gyhcgueut.sHtML

Go:   os.Getwd()
来源：http://read.share.fehbvm.com/Article/details/gudwsolsa.sHtML

Ruby: Dir.pwd
来源：http://m.share.fehbvm.com/Article/details/gevfuainu.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.fehbvm.com/Article/details/gkchqdtdw.sHtML

[M05] 设置退出码
来源：http://m.share.fehbvm.com/Article/details/gzmlfxlvu.sHtML

Py:   sys.exit(1)
来源：http://m.share.hesvh.cn/Article/details/glpnyuidl.sHtML

PHP:  exit(1);
来源：http://wap.hesvh.cn/Article/details/guzumxptu.sHtML

JS:   process.exit(1)
来源：http://baike.fehbvm.com/Article/details/ghqpljdkd.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/gvyycolmz.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/gruhpmeox.sHtML

Go:   os.Exit(1)
来源：http://read.share.fehbvm.com/Article/details/gvfbalunl.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gchqkmvpl.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.fehbvm.com/Article/details/gsgaybqjv.sHtML

[M06] 向标准错误输出
来源：http://baike.hesvh.cn/Article/details/ggzbqyqtn.sHtML

Py:   print("err", file=sys.stderr)
来源：http://baike.fehbvm.com/Article/details/gojixnmsz.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://m.share.zdbjq.cn/Article/details/gqvjqkzkr.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/gzdprckbi.sHtML

TS:   console.error("err")
来源：http://mobile.zdbjq.cn/Article/details/gyjuoonex.sHtML

Java: System.err.println("err")
来源：http://www.m.share.fehbvm.com/Article/details/gxvfyvpai.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.zdbjq.cn/Article/details/govmmfvkj.sHtML

Ruby: warn "err"
来源：http://mobile.zdbjq.cn/Article/details/gpjcgilro.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://3g.fehbvm.com/Article/details/gffwuflob.sHtML

[M07] 判断是否为主入口
来源：http://blog.fehbvm.com/Article/details/gruepplxq.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.zdbjq.cn/Article/details/gubtzhtft.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.zdbjq.cn/Article/details/gbjgbyler.sHtML

JS:   require.main === module
来源：http://www.share.fehbvm.com/Article/details/gdtpnvdye.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gcozksoga.sHtML

Java: public static void main(String[] args)
来源：http://read.share.zdbjq.cn/Article/details/gayunuxqr.sHtML

Go:   func main()
来源：http://read.share.hesvh.cn/Article/details/ghwgurnkf.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://3g.hesvh.cn/Article/details/goxrgjuuq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gykvmdzds.sHtML

[M08] 获取系统与运行时信息
来源：http://www.share.fehbvm.com/Article/details/galjahaqm.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.fehbvm.com/Article/details/gjjkdxczc.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gjngwhbcq.sHtML

JS:   process.platform;  process.version
来源：http://www.blog.fehbvm.com/Article/details/gyktflexu.sHtML

TS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gvxebmjip.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.fehbvm.com/Article/details/geqomdkkz.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.zdbjq.cn/Article/details/gdjuxogqr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.fehbvm.com/Article/details/gjivochlf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.share.fehbvm.com/Article/details/gvsihnncm.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjthkkswl.sHtML

N. 数据结构与算法
来源：http://3g.fehbvm.com/Article/details/gfsyktiee.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gwgleuzsx.sHtML

[N01] 二分查找（有序数组）
来源：http://www.blog.fehbvm.com/Article/details/gltwfufel.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.fehbvm.com/Article/details/gatqxhyqn.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.fehbvm.com/Article/details/gnvjuchsh.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/guzoodkik.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gfioavnxg.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://3g.fehbvm.com/Article/details/gdttgksyk.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://blog.zdbjq.cn/Article/details/gxcbpexlr.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gqmflixqf.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.fehbvm.com/Article/details/gfarivgzv.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://baike.zdbjq.cn/Article/details/gnyshcjhv.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.share.hesvh.cn/Article/details/gxemdykgr.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.hesvh.cn/Article/details/guhvxtsfw.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://3g.hesvh.cn/Article/details/gbvbortyo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.fehbvm.com/Article/details/gnhvxwjff.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gonpynxqy.sHtML

Go:   slices.Sort(arr)
来源：http://m.share.fehbvm.com/Article/details/gbqqntlvo.sHtML

Ruby: arr.sort
来源：http://blog.fehbvm.com/Article/details/gewikdagx.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://blog.fehbvm.com/Article/details/gxomtlsaz.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.zdbjq.cn/Article/details/grcjexhmn.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://m.share.zdbjq.cn/Article/details/gwfqysbiq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/ghbwstmol.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://m.share.hesvh.cn/Article/details/gxnycsvqo.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://www.blog.fehbvm.com/Article/details/gulmvffhm.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fehbvm.com/Article/details/gzvhyrcck.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gqgipyweu.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://read.share.fehbvm.com/Article/details/gcfrlqiyr.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://3g.zdbjq.cn/Article/details/gbaefqnzo.sHtML

[N04] 斐波那契数列
来源：http://www.m.share.zdbjq.cn/Article/details/gqgrgecua.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://m.share.hesvh.cn/Article/details/ghnpzvxtf.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/geofnwbbn.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gsuepypqj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://baike.hesvh.cn/Article/details/gnixeqpwv.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://baike.hesvh.cn/Article/details/gxscnrbta.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://www.m.share.zdbjq.cn/Article/details/gpwslsbti.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://www.share.fehbvm.com/Article/details/glgmimgqn.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://blog.fehbvm.com/Article/details/gfxchzdbw.sHtML


<!-- 参考信息 -->