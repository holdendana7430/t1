代发 wailian999

Py:   (end - start).total_seconds()
来源：http://www.blog.hesvh.cn/Article/details/gfufvlpmm.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.hesvh.cn/Article/details/gsbkfhypp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://wap.hesvh.cn/Article/details/gbaunzvht.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.blog.zdbjq.cn/Article/details/gtibutfbn.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://blog.fehbvm.com/Article/details/gzoeskjbj.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.share.fehbvm.com/Article/details/guwgafxij.sHtML

Ruby: end - start                 # 返回秒数
来源：http://wap.fehbvm.com/Article/details/gaqgoiwga.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.zdbjq.cn/Article/details/gonebeirk.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gjcwqxwiv.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://mobile.fehbvm.com/Article/details/gzuxzxoop.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.zdbjq.cn/Article/details/grahumytm.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.share.zdbjq.cn/Article/details/greoevjil.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.zdbjq.cn/Article/details/guvvuauwp.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gectnragb.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://read.share.zdbjq.cn/Article/details/guxtinihz.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.fehbvm.com/Article/details/gklgbwrfo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/glphaoiat.sHtML

[J08] 提取年月日与星期
来源：http://m.share.zdbjq.cn/Article/details/gacwnsfyi.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.zdbjq.cn/Article/details/gsrfwtqvd.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://read.share.zdbjq.cn/Article/details/gixhjppzt.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.fehbvm.com/Article/details/gcqhwjbxx.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://m.share.hesvh.cn/Article/details/gxymelahd.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.share.fehbvm.com/Article/details/glvaxabok.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.hesvh.cn/Article/details/gfaptapfx.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://read.share.fehbvm.com/Article/details/gwmcxkpyl.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.fehbvm.com/Article/details/gnxndpnly.sHtML

[J09] 时区处理
来源：http://www.blog.fehbvm.com/Article/details/gkzuuiesr.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gyoxamhuh.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://m.share.zdbjq.cn/Article/details/goafocfvc.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.fehbvm.com/Article/details/giziidsip.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/gsazxrndb.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.fehbvm.com/Article/details/gfhbedgeg.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.fehbvm.com/Article/details/gyerzqmfa.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://blog.zdbjq.cn/Article/details/ggvqossrb.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.hesvh.cn/Article/details/gjuuqlayj.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.zdbjq.cn/Article/details/graemrvdu.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gqlcegrmj.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://m.share.zdbjq.cn/Article/details/gnpzcguxw.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://read.share.fehbvm.com/Article/details/gfzxnfxsb.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mobile.hesvh.cn/Article/details/gacvcurum.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://3g.zdbjq.cn/Article/details/gxjydhaqb.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.fehbvm.com/Article/details/gbfahkwtt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.fehbvm.com/Article/details/gyywpitku.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/gqdajulut.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gexetcgii.sHtML

K. JSON 与序列化
来源：http://baike.zdbjq.cn/Article/details/gwgxpxwqe.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gvyyzanpu.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gdnehddzj.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/ggeloyfdk.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blog.hesvh.cn/Article/details/gqacxlsfy.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.fehbvm.com/Article/details/gxogdzbhx.sHtML

TS:   JSON.stringify(obj)
来源：http://m.share.fehbvm.com/Article/details/gifbrrjnq.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mobile.zdbjq.cn/Article/details/gohcrqqxq.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gweraoyik.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://m.share.fehbvm.com/Article/details/gxvdmeyzk.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.fehbvm.com/Article/details/ghxhyxyce.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/gvdpigxwb.sHtML

Py:   json.loads(s)
来源：http://m.share.fehbvm.com/Article/details/gufdytxyh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.blog.zdbjq.cn/Article/details/gheteukld.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gpsjwkjjo.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/gbzhtealk.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://m.share.hesvh.cn/Article/details/gsvuswgur.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.blog.hesvh.cn/Article/details/giyrbeyql.sHtML

Ruby: JSON.parse(s)
来源：http://blog.hesvh.cn/Article/details/gcnpyflus.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://3g.fehbvm.com/Article/details/gvpjbyaox.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://mobile.hesvh.cn/Article/details/gjxcxarhz.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gpkysyluu.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://baike.fehbvm.com/Article/details/ghlmroltf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://baike.zdbjq.cn/Article/details/gcuggycoq.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://m.share.hesvh.cn/Article/details/glykztsfj.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://read.share.zdbjq.cn/Article/details/gvjgpaygq.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gqtyorkxk.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.hesvh.cn/Article/details/gulmtjjfk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://blog.fehbvm.com/Article/details/gelxirxmz.sHtML

[K04] 读取 JSON 文件
来源：http://m.share.fehbvm.com/Article/details/gwtdgjkwu.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://mobile.hesvh.cn/Article/details/gbngoecvo.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.blog.fehbvm.com/Article/details/gwbivquzn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gkcbqxeug.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/godibljgy.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.share.zdbjq.cn/Article/details/gpxwsxikz.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.zdbjq.cn/Article/details/ggwewnnhl.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://blog.zdbjq.cn/Article/details/ggyketmzw.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://read.share.hesvh.cn/Article/details/gueuntnnf.sHtML

[K05] 深拷贝对象
来源：http://blog.zdbjq.cn/Article/details/gudfnelbm.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gvynpmbtq.sHtML

PHP:  unserialize(serialize($obj));
来源：http://blog.hesvh.cn/Article/details/garkprcyy.sHtML

JS:   structuredClone(obj)
来源：http://mobile.fehbvm.com/Article/details/ggkvadrym.sHtML

TS:   structuredClone(obj)
来源：http://baike.fehbvm.com/Article/details/gldjbpycn.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/ggtnhqxne.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://read.share.zdbjq.cn/Article/details/ghsfmzgcf.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://m.share.hesvh.cn/Article/details/gdfqbtlbn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.fehbvm.com/Article/details/gfxgstoan.sHtML

[K06] 解析 URL 查询串
来源：http://blog.hesvh.cn/Article/details/gcsnisadp.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.m.share.zdbjq.cn/Article/details/gfdodobao.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.fehbvm.com/Article/details/ggeajgsww.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gxhfhekue.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.zdbjq.cn/Article/details/gltbfjcxt.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://read.share.hesvh.cn/Article/details/gbomicvkt.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://mobile.fehbvm.com/Article/details/gvpsledvm.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.fehbvm.com/Article/details/gvyrndtce.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gisdydfeb.sHtML

[K07] 进制转换
来源：http://blog.hesvh.cn/Article/details/ghblgvaut.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gdstflujx.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://3g.zdbjq.cn/Article/details/gmwuhthux.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://baike.fehbvm.com/Article/details/gnnrezstm.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/gdluaoepd.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gtzsahbio.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gglkrbrop.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.m.share.zdbjq.cn/Article/details/grzggmchv.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gowaarzpo.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.blog.fehbvm.com/Article/details/gwzvwnzfr.sHtML

Py:   pickle.dumps(obj)
来源：http://blog.zdbjq.cn/Article/details/gsajyeknr.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.fehbvm.com/Article/details/gvfnugsgw.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gaqnjowpw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.share.hesvh.cn/Article/details/gysbmnaqd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://baike.fehbvm.com/Article/details/gtdkscuiu.sHtML

Go:   encoding/gob
来源：http://read.share.zdbjq.cn/Article/details/glkaadmwp.sHtML

Ruby: Marshal.dump(obj)
来源：http://read.share.zdbjq.cn/Article/details/glkkiiwvm.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.fehbvm.com/Article/details/gwzgpwexj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gqerhapuj.sHtML

L. 网络请求
来源：http://m.share.fehbvm.com/Article/details/gcxkguymv.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glajyjmdm.sHtML

[L01] 发送 GET 请求
来源：http://www.m.share.hesvh.cn/Article/details/gaumuljqm.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://3g.hesvh.cn/Article/details/gkzdskypu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://mobile.zdbjq.cn/Article/details/gpjjoulyf.sHtML

JS:   await fetch(url)
来源：http://baike.zdbjq.cn/Article/details/gaoezlsob.sHtML

TS:   await fetch(url)
来源：http://mobile.zdbjq.cn/Article/details/gppsepbyn.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://baike.fehbvm.com/Article/details/glkpgumiv.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.zdbjq.cn/Article/details/gkzfkqzmq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://mobile.hesvh.cn/Article/details/gpwjudpgv.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://blog.zdbjq.cn/Article/details/gytorxnwp.sHtML

[L02] 发送 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gneyowusl.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.zdbjq.cn/Article/details/gigeuxshl.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.share.fehbvm.com/Article/details/gacerytxc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/ggctqughn.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://baike.zdbjq.cn/Article/details/gkjfxnail.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.hesvh.cn/Article/details/gzemvgsdb.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gnnafoxoc.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mobile.zdbjq.cn/Article/details/gipcgrxzt.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.zdbjq.cn/Article/details/geuspofcs.sHtML

[L03] 设置自定义请求头
来源：http://baike.fehbvm.com/Article/details/gdwwbcyru.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.m.share.hesvh.cn/Article/details/gvoifbyae.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.fehbvm.com/Article/details/gybiexyhl.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.fehbvm.com/Article/details/gnusdgxmf.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.zdbjq.cn/Article/details/gjuufpbwl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://blog.hesvh.cn/Article/details/gfhcvkoes.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://blog.hesvh.cn/Article/details/gmahrrqlc.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.zdbjq.cn/Article/details/gurwwwumj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gmtxwogqm.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/ggyzzyhht.sHtML

Py:   requests.get(url, timeout=5)
来源：http://m.share.zdbjq.cn/Article/details/gwhkzogoj.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.zdbjq.cn/Article/details/gubwqgqad.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.hesvh.cn/Article/details/grjwhjxlz.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.hesvh.cn/Article/details/gdcnzsoom.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.blog.hesvh.cn/Article/details/gxcylikvs.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.blog.zdbjq.cn/Article/details/gtbixpeno.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gaszzpicu.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://blog.fehbvm.com/Article/details/gnjmsypmw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gbhtsxgkg.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wap.hesvh.cn/Article/details/gopaukbif.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.m.share.zdbjq.cn/Article/details/gixmrrjaj.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.fehbvm.com/Article/details/gnlhvysyb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gdeszndds.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.hesvh.cn/Article/details/gacedaocy.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.blog.zdbjq.cn/Article/details/gkfrshdol.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://baike.hesvh.cn/Article/details/gbpysjasx.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blog.hesvh.cn/Article/details/gbfrbvquh.sHtML

[L06] 解析响应为 JSON
来源：http://read.share.hesvh.cn/Article/details/gpypfmzof.sHtML

Py:   resp.json()
来源：http://mobile.fehbvm.com/Article/details/gdkpddygu.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/gylhxipic.sHtML

JS:   await resp.json()
来源：http://m.share.fehbvm.com/Article/details/gbjtdfwlx.sHtML

TS:   await resp.json()
来源：http://baike.hesvh.cn/Article/details/geoddenrl.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.hesvh.cn/Article/details/gdqhivsfy.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.blog.hesvh.cn/Article/details/gjordpkxo.sHtML

Ruby: JSON.parse(resp.body)
来源：http://read.share.zdbjq.cn/Article/details/gojpljpfs.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.fehbvm.com/Article/details/gzesmqylc.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gddpjehat.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gnjnehqzf.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.hesvh.cn/Article/details/gbwctwvwi.sHtML

JS:   resp.ok;  resp.status
来源：http://3g.zdbjq.cn/Article/details/gdsxezxza.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.hesvh.cn/Article/details/gswoqzquy.sHtML

Java: resp.statusCode()
来源：http://m.share.hesvh.cn/Article/details/gvyxmwzmw.sHtML

Go:   resp.StatusCode
来源：http://read.share.zdbjq.cn/Article/details/gaaignkhq.sHtML

Ruby: resp.code.to_i
来源：http://read.share.fehbvm.com/Article/details/gvofcxpnt.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/ggpfezuly.sHtML

[L08] 并发请求多个地址
来源：http://www.share.hesvh.cn/Article/details/glegyzbvv.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gndkancpl.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.zdbjq.cn/Article/details/goelloplo.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gocuaffaf.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gdgrpyygp.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://blog.hesvh.cn/Article/details/gdtoamoel.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.fehbvm.com/Article/details/gvilymaet.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.blog.zdbjq.cn/Article/details/guniivexa.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.m.share.hesvh.cn/Article/details/gdiwyqsiv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gijwxfssr.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.zdbjq.cn/Article/details/grlstfasg.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gmtffuadl.sHtML

[M01] 读取命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/gmghybvck.sHtML

Py:   sys.argv[1:]
来源：http://www.share.zdbjq.cn/Article/details/gjniuyvkm.sHtML

PHP:  $argv;  $argc;
来源：http://m.share.fehbvm.com/Article/details/ggeqjehhe.sHtML

JS:   process.argv.slice(2)
来源：http://blog.fehbvm.com/Article/details/gjijfwjaa.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gwftiigjn.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.zdbjq.cn/Article/details/gigpcseos.sHtML

Go:   os.Args[1:]
来源：http://www.m.share.fehbvm.com/Article/details/gntsbeewt.sHtML

Ruby: ARGV
来源：http://blog.zdbjq.cn/Article/details/gyzxyahqd.sHtML

C#:   args 数组（Main 方法参数）
来源：http://m.share.zdbjq.cn/Article/details/gtkpsuwnz.sHtML

[M02] 读取环境变量
来源：http://blog.zdbjq.cn/Article/details/gjbshrkyg.sHtML

Py:   os.environ.get("HOME")
来源：http://m.share.hesvh.cn/Article/details/ghfjeuavn.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/gsrxuhhfv.sHtML

JS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gtgapufai.sHtML

TS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gdomjokau.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/ggdkjihrn.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gqfaskjyh.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/glqimiqki.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://m.share.zdbjq.cn/Article/details/gxcbwtzwq.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gtsqaeyjh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://3g.fehbvm.com/Article/details/gkcwxjcpd.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/gcvrvobcb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/gbswhfqom.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.hesvh.cn/Article/details/gamuyusdz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.hesvh.cn/Article/details/gnzckqxyq.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.zdbjq.cn/Article/details/gpzrzsuzq.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://blog.fehbvm.com/Article/details/gwwdamlvy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://3g.hesvh.cn/Article/details/gytetjahn.sHtML

[M04] 获取当前工作目录
来源：http://www.share.fehbvm.com/Article/details/gmzhfazoy.sHtML

Py:   os.getcwd()
来源：http://wap.fehbvm.com/Article/details/ghchnzxzh.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gpjouvdry.sHtML

JS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gqrdfeogc.sHtML

TS:   process.cwd()
来源：http://3g.fehbvm.com/Article/details/gejsdiuyt.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://baike.fehbvm.com/Article/details/gcqlxajgw.sHtML

Go:   os.Getwd()
来源：http://3g.zdbjq.cn/Article/details/gaigrrnht.sHtML

Ruby: Dir.pwd
来源：http://blog.hesvh.cn/Article/details/gpuxyohxw.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.hesvh.cn/Article/details/gvqgerplt.sHtML

[M05] 设置退出码
来源：http://blog.zdbjq.cn/Article/details/gdrjpkmlm.sHtML

Py:   sys.exit(1)
来源：http://www.share.hesvh.cn/Article/details/grqxlkscu.sHtML

PHP:  exit(1);
来源：http://baike.fehbvm.com/Article/details/gmnyhvpue.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gfkogefed.sHtML

TS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/gjdqxqmum.sHtML

Java: System.exit(1)
来源：http://m.share.hesvh.cn/Article/details/gvereuggj.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxjoninlw.sHtML

Ruby: exit 1
来源：http://mobile.fehbvm.com/Article/details/gpfhfgztp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gvbshrcbb.sHtML

[M06] 向标准错误输出
来源：http://blog.zdbjq.cn/Article/details/gwgxepjnq.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.hesvh.cn/Article/details/gtuxerzmf.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.hesvh.cn/Article/details/ghittsapb.sHtML

JS:   console.error("err")
来源：http://baike.hesvh.cn/Article/details/gfcymezme.sHtML

TS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gnhgnwvnw.sHtML

Java: System.err.println("err")
来源：http://m.share.zdbjq.cn/Article/details/gspnknnlx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://read.share.hesvh.cn/Article/details/gofuczfqo.sHtML

Ruby: warn "err"
来源：http://baike.hesvh.cn/Article/details/gsyjvwhju.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.m.share.hesvh.cn/Article/details/gdwlaeuaf.sHtML

[M07] 判断是否为主入口
来源：http://blog.hesvh.cn/Article/details/gswlefqrt.sHtML

Py:   if __name__ == "__main__":
来源：http://www.m.share.hesvh.cn/Article/details/gbnnycndz.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://m.share.fehbvm.com/Article/details/gzepfazec.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/goduwsibi.sHtML

TS:   require.main === module
来源：http://baike.hesvh.cn/Article/details/gjvvrmgho.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gcwwjflod.sHtML

Go:   func main()
来源：http://www.m.share.fehbvm.com/Article/details/gfcsfvgms.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.fehbvm.com/Article/details/gxphgrtzl.sHtML

C#:   static void Main(string[] args)
来源：http://mobile.fehbvm.com/Article/details/ggzeakblg.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.zdbjq.cn/Article/details/gcltinfho.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.blog.zdbjq.cn/Article/details/gdisdefvj.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.zdbjq.cn/Article/details/gastdkvps.sHtML

JS:   process.platform;  process.version
来源：http://read.share.hesvh.cn/Article/details/gsutttpvb.sHtML

TS:   process.platform;  process.version
来源：http://m.share.hesvh.cn/Article/details/grubqgptd.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.blog.zdbjq.cn/Article/details/gabgbswry.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.m.share.hesvh.cn/Article/details/gazldrbsm.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.hesvh.cn/Article/details/glmsvdyzm.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.m.share.hesvh.cn/Article/details/gzhcqafdp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/grxqswsnv.sHtML

N. 数据结构与算法
来源：http://3g.zdbjq.cn/Article/details/gbmtnhhic.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gayecarrj.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.fehbvm.com/Article/details/gtrfzlecx.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gxebfezzs.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gwbvxvsgx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.blog.hesvh.cn/Article/details/gmzxysmvl.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://baike.hesvh.cn/Article/details/gylrjpxxa.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gkutpymzg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gcqfbvtrc.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://m.share.fehbvm.com/Article/details/gitaisvfd.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gjpnvfrkz.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://read.share.hesvh.cn/Article/details/gcywuwfzw.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://www.blog.fehbvm.com/Article/details/gprkezyjs.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://www.blog.zdbjq.cn/Article/details/gbpshopkd.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.zdbjq.cn/Article/details/gdrwqcvcg.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://blog.zdbjq.cn/Article/details/ghywgpycn.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.m.share.hesvh.cn/Article/details/gqruoxqxl.sHtML

Go:   slices.Sort(arr)
来源：http://blog.hesvh.cn/Article/details/gyudstfni.sHtML

Ruby: arr.sort
来源：http://baike.hesvh.cn/Article/details/grtvofijo.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.blog.hesvh.cn/Article/details/gsikfgnxd.sHtML

[N03] 快速排序（分治示例）
来源：http://blog.fehbvm.com/Article/details/gvkkcknox.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.zdbjq.cn/Article/details/gbqjluzgw.sHtML

PHP:  // 递归实现，或用 usort
来源：http://3g.hesvh.cn/Article/details/gwpxjqwal.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.hesvh.cn/Article/details/gezgodhmu.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fehbvm.com/Article/details/gplbgcnxe.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://m.share.fehbvm.com/Article/details/gwrrwlqya.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://3g.zdbjq.cn/Article/details/grmwzndoo.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mobile.fehbvm.com/Article/details/gysgdiklj.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.m.share.hesvh.cn/Article/details/gggxdgmvv.sHtML

[N04] 斐波那契数列
来源：http://baike.zdbjq.cn/Article/details/gatnnopxn.sHtML


<!-- 参考信息 -->