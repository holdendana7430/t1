代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.fehbvm.com/Article/details/gxfutkfcw.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gkedtzpyu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.fehbvm.com/Article/details/gpcowzlcy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://read.share.fehbvm.com/Article/details/gekqfrefm.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gxhrbnudf.sHtML

[J08] 提取年月日与星期
来源：http://m.share.hesvh.cn/Article/details/ggnmeveqd.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.hesvh.cn/Article/details/gqtkdymoy.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.zdbjq.cn/Article/details/gfqdezwnr.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.m.share.zdbjq.cn/Article/details/gojsdomli.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gchvsoucp.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://read.share.hesvh.cn/Article/details/gpghmavkw.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.hesvh.cn/Article/details/gfkgleckj.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wap.hesvh.cn/Article/details/gwdntmpmh.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.share.hesvh.cn/Article/details/gaiegcruy.sHtML

[J09] 时区处理
来源：http://m.share.hesvh.cn/Article/details/gqkhyneuj.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.share.zdbjq.cn/Article/details/gfhilxspj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.zdbjq.cn/Article/details/gjpvtjgcy.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.zdbjq.cn/Article/details/geagkyqsx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://3g.hesvh.cn/Article/details/gpgreokvo.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mobile.hesvh.cn/Article/details/gaivsrcrh.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://blog.hesvh.cn/Article/details/gakufxins.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://www.blog.zdbjq.cn/Article/details/graklnelw.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mobile.fehbvm.com/Article/details/ggoiipvsq.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gtkzaswyh.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/gllvtzalc.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.zdbjq.cn/Article/details/gjrblzqkz.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.zdbjq.cn/Article/details/grmpjnqxf.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gthdwnvod.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gxjimbbod.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://mobile.fehbvm.com/Article/details/gdnmnehns.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gblljpxls.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvtzstxhu.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqvxzcovh.sHtML

K. JSON 与序列化
来源：http://read.share.hesvh.cn/Article/details/gqkhiwgdg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gxdxisgiw.sHtML

[K01] 对象转 JSON 字符串
来源：http://mobile.fehbvm.com/Article/details/giogtmrjm.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.m.share.zdbjq.cn/Article/details/gsumrrwuv.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.fehbvm.com/Article/details/ghfltpswq.sHtML

JS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/glrbstymm.sHtML

TS:   JSON.stringify(obj)
来源：http://3g.zdbjq.cn/Article/details/gfdatmbwh.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://baike.zdbjq.cn/Article/details/gyyzbwgjc.sHtML

Go:   json.Marshal(obj)
来源：http://wap.hesvh.cn/Article/details/gkfjgadxt.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.zdbjq.cn/Article/details/gjumpfezh.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://www.m.share.hesvh.cn/Article/details/ghbqwqoko.sHtML

[K02] JSON 字符串转对象
来源：http://baike.fehbvm.com/Article/details/gbxkywlfa.sHtML

Py:   json.loads(s)
来源：http://blog.fehbvm.com/Article/details/geglxniba.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mobile.zdbjq.cn/Article/details/gweibdrij.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gpydvujsv.sHtML

TS:   JSON.parse(s)
来源：http://m.share.fehbvm.com/Article/details/gkvoprurx.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.share.hesvh.cn/Article/details/genyquwvi.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://3g.zdbjq.cn/Article/details/gtswphuyv.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gawgmbfkt.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gzdstyqrj.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.hesvh.cn/Article/details/gnkhprqks.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gklvwpkjp.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/geylqkzti.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpoiencah.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.zdbjq.cn/Article/details/geiguwyxi.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wap.fehbvm.com/Article/details/gabwoviud.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gmaogisub.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://mobile.fehbvm.com/Article/details/gbxuulokq.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gmogkgjdf.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.hesvh.cn/Article/details/giappitzl.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gkpwvanjh.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.fehbvm.com/Article/details/gjoerkxlf.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gzpucnptj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gtiutuctf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://baike.zdbjq.cn/Article/details/gxmkqsjmh.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://m.share.hesvh.cn/Article/details/glrltywnl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.zdbjq.cn/Article/details/gnwxuecwf.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/gcjmcbsdx.sHtML

[K05] 深拷贝对象
来源：http://3g.hesvh.cn/Article/details/gizhddkiq.sHtML

Py:   copy.deepcopy(obj)
来源：http://wap.hesvh.cn/Article/details/gqhpizbjq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.fehbvm.com/Article/details/gxkempyem.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.hesvh.cn/Article/details/ghuezxcqi.sHtML

TS:   structuredClone(obj)
来源：http://mobile.hesvh.cn/Article/details/gixopnwgc.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.fehbvm.com/Article/details/gshmgyqtc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.m.share.fehbvm.com/Article/details/gbicookal.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://read.share.fehbvm.com/Article/details/gsemltwgr.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://www.m.share.zdbjq.cn/Article/details/gmfvegcwb.sHtML

[K06] 解析 URL 查询串
来源：http://www.blog.hesvh.cn/Article/details/gvzcxtpyo.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.share.hesvh.cn/Article/details/gmepfhhuz.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://m.share.hesvh.cn/Article/details/gzouongjh.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.zdbjq.cn/Article/details/gumxgvjvl.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gecqthrqi.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://mobile.fehbvm.com/Article/details/glbsqibix.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.zdbjq.cn/Article/details/gadtrdody.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wap.zdbjq.cn/Article/details/ggxrxpojt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/golhjbend.sHtML

[K07] 进制转换
来源：http://www.m.share.zdbjq.cn/Article/details/gmlkehlnf.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/ggvxzugqx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.fehbvm.com/Article/details/gxuwdbtsf.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gblfeomwm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.zdbjq.cn/Article/details/gidsqozjk.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gjcxwdkmh.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gavhpyclm.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.hesvh.cn/Article/details/gciiaycns.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://read.share.zdbjq.cn/Article/details/gzjflskyg.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.zdbjq.cn/Article/details/ghyiunddl.sHtML

Py:   pickle.dumps(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gqbbsgmcz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://m.share.hesvh.cn/Article/details/gqzzlgdgo.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gejavepqv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://wap.hesvh.cn/Article/details/gafjyusgn.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.zdbjq.cn/Article/details/grdvgiwrx.sHtML

Go:   encoding/gob
来源：http://www.m.share.hesvh.cn/Article/details/gktjaslkq.sHtML

Ruby: Marshal.dump(obj)
来源：http://www.blog.zdbjq.cn/Article/details/getcyadpo.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.share.zdbjq.cn/Article/details/gxdnpdzia.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/grkwoslur.sHtML

L. 网络请求
来源：http://www.blog.hesvh.cn/Article/details/gbxhkmnna.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gtlaoeped.sHtML

[L01] 发送 GET 请求
来源：http://mobile.hesvh.cn/Article/details/gxuqovmst.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mobile.fehbvm.com/Article/details/gnokkugzt.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.hesvh.cn/Article/details/ghnsbigxy.sHtML

JS:   await fetch(url)
来源：http://mobile.fehbvm.com/Article/details/gpunncymt.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gjgyzqrzp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://read.share.hesvh.cn/Article/details/gpzdyivew.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.hesvh.cn/Article/details/gjpkwrdsd.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/ggtwyrhue.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://3g.hesvh.cn/Article/details/gqxhhagdu.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/glctnmelu.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.fehbvm.com/Article/details/ghdxsigym.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://read.share.hesvh.cn/Article/details/gyvzhjsop.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gykmphbcd.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.fehbvm.com/Article/details/gryomkpsd.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.zdbjq.cn/Article/details/gowfnlfyd.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.m.share.fehbvm.com/Article/details/gdkthjezx.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://m.share.hesvh.cn/Article/details/gjqyunuea.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gziiaecyx.sHtML

[L03] 设置自定义请求头
来源：http://3g.zdbjq.cn/Article/details/gmuvysude.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gnlyyleyu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wap.hesvh.cn/Article/details/gptmktypj.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.hesvh.cn/Article/details/gtjsypxcz.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.m.share.zdbjq.cn/Article/details/gbkndadaj.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://read.share.fehbvm.com/Article/details/gtoftprvb.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gvhdunjes.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://m.share.hesvh.cn/Article/details/gnydqsacv.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://m.share.zdbjq.cn/Article/details/gvzibrcnu.sHtML

[L04] 设置超时
来源：http://www.blog.zdbjq.cn/Article/details/gtweinjvr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.fehbvm.com/Article/details/gzfqmdjmu.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wap.hesvh.cn/Article/details/gizhpsgri.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gkoqvwyno.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gzgdwumte.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://m.share.fehbvm.com/Article/details/goxdinsto.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.fehbvm.com/Article/details/glrqwfrcf.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gtraswafr.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.fehbvm.com/Article/details/gmbmssxzh.sHtML

[L05] 上传文件（multipart）
来源：http://mobile.fehbvm.com/Article/details/gmurjpiwq.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/girwyutmf.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gwzknyhtj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://blog.hesvh.cn/Article/details/gatfxligf.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.zdbjq.cn/Article/details/gaikciegi.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://m.share.fehbvm.com/Article/details/gmjyayaqw.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://baike.hesvh.cn/Article/details/gtauxgkkh.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.hesvh.cn/Article/details/ghayqkttb.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gumffyvvt.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gsnwymukm.sHtML

Py:   resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gssxdjqeh.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gzsnjlmop.sHtML

JS:   await resp.json()
来源：http://read.share.hesvh.cn/Article/details/gvdohujmm.sHtML

TS:   await resp.json()
来源：http://www.share.hesvh.cn/Article/details/gyazuggut.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.hesvh.cn/Article/details/grqcsibpf.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gmqvvvfey.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.hesvh.cn/Article/details/galxhfbje.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.m.share.zdbjq.cn/Article/details/ghmmdecki.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/ghdrozpbg.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gmotmhlwb.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.fehbvm.com/Article/details/gbflqgcvb.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gnwcpktow.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/garjvkbhl.sHtML

Java: resp.statusCode()
来源：http://read.share.hesvh.cn/Article/details/gpcrhywcw.sHtML

Go:   resp.StatusCode
来源：http://baike.fehbvm.com/Article/details/gaxtrkufl.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/gkojfsvva.sHtML

C#:   (int)resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gcjwejcpg.sHtML

[L08] 并发请求多个地址
来源：http://blog.zdbjq.cn/Article/details/gcggbrpag.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gvijlgghg.sHtML

PHP:  curl_multi_init() 系列
来源：http://baike.zdbjq.cn/Article/details/ghzmttaue.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.fehbvm.com/Article/details/gyhsjrkdc.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.zdbjq.cn/Article/details/gcpwdjyjb.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.m.share.zdbjq.cn/Article/details/gugjuvltg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/gypcyvblq.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.m.share.zdbjq.cn/Article/details/gtlvdvizj.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://blog.fehbvm.com/Article/details/gfjjtavdb.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjbwmszmc.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.share.hesvh.cn/Article/details/gfoyqglew.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxqyiptmc.sHtML

[M01] 读取命令行参数
来源：http://3g.hesvh.cn/Article/details/gjqhvzegt.sHtML

Py:   sys.argv[1:]
来源：http://m.share.fehbvm.com/Article/details/gdiyasucw.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gnmogwufs.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gkxawxfdc.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gayuojlfo.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.hesvh.cn/Article/details/gcupfdwit.sHtML

Go:   os.Args[1:]
来源：http://mobile.fehbvm.com/Article/details/ganvrvqog.sHtML

Ruby: ARGV
来源：http://read.share.fehbvm.com/Article/details/grnbecfxp.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gjijvjcgh.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gxmkiweck.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.hesvh.cn/Article/details/gigmkjdgr.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.hesvh.cn/Article/details/gimdxydlk.sHtML

JS:   process.env.HOME
来源：http://baike.fehbvm.com/Article/details/gaveylvhf.sHtML

TS:   process.env.HOME
来源：http://3g.zdbjq.cn/Article/details/gdiqdkbyy.sHtML

Java: System.getenv("HOME")
来源：http://blog.zdbjq.cn/Article/details/gjbzzrnns.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/ggmgvktpl.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.hesvh.cn/Article/details/gnokcywbq.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.m.share.hesvh.cn/Article/details/gfzbmwpet.sHtML

[M03] 执行外部命令
来源：http://www.m.share.fehbvm.com/Article/details/gkpcpxnsv.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.share.hesvh.cn/Article/details/gndyznbxr.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://m.share.zdbjq.cn/Article/details/gawdidxrb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gulqptgzq.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.hesvh.cn/Article/details/gfxnkvkio.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://m.share.fehbvm.com/Article/details/gwgzxbhgx.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gpcxocgpq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.fehbvm.com/Article/details/grdibolql.sHtML

C#:   Process.Start("ls", "-l");
来源：http://wap.fehbvm.com/Article/details/gnvxmkajr.sHtML

[M04] 获取当前工作目录
来源：http://www.blog.fehbvm.com/Article/details/gfrtwwwam.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/gwsbdhbhu.sHtML

PHP:  getcwd();
来源：http://www.m.share.fehbvm.com/Article/details/gyqrbdfdl.sHtML

JS:   process.cwd()
来源：http://blog.fehbvm.com/Article/details/gbwqbrqxl.sHtML

TS:   process.cwd()
来源：http://mobile.fehbvm.com/Article/details/grlgsrccs.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gvvqircuc.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/ggozfqjta.sHtML

Ruby: Dir.pwd
来源：http://www.share.hesvh.cn/Article/details/gobnnducs.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://baike.zdbjq.cn/Article/details/gyhtgsxrs.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/guefaegki.sHtML

Py:   sys.exit(1)
来源：http://read.share.fehbvm.com/Article/details/grbczzcdh.sHtML

PHP:  exit(1);
来源：http://www.blog.zdbjq.cn/Article/details/gizxzimzk.sHtML

JS:   process.exit(1)
来源：http://mobile.zdbjq.cn/Article/details/gdcqgkrvl.sHtML

TS:   process.exit(1)
来源：http://www.blog.fehbvm.com/Article/details/goptubzuy.sHtML

Java: System.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gptqwsrli.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/ghbnmeafn.sHtML

Ruby: exit 1
来源：http://wap.zdbjq.cn/Article/details/gaylilfdg.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://3g.zdbjq.cn/Article/details/gjcxhrecs.sHtML

[M06] 向标准错误输出
来源：http://www.blog.hesvh.cn/Article/details/gccwmdwzb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.fehbvm.com/Article/details/gurwhikew.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/ghgzihpxu.sHtML

JS:   console.error("err")
来源：http://www.blog.hesvh.cn/Article/details/gbzighzwx.sHtML

TS:   console.error("err")
来源：http://www.m.share.zdbjq.cn/Article/details/gnvwbravm.sHtML

Java: System.err.println("err")
来源：http://wap.fehbvm.com/Article/details/gtlmqhfmc.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.zdbjq.cn/Article/details/gtsvkwjbe.sHtML

Ruby: warn "err"
来源：http://mobile.hesvh.cn/Article/details/gpjfztquy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gtswcazwi.sHtML

[M07] 判断是否为主入口
来源：http://baike.hesvh.cn/Article/details/gxlsvtueh.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.zdbjq.cn/Article/details/gqanxttfk.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://mobile.hesvh.cn/Article/details/gshuoqjio.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gnpfqrgjn.sHtML

TS:   require.main === module
来源：http://mobile.hesvh.cn/Article/details/gcivqeeke.sHtML

Java: public static void main(String[] args)
来源：http://wap.hesvh.cn/Article/details/gtlgksdvs.sHtML

Go:   func main()
来源：http://www.blog.zdbjq.cn/Article/details/gsjelvfjg.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gtkmslcun.sHtML

C#:   static void Main(string[] args)
来源：http://3g.hesvh.cn/Article/details/gwktzegqp.sHtML

[M08] 获取系统与运行时信息
来源：http://read.share.fehbvm.com/Article/details/gomujudnq.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/ghpuvgwhb.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gnxsvotlx.sHtML

JS:   process.platform;  process.version
来源：http://blog.zdbjq.cn/Article/details/gmtdojtet.sHtML

TS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gjjiraxxt.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.fehbvm.com/Article/details/guifquiyn.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://baike.fehbvm.com/Article/details/goisuakem.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/gplkabljf.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.blog.zdbjq.cn/Article/details/gccraawtj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gprxkwbpp.sHtML

N. 数据结构与算法
来源：http://baike.hesvh.cn/Article/details/guibujqbv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gmestelhe.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.hesvh.cn/Article/details/gbemrnaat.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gihddrvfa.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.hesvh.cn/Article/details/gggzdufas.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://3g.zdbjq.cn/Article/details/gpngycsig.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/ghhpsnjye.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gagnqkobj.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://mobile.fehbvm.com/Article/details/gkcgbuspk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://wap.zdbjq.cn/Article/details/gjijpyygk.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://3g.hesvh.cn/Article/details/gdntysybm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://3g.hesvh.cn/Article/details/gpfuayywq.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://wap.hesvh.cn/Article/details/gxywhmwmf.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gwwumxdjg.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.zdbjq.cn/Article/details/gbwkfrvhy.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://www.share.hesvh.cn/Article/details/glffydtwx.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wap.fehbvm.com/Article/details/gyuudbvld.sHtML

Go:   slices.Sort(arr)
来源：http://3g.fehbvm.com/Article/details/gexajfwss.sHtML

Ruby: arr.sort
来源：http://www.m.share.zdbjq.cn/Article/details/glyoqdtxl.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://baike.fehbvm.com/Article/details/grxrzltav.sHtML

[N03] 快速排序（分治示例）
来源：http://www.blog.fehbvm.com/Article/details/gnrinlvoi.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gyhtatcjq.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gcujhznqp.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://baike.fehbvm.com/Article/details/ghjxaainn.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.fehbvm.com/Article/details/gspidkmau.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.share.fehbvm.com/Article/details/gbeymgjzp.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://read.share.hesvh.cn/Article/details/gulyfqkhw.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wap.hesvh.cn/Article/details/gkxxuhtdd.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://blog.zdbjq.cn/Article/details/gkjbyqtea.sHtML

[N04] 斐波那契数列
来源：http://www.share.hesvh.cn/Article/details/gtnpixeal.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mobile.fehbvm.com/Article/details/gaxdvgqxo.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://www.share.zdbjq.cn/Article/details/gdskgsuxf.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/glzzxswkc.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mobile.zdbjq.cn/Article/details/greygevtd.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://www.blog.zdbjq.cn/Article/details/gdzmwshiu.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://m.share.hesvh.cn/Article/details/gcasogzwf.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://3g.fehbvm.com/Article/details/gfcrrgccg.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://3g.fehbvm.com/Article/details/gkqngxoug.sHtML

[N05] 最大公约数
来源：http://www.m.share.fehbvm.com/Article/details/gtujfwzwf.sHtML

Py:   math.gcd(a, b)
来源：http://baike.hesvh.cn/Article/details/gkxekrrhi.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://www.share.zdbjq.cn/Article/details/gfsmfckwf.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://www.m.share.hesvh.cn/Article/details/grhohsjyj.sHtML


<!-- 参考信息 -->