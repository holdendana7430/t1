代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://baike.zdbjq.cn/Article/details/gkzhdbfyv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.fehbvm.com/Article/details/gicvaxmoz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gibnuqyyv.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://m.share.fehbvm.com/Article/details/gdzscszxi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gzpnitrsc.sHtML

Ruby: Time.now + 7 * 86400
来源：http://m.share.fehbvm.com/Article/details/ghpnrfykv.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.zdbjq.cn/Article/details/gwckwymfb.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/gwbvwvqkh.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.zdbjq.cn/Article/details/gqfqtdban.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.m.share.zdbjq.cn/Article/details/gfgoxmhqp.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://blog.hesvh.cn/Article/details/gofeeoiae.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wap.hesvh.cn/Article/details/gnhzxwsmg.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://m.share.zdbjq.cn/Article/details/gkdwcetew.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.hesvh.cn/Article/details/gflbyhvfd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://baike.fehbvm.com/Article/details/glzcqewvk.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/guakzbphp.sHtML

[J07] 比较两个日期
来源：http://m.share.fehbvm.com/Article/details/ggljqehsc.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://3g.hesvh.cn/Article/details/gutkhelte.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.m.share.fehbvm.com/Article/details/gawxlyzgz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gxoeyssng.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.hesvh.cn/Article/details/grzewgdvg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.zdbjq.cn/Article/details/gcvciedtt.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://3g.zdbjq.cn/Article/details/guztvbcjy.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.fehbvm.com/Article/details/gjmemcmeu.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gcsbrgfuk.sHtML

[J08] 提取年月日与星期
来源：http://3g.hesvh.cn/Article/details/gzcjsnkdy.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://m.share.fehbvm.com/Article/details/gyzhjimvo.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.hesvh.cn/Article/details/gohdenlgf.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://read.share.hesvh.cn/Article/details/gvmvxkmqg.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gpnejwlsm.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gptcxkrlo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://m.share.fehbvm.com/Article/details/gfzuixtdt.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.zdbjq.cn/Article/details/gqarhycjb.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gdztvlnrc.sHtML

[J09] 时区处理
来源：http://m.share.zdbjq.cn/Article/details/gvhsvpqbl.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.hesvh.cn/Article/details/gieoxrusp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.blog.hesvh.cn/Article/details/ggwahwrqd.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.m.share.hesvh.cn/Article/details/gticzksxc.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://m.share.hesvh.cn/Article/details/gvpszlnay.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://3g.fehbvm.com/Article/details/gznpyxwuu.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/ggspghmhn.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.fehbvm.com/Article/details/gxdoobdgi.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/gnqfxmkfa.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.zdbjq.cn/Article/details/gzuybicdc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://wap.fehbvm.com/Article/details/glnqajlcy.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://baike.fehbvm.com/Article/details/gnygrqrih.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gswncrzhz.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gxefcismk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wap.zdbjq.cn/Article/details/gesmpcupx.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gdlytqqjk.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mobile.zdbjq.cn/Article/details/gnidhhuga.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://3g.zdbjq.cn/Article/details/ghmartnjm.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gbnceqsbn.sHtML

K. JSON 与序列化
来源：http://blog.zdbjq.cn/Article/details/gzunzjxuy.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggfjsyfwx.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.fehbvm.com/Article/details/gebkumuta.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/gieudiivb.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.zdbjq.cn/Article/details/gdkxrbsqu.sHtML

JS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gxihywsnp.sHtML

TS:   JSON.stringify(obj)
来源：http://mobile.zdbjq.cn/Article/details/gfzzozthu.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.blog.zdbjq.cn/Article/details/gfvxohxut.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.fehbvm.com/Article/details/garpomaay.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.zdbjq.cn/Article/details/gcmwtarhc.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.hesvh.cn/Article/details/glrhbesnj.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.fehbvm.com/Article/details/gikekgjfa.sHtML

Py:   json.loads(s)
来源：http://blog.zdbjq.cn/Article/details/gqlugazpa.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://baike.zdbjq.cn/Article/details/gnlbwvlar.sHtML

JS:   JSON.parse(s)
来源：http://www.share.hesvh.cn/Article/details/gfcznevev.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gkslwfqli.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gxukvslqc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gdxsmbqtq.sHtML

Ruby: JSON.parse(s)
来源：http://www.blog.hesvh.cn/Article/details/ggvirrnvy.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://m.share.fehbvm.com/Article/details/gomgpyrzp.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.share.fehbvm.com/Article/details/ggrowbrsh.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/ggjgwbyez.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://read.share.fehbvm.com/Article/details/gevpvfisy.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.share.fehbvm.com/Article/details/ghtuqtsow.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gfvqamlsz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.blog.fehbvm.com/Article/details/gweluohbb.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://mobile.hesvh.cn/Article/details/gkqinkcue.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://3g.zdbjq.cn/Article/details/gbrajcnkj.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.fehbvm.com/Article/details/gzqmomlzk.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gwnkjiptj.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.share.zdbjq.cn/Article/details/gwpwjchba.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://read.share.fehbvm.com/Article/details/gdvmptajn.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://baike.hesvh.cn/Article/details/gqkyadtnj.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://m.share.zdbjq.cn/Article/details/gicysfgdf.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.fehbvm.com/Article/details/gymwexozo.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.hesvh.cn/Article/details/gkrjoptdf.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gugjsusgz.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.zdbjq.cn/Article/details/gnzsplbrz.sHtML

[K05] 深拷贝对象
来源：http://m.share.hesvh.cn/Article/details/glkknlbaz.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.hesvh.cn/Article/details/gqtwmxpqz.sHtML

PHP:  unserialize(serialize($obj));
来源：http://baike.zdbjq.cn/Article/details/grifiqlxe.sHtML

JS:   structuredClone(obj)
来源：http://www.blog.fehbvm.com/Article/details/guxprubxd.sHtML

TS:   structuredClone(obj)
来源：http://3g.hesvh.cn/Article/details/gvszeuxgj.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://read.share.fehbvm.com/Article/details/gwehckzpn.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://baike.fehbvm.com/Article/details/gcgsanlki.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://blog.zdbjq.cn/Article/details/gmtigznkn.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://blog.zdbjq.cn/Article/details/gaxwhzxon.sHtML

[K06] 解析 URL 查询串
来源：http://www.m.share.hesvh.cn/Article/details/gcfcskejr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://baike.fehbvm.com/Article/details/gkcimosqb.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://3g.hesvh.cn/Article/details/gxezuvmzj.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.zdbjq.cn/Article/details/gagqitepe.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/grltmjnsh.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://3g.fehbvm.com/Article/details/gpggcfpbu.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.hesvh.cn/Article/details/gfwftmvwn.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://blog.fehbvm.com/Article/details/gdzdqgshf.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/ghjhcssyf.sHtML

[K07] 进制转换
来源：http://wap.zdbjq.cn/Article/details/gkhyjrukb.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gswbawije.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.blog.zdbjq.cn/Article/details/gbblqvdfg.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.fehbvm.com/Article/details/geduhdnmf.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://mobile.zdbjq.cn/Article/details/gtepbsbsu.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.hesvh.cn/Article/details/gmrjyqjrj.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.zdbjq.cn/Article/details/gesgmhxcc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gtimqqxip.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://baike.hesvh.cn/Article/details/ggroozdht.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.fehbvm.com/Article/details/gcyduzvma.sHtML

Py:   pickle.dumps(obj)
来源：http://www.blog.fehbvm.com/Article/details/gydcwqpxi.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://baike.zdbjq.cn/Article/details/gkpjdeppr.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://wap.zdbjq.cn/Article/details/gricyriux.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.fehbvm.com/Article/details/gnioimfbp.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://read.share.zdbjq.cn/Article/details/govutrzfz.sHtML

Go:   encoding/gob
来源：http://3g.fehbvm.com/Article/details/gdghksvof.sHtML

Ruby: Marshal.dump(obj)
来源：http://m.share.hesvh.cn/Article/details/gnlesspty.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gchimovqq.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gituujtno.sHtML

L. 网络请求
来源：http://blog.fehbvm.com/Article/details/gdihqbmyx.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gpkmcbmol.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gxgexksto.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.hesvh.cn/Article/details/gwhlztpaj.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://3g.zdbjq.cn/Article/details/gvvdfuttn.sHtML

JS:   await fetch(url)
来源：http://wap.hesvh.cn/Article/details/guvzmsjla.sHtML

TS:   await fetch(url)
来源：http://read.share.zdbjq.cn/Article/details/guekvfreo.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wap.fehbvm.com/Article/details/gqjlzldvq.sHtML

Go:   resp, err := http.Get(url)
来源：http://wap.fehbvm.com/Article/details/gxpdimxha.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://read.share.zdbjq.cn/Article/details/gfcchlpaz.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.fehbvm.com/Article/details/gsbrxeisl.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gwrqkycno.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.hesvh.cn/Article/details/glegyyewc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://baike.zdbjq.cn/Article/details/gcyomyarv.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gcsvcpffm.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://blog.hesvh.cn/Article/details/gsbddlenc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/goyjkwinl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.zdbjq.cn/Article/details/gawusctno.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/gpqtwbmmd.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://blog.zdbjq.cn/Article/details/gfpomnlxq.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gsnccadsj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://blog.fehbvm.com/Article/details/gbcewthqa.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://3g.fehbvm.com/Article/details/gdwlnoopm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blog.hesvh.cn/Article/details/gazzcgxrp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://baike.zdbjq.cn/Article/details/gpavgasjx.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://m.share.fehbvm.com/Article/details/goxcuahey.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gjbddtaoz.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://read.share.fehbvm.com/Article/details/gygypljtq.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wap.fehbvm.com/Article/details/gqzxpfppg.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gokmrskgv.sHtML

Py:   requests.get(url, timeout=5)
来源：http://blog.hesvh.cn/Article/details/gjfpqyazk.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.fehbvm.com/Article/details/gvbbdpxlr.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.m.share.fehbvm.com/Article/details/gmfqtevbf.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.hesvh.cn/Article/details/ggxudseeh.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.zdbjq.cn/Article/details/gthtmiwkj.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mobile.hesvh.cn/Article/details/grquxzaws.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.hesvh.cn/Article/details/gveorojqa.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gqbhffpgn.sHtML

[L05] 上传文件（multipart）
来源：http://blog.zdbjq.cn/Article/details/gputxxabz.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://blog.hesvh.cn/Article/details/gfiqccwlj.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://read.share.fehbvm.com/Article/details/gfgmhfujm.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/gonzrvirj.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.share.fehbvm.com/Article/details/gjdzchgzt.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.hesvh.cn/Article/details/grdldfjxq.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gkhqjetbm.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://m.share.fehbvm.com/Article/details/gsugapvti.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gexeyyfno.sHtML

[L06] 解析响应为 JSON
来源：http://blog.hesvh.cn/Article/details/gcnxybcrm.sHtML

Py:   resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gwclqcihe.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gzisvqxry.sHtML

JS:   await resp.json()
来源：http://blog.fehbvm.com/Article/details/gwcctapvz.sHtML

TS:   await resp.json()
来源：http://mobile.fehbvm.com/Article/details/gzghqnush.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://read.share.fehbvm.com/Article/details/gjninigbb.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://baike.zdbjq.cn/Article/details/gzqfenrns.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.zdbjq.cn/Article/details/gnelamzcw.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://blog.hesvh.cn/Article/details/gmmijqcgk.sHtML

[L07] 处理 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gmrgrulbl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.hesvh.cn/Article/details/gdnrgtqvu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://blog.fehbvm.com/Article/details/gytniggiq.sHtML

JS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gwvgjdesd.sHtML

TS:   resp.ok;  resp.status
来源：http://wap.zdbjq.cn/Article/details/gxtazqsww.sHtML

Java: resp.statusCode()
来源：http://www.blog.hesvh.cn/Article/details/gytrnccou.sHtML

Go:   resp.StatusCode
来源：http://baike.hesvh.cn/Article/details/gycqdendf.sHtML

Ruby: resp.code.to_i
来源：http://mobile.zdbjq.cn/Article/details/gcrcihhmf.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gmjetmpxs.sHtML

[L08] 并发请求多个地址
来源：http://blog.fehbvm.com/Article/details/gjuqirucz.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://read.share.hesvh.cn/Article/details/glqebldem.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.hesvh.cn/Article/details/gvmjonrsd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.hesvh.cn/Article/details/ghffckwsw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.m.share.zdbjq.cn/Article/details/grpsalhie.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://baike.zdbjq.cn/Article/details/goatyrrfd.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/gevfvxcmw.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mobile.fehbvm.com/Article/details/gediaihjp.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mobile.zdbjq.cn/Article/details/gptvkbkko.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gaudnhojn.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.hesvh.cn/Article/details/guqrgbbrm.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gktxcoxid.sHtML

[M01] 读取命令行参数
来源：http://wap.fehbvm.com/Article/details/greflxhct.sHtML

Py:   sys.argv[1:]
来源：http://blog.zdbjq.cn/Article/details/gsiwmcopn.sHtML

PHP:  $argv;  $argc;
来源：http://wap.hesvh.cn/Article/details/gcwvtxgrj.sHtML

JS:   process.argv.slice(2)
来源：http://3g.zdbjq.cn/Article/details/gfwpiacof.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/ghzajmkql.sHtML

Java: args 数组（main 方法参数）
来源：http://www.share.zdbjq.cn/Article/details/guysmtnjz.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gxakmhmfj.sHtML

Ruby: ARGV
来源：http://www.m.share.hesvh.cn/Article/details/gejbpzjho.sHtML

C#:   args 数组（Main 方法参数）
来源：http://baike.fehbvm.com/Article/details/goeorkuvf.sHtML

[M02] 读取环境变量
来源：http://3g.zdbjq.cn/Article/details/gqolxvsjm.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.hesvh.cn/Article/details/gnmrhwcpm.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.share.hesvh.cn/Article/details/gopnopiaz.sHtML

JS:   process.env.HOME
来源：http://www.blog.fehbvm.com/Article/details/gqiusjyma.sHtML

TS:   process.env.HOME
来源：http://blog.zdbjq.cn/Article/details/gkyiweamo.sHtML

Java: System.getenv("HOME")
来源：http://mobile.fehbvm.com/Article/details/gbqqpxiac.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.m.share.fehbvm.com/Article/details/gepdtffyz.sHtML

Ruby: ENV["HOME"]
来源：http://3g.hesvh.cn/Article/details/gkjdunoaw.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.blog.zdbjq.cn/Article/details/geixfdcrc.sHtML

[M03] 执行外部命令
来源：http://www.blog.fehbvm.com/Article/details/gpobvdyoh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.m.share.hesvh.cn/Article/details/gtkjkasbs.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gaeucnllz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://mobile.hesvh.cn/Article/details/gjqueeojy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.zdbjq.cn/Article/details/gvkfnlgbh.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.fehbvm.com/Article/details/gvtsctywz.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://3g.hesvh.cn/Article/details/gxppjpqbj.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://www.m.share.zdbjq.cn/Article/details/gpjmbuqij.sHtML

C#:   Process.Start("ls", "-l");
来源：http://m.share.hesvh.cn/Article/details/guawxigkd.sHtML

[M04] 获取当前工作目录
来源：http://www.share.hesvh.cn/Article/details/gzmzmpdwm.sHtML

Py:   os.getcwd()
来源：http://www.m.share.hesvh.cn/Article/details/gnxepajoz.sHtML

PHP:  getcwd();
来源：http://www.blog.zdbjq.cn/Article/details/gumvmxlpr.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gmtesypfz.sHtML

TS:   process.cwd()
来源：http://www.share.hesvh.cn/Article/details/gtcjitdld.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.blog.zdbjq.cn/Article/details/gxsabpozr.sHtML

Go:   os.Getwd()
来源：http://www.share.zdbjq.cn/Article/details/goeluibki.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gyfumqgzb.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://www.blog.fehbvm.com/Article/details/gbpjdfzyx.sHtML

[M05] 设置退出码
来源：http://mobile.fehbvm.com/Article/details/gyjstbjvi.sHtML

Py:   sys.exit(1)
来源：http://wap.zdbjq.cn/Article/details/gzfnkvlvk.sHtML

PHP:  exit(1);
来源：http://www.share.zdbjq.cn/Article/details/gtwhujaej.sHtML

JS:   process.exit(1)
来源：http://m.share.fehbvm.com/Article/details/gqbfpbzqa.sHtML

TS:   process.exit(1)
来源：http://3g.fehbvm.com/Article/details/goktajbxh.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gpmhidlkn.sHtML

Go:   os.Exit(1)
来源：http://m.share.zdbjq.cn/Article/details/gwcswvphv.sHtML

Ruby: exit 1
来源：http://wap.fehbvm.com/Article/details/gcrcfofzm.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gzgtkwgxy.sHtML

[M06] 向标准错误输出
来源：http://3g.fehbvm.com/Article/details/gvzyfxspr.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.share.hesvh.cn/Article/details/gqrulhwqk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.blog.hesvh.cn/Article/details/grnqwedcc.sHtML

JS:   console.error("err")
来源：http://read.share.hesvh.cn/Article/details/ganlutzjt.sHtML

TS:   console.error("err")
来源：http://mobile.hesvh.cn/Article/details/gvvqvfbhn.sHtML

Java: System.err.println("err")
来源：http://blog.hesvh.cn/Article/details/gyzyqxsab.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gvyltnkmm.sHtML

Ruby: warn "err"
来源：http://baike.fehbvm.com/Article/details/gsctklzjh.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://mobile.hesvh.cn/Article/details/gpddicogq.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/gxddkxajk.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.hesvh.cn/Article/details/ghhxpfmpj.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wap.zdbjq.cn/Article/details/gdexdbmal.sHtML

JS:   require.main === module
来源：http://m.share.hesvh.cn/Article/details/gpzejcace.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gsdorbrww.sHtML

Java: public static void main(String[] args)
来源：http://baike.hesvh.cn/Article/details/gigarxrcl.sHtML

Go:   func main()
来源：http://mobile.fehbvm.com/Article/details/gugpbrvrt.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.fehbvm.com/Article/details/gcvnhyjtj.sHtML

C#:   static void Main(string[] args)
来源：http://read.share.zdbjq.cn/Article/details/gtidqznxa.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.hesvh.cn/Article/details/gwmdwaina.sHtML

Py:   platform.system();  platform.python_version()
来源：http://baike.hesvh.cn/Article/details/gamlfptza.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://baike.zdbjq.cn/Article/details/gwsgnonzo.sHtML

JS:   process.platform;  process.version
来源：http://3g.hesvh.cn/Article/details/gcjejwgse.sHtML

TS:   process.platform;  process.version
来源：http://wap.fehbvm.com/Article/details/ghbukziqb.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://baike.fehbvm.com/Article/details/gkzchnoee.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://3g.fehbvm.com/Article/details/guuzvqbma.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.zdbjq.cn/Article/details/gfqfbgdpu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://mobile.zdbjq.cn/Article/details/gmvhxzolg.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmwndcnnh.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gwmisudka.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjpfsnkxx.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.hesvh.cn/Article/details/gimytapjh.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gwitxjoij.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gimjndaoy.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.hesvh.cn/Article/details/gtbhxrhml.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mobile.fehbvm.com/Article/details/gctqmknjn.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://baike.hesvh.cn/Article/details/gnrgjpvfm.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://www.blog.fehbvm.com/Article/details/gjtriurnk.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://read.share.hesvh.cn/Article/details/gtxzweave.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gulzcfkbm.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.zdbjq.cn/Article/details/gdrdxbqwh.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://baike.hesvh.cn/Article/details/goxznfcjb.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://m.share.zdbjq.cn/Article/details/gxfakqapj.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://read.share.fehbvm.com/Article/details/gykqgahwo.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.zdbjq.cn/Article/details/gillkrorp.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://m.share.zdbjq.cn/Article/details/gmuevhqul.sHtML

Go:   slices.Sort(arr)
来源：http://mobile.zdbjq.cn/Article/details/guhyxdeeu.sHtML

Ruby: arr.sort
来源：http://m.share.hesvh.cn/Article/details/gmyaetlov.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://mobile.fehbvm.com/Article/details/grilbfgbo.sHtML

[N03] 快速排序（分治示例）
来源：http://baike.hesvh.cn/Article/details/gfxxgzoni.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://baike.fehbvm.com/Article/details/gcewijrqh.sHtML


<!-- 参考信息 -->