代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://baike.zdbjq.cn/Article/details/genoxxihe.sHtML

[J04] 时间戳与日期互转
来源：http://www.share.zdbjq.cn/Article/details/gnpkjwgqn.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.hesvh.cn/Article/details/gunyjbwqd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.blog.hesvh.cn/Article/details/gewyofwts.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gamytypkp.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://read.share.hesvh.cn/Article/details/ghfulajoi.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gbsibsxmt.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://read.share.fehbvm.com/Article/details/gskodvnmt.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://wap.hesvh.cn/Article/details/gxllkxqsl.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://3g.hesvh.cn/Article/details/gwzzftwkd.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.zdbjq.cn/Article/details/ghwchuuku.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.zdbjq.cn/Article/details/gqvvyrxfj.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gbirrnqxv.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://baike.hesvh.cn/Article/details/gvpirmlcz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://read.share.zdbjq.cn/Article/details/ggizyulng.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://3g.hesvh.cn/Article/details/gxklzidsb.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://mobile.hesvh.cn/Article/details/gjyclnjsb.sHtML

Ruby: Time.now + 7 * 86400
来源：http://read.share.hesvh.cn/Article/details/gnpzhjvhq.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://3g.hesvh.cn/Article/details/gupzytulo.sHtML

[J06] 计算两时间之差
来源：http://read.share.zdbjq.cn/Article/details/gwfojbtyk.sHtML

Py:   (end - start).total_seconds()
来源：http://wap.hesvh.cn/Article/details/glnqejyia.sHtML

PHP:  $end->diff($start)->days;
来源：http://blog.zdbjq.cn/Article/details/gctyqydel.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.m.share.zdbjq.cn/Article/details/gyitjygqg.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gpgvvsdjh.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.fehbvm.com/Article/details/gjhqypiha.sHtML

Go:   end.Sub(start).Hours()
来源：http://www.m.share.zdbjq.cn/Article/details/gjxhriqxd.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.hesvh.cn/Article/details/gknjjyfum.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.m.share.fehbvm.com/Article/details/gukgghufl.sHtML

[J07] 比较两个日期
来源：http://baike.zdbjq.cn/Article/details/gdvdngcmb.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.zdbjq.cn/Article/details/gwdovwruc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://mobile.hesvh.cn/Article/details/gedmlkuiw.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.zdbjq.cn/Article/details/ghlqeakja.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://blog.fehbvm.com/Article/details/goysmsaev.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mobile.fehbvm.com/Article/details/gdxhotbuq.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.hesvh.cn/Article/details/gwralnvik.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gkwbrwxmn.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gnegokmkm.sHtML

[J08] 提取年月日与星期
来源：http://wap.zdbjq.cn/Article/details/gfqrdldmb.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://baike.hesvh.cn/Article/details/ggzgcuhti.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.m.share.fehbvm.com/Article/details/gmsoucrer.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://baike.hesvh.cn/Article/details/gjlevnwsc.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.hesvh.cn/Article/details/greinogbs.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://baike.zdbjq.cn/Article/details/gmlaayhql.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://read.share.zdbjq.cn/Article/details/ghaxowquh.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://baike.hesvh.cn/Article/details/gneghvdap.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://baike.zdbjq.cn/Article/details/gqhzqhxhs.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gzbbwzptm.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://m.share.zdbjq.cn/Article/details/grnchwkwp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/gexivxgab.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wap.fehbvm.com/Article/details/gzsbdtdyu.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gqdjooeap.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.m.share.zdbjq.cn/Article/details/gknstkfhd.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://read.share.zdbjq.cn/Article/details/gvpzieluf.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://read.share.zdbjq.cn/Article/details/gyysfyjrv.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/ghtfmdkol.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.hesvh.cn/Article/details/gwummyisa.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://www.blog.zdbjq.cn/Article/details/gztarzzzm.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.blog.fehbvm.com/Article/details/gexgqpyoy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://mobile.hesvh.cn/Article/details/grmyroiwd.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gszsufhqa.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.blog.hesvh.cn/Article/details/gqgawxfue.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://baike.zdbjq.cn/Article/details/gzkilrbkt.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://blog.fehbvm.com/Article/details/gwzwluhgl.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wap.fehbvm.com/Article/details/glggqwuhx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbjbeztpe.sHtML

K. JSON 与序列化
来源：http://www.share.fehbvm.com/Article/details/gtnbllxrp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwexypuog.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.blog.hesvh.cn/Article/details/ghmfmzdnw.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mobile.fehbvm.com/Article/details/grdsulird.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gztzjkkrr.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gchcfgjjf.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.hesvh.cn/Article/details/ggnhczhsv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.m.share.hesvh.cn/Article/details/gfyxxjutg.sHtML

Go:   json.Marshal(obj)
来源：http://blog.hesvh.cn/Article/details/gwbbnczbx.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://www.share.zdbjq.cn/Article/details/gzvsjmvxi.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://blog.fehbvm.com/Article/details/goyrnuaus.sHtML

[K02] JSON 字符串转对象
来源：http://www.blog.fehbvm.com/Article/details/garspgbpn.sHtML

Py:   json.loads(s)
来源：http://m.share.hesvh.cn/Article/details/gtiaxnwzt.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.hesvh.cn/Article/details/giychqljv.sHtML

JS:   JSON.parse(s)
来源：http://mobile.hesvh.cn/Article/details/gugapaofz.sHtML

TS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gcfmrtqxe.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.blog.fehbvm.com/Article/details/gmsngyqoq.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://read.share.fehbvm.com/Article/details/gcczourlb.sHtML

Ruby: JSON.parse(s)
来源：http://3g.hesvh.cn/Article/details/givrxpyky.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.blog.zdbjq.cn/Article/details/gjxvuthls.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://baike.hesvh.cn/Article/details/gnbrfzexp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mobile.hesvh.cn/Article/details/gdlpykrwo.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://m.share.zdbjq.cn/Article/details/gokoxcyqf.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://blog.zdbjq.cn/Article/details/ggwdrwyjp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.share.hesvh.cn/Article/details/gbvvggvbh.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.zdbjq.cn/Article/details/gstzxgbfl.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gbczzmihp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://wap.fehbvm.com/Article/details/gayuatyeu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.hesvh.cn/Article/details/gpouiqkjm.sHtML

[K04] 读取 JSON 文件
来源：http://blog.hesvh.cn/Article/details/gmwjtkuvx.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.hesvh.cn/Article/details/gcjvbshrk.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/ghcicrtud.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.hesvh.cn/Article/details/gnyrhibvb.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.blog.fehbvm.com/Article/details/gfocyudxd.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gpbrpwjgp.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gcvmcrucc.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gzgmviivp.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.fehbvm.com/Article/details/ghybdznvw.sHtML

[K05] 深拷贝对象
来源：http://www.share.hesvh.cn/Article/details/gefnralqj.sHtML

Py:   copy.deepcopy(obj)
来源：http://blog.fehbvm.com/Article/details/glnltikrt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://m.share.fehbvm.com/Article/details/gqhlwixto.sHtML

JS:   structuredClone(obj)
来源：http://www.share.zdbjq.cn/Article/details/ghysrfern.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gpsltoene.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.m.share.hesvh.cn/Article/details/gsabjltfc.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.blog.fehbvm.com/Article/details/gpswtocwz.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gtnykcrkd.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gtcbksjtb.sHtML

[K06] 解析 URL 查询串
来源：http://wap.zdbjq.cn/Article/details/gsmtjjufd.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wap.hesvh.cn/Article/details/gjzcghsxe.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.share.fehbvm.com/Article/details/gfyctcdsv.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://3g.fehbvm.com/Article/details/gpvrwyqzo.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gfpslaiae.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://baike.hesvh.cn/Article/details/gmikzrsiq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gxhzzynmi.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gnsatczay.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://blog.zdbjq.cn/Article/details/geumqtdhk.sHtML

[K07] 进制转换
来源：http://baike.hesvh.cn/Article/details/gewzgpduo.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gmldmerqz.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://blog.fehbvm.com/Article/details/goucxmqjo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://blog.zdbjq.cn/Article/details/gynqydvjs.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://3g.hesvh.cn/Article/details/geqeuziag.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gavsnngrw.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wap.fehbvm.com/Article/details/gpwdrtfre.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://read.share.fehbvm.com/Article/details/gbvyawbsw.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gihrnewvj.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://read.share.fehbvm.com/Article/details/gjhpellpm.sHtML

Py:   pickle.dumps(obj)
来源：http://wap.zdbjq.cn/Article/details/gdvhufqqj.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.zdbjq.cn/Article/details/gajcqyiyn.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gxvxwrahv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.hesvh.cn/Article/details/gmhqzcfja.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.m.share.fehbvm.com/Article/details/grnddyvzr.sHtML

Go:   encoding/gob
来源：http://wap.zdbjq.cn/Article/details/gmzfytkuo.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.fehbvm.com/Article/details/gwpooyntj.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://m.share.zdbjq.cn/Article/details/giezxtost.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcaeexsgh.sHtML

L. 网络请求
来源：http://wap.hesvh.cn/Article/details/gigptsxtd.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/giwuiahwi.sHtML

[L01] 发送 GET 请求
来源：http://baike.fehbvm.com/Article/details/gdyovchhf.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.fehbvm.com/Article/details/gqtphignp.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.m.share.zdbjq.cn/Article/details/gwqhxhpnr.sHtML

JS:   await fetch(url)
来源：http://read.share.hesvh.cn/Article/details/gldyaoyil.sHtML

TS:   await fetch(url)
来源：http://m.share.fehbvm.com/Article/details/gsmchugkx.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.fehbvm.com/Article/details/gomvfajze.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gretzsvit.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.share.fehbvm.com/Article/details/gkflqynrb.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wap.hesvh.cn/Article/details/gifzyjpgt.sHtML

[L02] 发送 POST JSON
来源：http://read.share.zdbjq.cn/Article/details/gxjibzamy.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://mobile.fehbvm.com/Article/details/gzaascikp.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.m.share.fehbvm.com/Article/details/giykfukkd.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.blog.hesvh.cn/Article/details/giremrgqu.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.fehbvm.com/Article/details/gnehtfqeo.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://3g.fehbvm.com/Article/details/ghkfnolwl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://read.share.hesvh.cn/Article/details/gdfvniwld.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.hesvh.cn/Article/details/gfkdbsqey.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.m.share.hesvh.cn/Article/details/gldnmmkfg.sHtML

[L03] 设置自定义请求头
来源：http://www.blog.fehbvm.com/Article/details/gupfprjmv.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/guqpuabfq.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/ghowgjpjm.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.fehbvm.com/Article/details/ggomyiwhr.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.blog.fehbvm.com/Article/details/globajdji.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.fehbvm.com/Article/details/gkhckswte.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.zdbjq.cn/Article/details/gdghclttk.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mobile.hesvh.cn/Article/details/gdawufxsg.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gykvzhvji.sHtML

[L04] 设置超时
来源：http://blog.hesvh.cn/Article/details/gtohkegfx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.hesvh.cn/Article/details/giktsasqt.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/grqvhuhol.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gqevjbezk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://baike.zdbjq.cn/Article/details/gkizdjkeo.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://baike.fehbvm.com/Article/details/gbkiocwja.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.share.hesvh.cn/Article/details/gqknsxsac.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gioeymwud.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.blog.zdbjq.cn/Article/details/gdyxfydyj.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/guerrouxi.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gmkesqppm.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wap.fehbvm.com/Article/details/gokywsinr.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.hesvh.cn/Article/details/glcgkwogb.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://read.share.zdbjq.cn/Article/details/grksvblco.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://blog.zdbjq.cn/Article/details/gtqkjxbdi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://read.share.fehbvm.com/Article/details/gaapqofti.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://blog.hesvh.cn/Article/details/gfcvozopy.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.fehbvm.com/Article/details/gerkwnamx.sHtML

[L06] 解析响应为 JSON
来源：http://wap.zdbjq.cn/Article/details/gaxkhiptm.sHtML

Py:   resp.json()
来源：http://mobile.zdbjq.cn/Article/details/gslsedfzb.sHtML

PHP:  json_decode($body, true);
来源：http://m.share.hesvh.cn/Article/details/ghvtbohgw.sHtML

JS:   await resp.json()
来源：http://www.m.share.zdbjq.cn/Article/details/gwefuvcjj.sHtML

TS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gwfwwgxvx.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.fehbvm.com/Article/details/gxbonfvbp.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://3g.hesvh.cn/Article/details/gqedhyoyf.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gdmwjickg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.zdbjq.cn/Article/details/gzfyezsik.sHtML

[L07] 处理 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gbnkmcxkk.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.hesvh.cn/Article/details/gviejllev.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://wap.fehbvm.com/Article/details/gzxdxppdj.sHtML

JS:   resp.ok;  resp.status
来源：http://www.share.hesvh.cn/Article/details/gyaysbyml.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.zdbjq.cn/Article/details/gqnwdkrxy.sHtML

Java: resp.statusCode()
来源：http://wap.zdbjq.cn/Article/details/gbvfmadgc.sHtML

Go:   resp.StatusCode
来源：http://www.blog.zdbjq.cn/Article/details/gsbwznveu.sHtML

Ruby: resp.code.to_i
来源：http://3g.fehbvm.com/Article/details/gdrmynltn.sHtML

C#:   (int)resp.StatusCode
来源：http://m.share.fehbvm.com/Article/details/grpslxwht.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gsizxioxu.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.fehbvm.com/Article/details/grsparbml.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/gjkizwwhl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://m.share.zdbjq.cn/Article/details/ggurwceaw.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gnndyxwxc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://read.share.fehbvm.com/Article/details/gngdvwzqk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.share.hesvh.cn/Article/details/gqbbsnjnr.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://3g.zdbjq.cn/Article/details/gatgftjss.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://baike.zdbjq.cn/Article/details/gtfljgalu.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grzwfmdtz.sHtML

M. 命令行 / 进程 / 环境
来源：http://3g.hesvh.cn/Article/details/gtgdvafbg.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/goqdsbayi.sHtML

[M01] 读取命令行参数
来源：http://www.share.hesvh.cn/Article/details/glnpocjvd.sHtML

Py:   sys.argv[1:]
来源：http://3g.hesvh.cn/Article/details/gxbwxkxua.sHtML

PHP:  $argv;  $argc;
来源：http://blog.zdbjq.cn/Article/details/gjjftnsre.sHtML

JS:   process.argv.slice(2)
来源：http://read.share.hesvh.cn/Article/details/gnikinmcd.sHtML

TS:   process.argv.slice(2)
来源：http://www.share.zdbjq.cn/Article/details/gxawikwmo.sHtML

Java: args 数组（main 方法参数）
来源：http://m.share.hesvh.cn/Article/details/ginwigqft.sHtML

Go:   os.Args[1:]
来源：http://baike.fehbvm.com/Article/details/grsewddut.sHtML

Ruby: ARGV
来源：http://mobile.fehbvm.com/Article/details/gzcnvavfi.sHtML

C#:   args 数组（Main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gzglulsel.sHtML

[M02] 读取环境变量
来源：http://baike.fehbvm.com/Article/details/gxoxdtqto.sHtML

Py:   os.environ.get("HOME")
来源：http://baike.zdbjq.cn/Article/details/gdarqpgfb.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.zdbjq.cn/Article/details/granhngzg.sHtML

JS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/gkysblgyn.sHtML

TS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gabqlvvik.sHtML

Java: System.getenv("HOME")
来源：http://wap.zdbjq.cn/Article/details/guqwcrdei.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.fehbvm.com/Article/details/gvjysimao.sHtML

Ruby: ENV["HOME"]
来源：http://wap.fehbvm.com/Article/details/gdhwlyeul.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.zdbjq.cn/Article/details/gqhiaxqmx.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gafoprnib.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.hesvh.cn/Article/details/gpwwghbev.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.share.zdbjq.cn/Article/details/gyfdyavmr.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://blog.zdbjq.cn/Article/details/guntmpjbe.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://wap.fehbvm.com/Article/details/gealdlssr.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wap.zdbjq.cn/Article/details/gnemrekox.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.m.share.fehbvm.com/Article/details/gmihubise.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.hesvh.cn/Article/details/grlqcezve.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gvpjfesoj.sHtML

[M04] 获取当前工作目录
来源：http://www.m.share.hesvh.cn/Article/details/gmmufjyaj.sHtML

Py:   os.getcwd()
来源：http://wap.hesvh.cn/Article/details/gcybqolwv.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gbtcmeite.sHtML

JS:   process.cwd()
来源：http://blog.hesvh.cn/Article/details/gngnqbiow.sHtML

TS:   process.cwd()
来源：http://www.blog.zdbjq.cn/Article/details/gfdziyjpy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://mobile.fehbvm.com/Article/details/grrsncwnr.sHtML

Go:   os.Getwd()
来源：http://blog.zdbjq.cn/Article/details/gtnzwgkyu.sHtML

Ruby: Dir.pwd
来源：http://baike.zdbjq.cn/Article/details/gwjwnmrff.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://3g.zdbjq.cn/Article/details/gbijcaorm.sHtML

[M05] 设置退出码
来源：http://3g.zdbjq.cn/Article/details/gdpgypryy.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gyktzkmhx.sHtML

PHP:  exit(1);
来源：http://read.share.fehbvm.com/Article/details/gnwxcoczk.sHtML

JS:   process.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gzfwsyvli.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gqhgbtfrj.sHtML

Java: System.exit(1)
来源：http://www.share.fehbvm.com/Article/details/geqdzhllv.sHtML

Go:   os.Exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/glcniecqx.sHtML

Ruby: exit 1
来源：http://www.m.share.zdbjq.cn/Article/details/gyjuwxbwj.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.blog.fehbvm.com/Article/details/gvhgqnkrx.sHtML

[M06] 向标准错误输出
来源：http://www.blog.fehbvm.com/Article/details/gqpyntmef.sHtML

Py:   print("err", file=sys.stderr)
来源：http://mobile.zdbjq.cn/Article/details/ggsxhlotj.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.zdbjq.cn/Article/details/gwwmhjavm.sHtML

JS:   console.error("err")
来源：http://www.blog.zdbjq.cn/Article/details/gqvjlmyno.sHtML

TS:   console.error("err")
来源：http://www.m.share.hesvh.cn/Article/details/gmzoytrwq.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/grkoqkjqu.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.zdbjq.cn/Article/details/gesfeurpl.sHtML

Ruby: warn "err"
来源：http://3g.zdbjq.cn/Article/details/glxxpszeo.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://m.share.fehbvm.com/Article/details/gyjpbzssb.sHtML

[M07] 判断是否为主入口
来源：http://www.m.share.hesvh.cn/Article/details/gpbdwrfeh.sHtML

Py:   if __name__ == "__main__":
来源：http://baike.hesvh.cn/Article/details/gziaefmft.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.share.hesvh.cn/Article/details/gshnbecjb.sHtML

JS:   require.main === module
来源：http://mobile.fehbvm.com/Article/details/ghtdtifgr.sHtML

TS:   require.main === module
来源：http://wap.zdbjq.cn/Article/details/gcocmycxq.sHtML

Java: public static void main(String[] args)
来源：http://3g.zdbjq.cn/Article/details/gjnzwxxep.sHtML

Go:   func main()
来源：http://mobile.zdbjq.cn/Article/details/gxtjsigem.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wap.zdbjq.cn/Article/details/gsosyrnfi.sHtML

C#:   static void Main(string[] args)
来源：http://baike.hesvh.cn/Article/details/gaftoovgj.sHtML

[M08] 获取系统与运行时信息
来源：http://baike.fehbvm.com/Article/details/glpnmtnhz.sHtML

Py:   platform.system();  platform.python_version()
来源：http://read.share.hesvh.cn/Article/details/gwkyyobtf.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.share.fehbvm.com/Article/details/gehyyswny.sHtML

JS:   process.platform;  process.version
来源：http://blog.fehbvm.com/Article/details/gpxeefehd.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/glwubpahf.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/gdlclrbwh.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.zdbjq.cn/Article/details/gzovqetwk.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.m.share.zdbjq.cn/Article/details/gfmojfxgt.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.fehbvm.com/Article/details/ganuyrbhl.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gbzswjelc.sHtML

N. 数据结构与算法
来源：http://baike.zdbjq.cn/Article/details/gttgwjhhh.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/garjzqpzg.sHtML

[N01] 二分查找（有序数组）
来源：http://baike.zdbjq.cn/Article/details/gxzgrwjix.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://3g.fehbvm.com/Article/details/gnxkpdolb.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://read.share.zdbjq.cn/Article/details/gqievalzs.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.zdbjq.cn/Article/details/gepssjlfe.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wap.zdbjq.cn/Article/details/gyevsppes.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://wap.hesvh.cn/Article/details/gnbbsvlpl.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/glkxtihnw.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.share.fehbvm.com/Article/details/gkuhpmslq.sHtML


<!-- 参考信息 -->