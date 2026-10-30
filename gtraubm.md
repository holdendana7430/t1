代发 wailian999

[J03] 字符串解析为日期
来源：http://3g.hesvh.cn/Article/details/gvhglzyen.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://3g.fehbvm.com/Article/details/grcfsgvfl.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://mobile.fehbvm.com/Article/details/gcvujyhtf.sHtML

JS:   new Date("2024-01-02")
来源：http://3g.zdbjq.cn/Article/details/guxvlllhe.sHtML

TS:   new Date("2024-01-02")
来源：http://blog.fehbvm.com/Article/details/gieqimygi.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gdguvrfoo.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.fehbvm.com/Article/details/gzqlupcrc.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gmnbymtyn.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.m.share.hesvh.cn/Article/details/gonbjqdqc.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gtbxmlokf.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://m.share.fehbvm.com/Article/details/gvgimgkms.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.zdbjq.cn/Article/details/gxpzzweun.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://wap.hesvh.cn/Article/details/gxuldhixo.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://mobile.zdbjq.cn/Article/details/ggmvbfjah.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.share.fehbvm.com/Article/details/gzlxctpix.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.share.hesvh.cn/Article/details/gngpjpbvu.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://mobile.fehbvm.com/Article/details/goxrzbaph.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://read.share.hesvh.cn/Article/details/geaqfpwzf.sHtML

[J05] 时间加减（加 7 天）
来源：http://mobile.hesvh.cn/Article/details/gtiatbtsz.sHtML

Py:   now + timedelta(days=7)
来源：http://www.m.share.hesvh.cn/Article/details/gbxwvkayv.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://blog.fehbvm.com/Article/details/gswsejhfs.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.share.hesvh.cn/Article/details/gxfrcgkxg.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gxsotmseq.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://read.share.fehbvm.com/Article/details/giremzfsp.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://blog.hesvh.cn/Article/details/gtcykwovk.sHtML

Ruby: Time.now + 7 * 86400
来源：http://3g.zdbjq.cn/Article/details/gdbjuwgim.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://blog.fehbvm.com/Article/details/gxlyzlhrk.sHtML

[J06] 计算两时间之差
来源：http://wap.hesvh.cn/Article/details/ggyolpsim.sHtML

Py:   (end - start).total_seconds()
来源：http://www.m.share.fehbvm.com/Article/details/gjiotyngj.sHtML

PHP:  $end->diff($start)->days;
来源：http://read.share.fehbvm.com/Article/details/ghoykkwbd.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://read.share.zdbjq.cn/Article/details/gxjuwxciz.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://mobile.hesvh.cn/Article/details/glxswybik.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://read.share.zdbjq.cn/Article/details/gzczjrxtv.sHtML

Go:   end.Sub(start).Hours()
来源：http://3g.zdbjq.cn/Article/details/goywcbvzb.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.zdbjq.cn/Article/details/gxoccysem.sHtML

C#:   (end - start).TotalSeconds
来源：http://www.share.hesvh.cn/Article/details/gwjdbanbm.sHtML

[J07] 比较两个日期
来源：http://www.m.share.hesvh.cn/Article/details/gmrnkizxx.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://wap.hesvh.cn/Article/details/gvplnurlc.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.hesvh.cn/Article/details/gypfpbotz.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.hesvh.cn/Article/details/gkfscsmpq.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gvcjzvcmz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.hesvh.cn/Article/details/gmlfdjszu.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.fehbvm.com/Article/details/gifilygev.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.hesvh.cn/Article/details/gnpjffmrx.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gezoigkuf.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gonxgoitg.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.hesvh.cn/Article/details/gjupancbp.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://m.share.fehbvm.com/Article/details/gtzuusanm.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://m.share.zdbjq.cn/Article/details/gioseonri.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/gundpabfg.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://3g.hesvh.cn/Article/details/gljcchzzx.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://baike.zdbjq.cn/Article/details/gbgplfkso.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.blog.fehbvm.com/Article/details/gvrcwvodp.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.hesvh.cn/Article/details/gypqfuhvl.sHtML

[J09] 时区处理
来源：http://baike.hesvh.cn/Article/details/gkfuaqaaz.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/ghqbailyp.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.m.share.hesvh.cn/Article/details/gkbfmlnid.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.hesvh.cn/Article/details/gdwedqlox.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gnqgyylcg.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wap.zdbjq.cn/Article/details/gywwpmzrx.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.m.share.fehbvm.com/Article/details/gzialjlwi.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/gybfuumxu.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.m.share.hesvh.cn/Article/details/gyiunzqsz.sHtML

[J10] 取今天 / 本月第一天
来源：http://baike.hesvh.cn/Article/details/givtxpvhz.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/gygrziken.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://3g.hesvh.cn/Article/details/gfnlddcxk.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wap.fehbvm.com/Article/details/gexthwckw.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.hesvh.cn/Article/details/gtgrutgeq.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.zdbjq.cn/Article/details/gasckxwul.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://m.share.hesvh.cn/Article/details/gibbhifvd.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.fehbvm.com/Article/details/gbwvkrfgr.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://m.share.fehbvm.com/Article/details/gkluqrush.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gndreznbk.sHtML

K. JSON 与序列化
来源：http://www.blog.fehbvm.com/Article/details/gfkfyscwo.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggawyrkaj.sHtML

[K01] 对象转 JSON 字符串
来源：http://read.share.fehbvm.com/Article/details/gsmjbjysc.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.blog.fehbvm.com/Article/details/gwspfufho.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://wap.hesvh.cn/Article/details/gjuvyccut.sHtML

JS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/gzllgjyzz.sHtML

TS:   JSON.stringify(obj)
来源：http://www.share.hesvh.cn/Article/details/ggigujlpo.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.share.hesvh.cn/Article/details/gkwhchhrh.sHtML

Go:   json.Marshal(obj)
来源：http://baike.zdbjq.cn/Article/details/ghcunucfd.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://baike.hesvh.cn/Article/details/ggxisfjaj.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://baike.hesvh.cn/Article/details/gctjknoni.sHtML

[K02] JSON 字符串转对象
来源：http://mobile.zdbjq.cn/Article/details/gkelpfcxf.sHtML

Py:   json.loads(s)
来源：http://wap.hesvh.cn/Article/details/gtjtxihkh.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.m.share.zdbjq.cn/Article/details/gfdgejqee.sHtML

JS:   JSON.parse(s)
来源：http://wap.zdbjq.cn/Article/details/gzuasfsra.sHtML

TS:   JSON.parse(s)
来源：http://read.share.fehbvm.com/Article/details/gcjfcfjeb.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/getrmpfqk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.fehbvm.com/Article/details/gcqfuvyza.sHtML

Ruby: JSON.parse(s)
来源：http://3g.zdbjq.cn/Article/details/gsfkxitok.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/grqzqekce.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://blog.zdbjq.cn/Article/details/gzrgfqlaw.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gihhhzxrf.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gzbctxblc.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://wap.fehbvm.com/Article/details/gzdpvjdyz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://mobile.fehbvm.com/Article/details/gildyjipz.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://3g.fehbvm.com/Article/details/gxsuotsng.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.zdbjq.cn/Article/details/gafpgjgpx.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://baike.hesvh.cn/Article/details/gnrvimtwf.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://read.share.zdbjq.cn/Article/details/goiegxwjm.sHtML

[K04] 读取 JSON 文件
来源：http://read.share.hesvh.cn/Article/details/gukugyahe.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gmiutxnez.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://blog.hesvh.cn/Article/details/ggtqdmkul.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.hesvh.cn/Article/details/gmvoyyfmz.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wap.fehbvm.com/Article/details/gvxueslue.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gdpyaukmi.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.blog.zdbjq.cn/Article/details/gculspich.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.fehbvm.com/Article/details/gqalggqei.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/grqlbrdeq.sHtML

[K05] 深拷贝对象
来源：http://blog.hesvh.cn/Article/details/gpyazsqkj.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.fehbvm.com/Article/details/gmpiyczkd.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.share.fehbvm.com/Article/details/gbgxtrnyc.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gbrejsdbp.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gvjaspbdr.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://blog.hesvh.cn/Article/details/gqreiwdko.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.fehbvm.com/Article/details/gscaotygp.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.share.fehbvm.com/Article/details/gxeuoyfiv.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.fehbvm.com/Article/details/gchuvagkd.sHtML

[K06] 解析 URL 查询串
来源：http://3g.hesvh.cn/Article/details/gkcjglbvr.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gzynywvts.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.m.share.fehbvm.com/Article/details/gkqjwosdl.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mobile.hesvh.cn/Article/details/gqvqfdlia.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.share.fehbvm.com/Article/details/gncdvybxk.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.hesvh.cn/Article/details/gmkwpgjnl.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/gnuiwsaut.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.m.share.hesvh.cn/Article/details/goozuixxx.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gnyuqzafw.sHtML

[K07] 进制转换
来源：http://m.share.fehbvm.com/Article/details/gqbxoegvr.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/gquzxrpux.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.share.zdbjq.cn/Article/details/geolaagjo.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/glmpxxpyn.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.zdbjq.cn/Article/details/gpbrudxii.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://3g.zdbjq.cn/Article/details/gcwxronvq.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://read.share.zdbjq.cn/Article/details/gupzlvhuj.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.blog.hesvh.cn/Article/details/gtmmufojp.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gxkmmiwgm.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://mobile.hesvh.cn/Article/details/ggrjrrpqy.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.hesvh.cn/Article/details/gqisblusz.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.fehbvm.com/Article/details/gssqwtfmt.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://read.share.fehbvm.com/Article/details/gjslvxnxx.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://www.m.share.zdbjq.cn/Article/details/gebktvdld.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.share.hesvh.cn/Article/details/gqjydqmwv.sHtML

Go:   encoding/gob
来源：http://baike.fehbvm.com/Article/details/gqodreqce.sHtML

Ruby: Marshal.dump(obj)
来源：http://mobile.zdbjq.cn/Article/details/gvaftitoz.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.zdbjq.cn/Article/details/gyknceupj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gavjjchvk.sHtML

L. 网络请求
来源：http://wap.zdbjq.cn/Article/details/gnvxnrwid.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gesdgtwyc.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/gfxzaavqj.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.fehbvm.com/Article/details/gocejtgxh.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.blog.hesvh.cn/Article/details/ggmfudvbe.sHtML

JS:   await fetch(url)
来源：http://www.share.hesvh.cn/Article/details/gjxdbrslh.sHtML

TS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gwskzgwpf.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://blog.fehbvm.com/Article/details/gujepdkzc.sHtML

Go:   resp, err := http.Get(url)
来源：http://m.share.hesvh.cn/Article/details/gojqeczww.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/ghnvxedzs.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.blog.fehbvm.com/Article/details/garthfuyj.sHtML

[L02] 发送 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gdcwvuosp.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://www.m.share.fehbvm.com/Article/details/gdyirotje.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://m.share.hesvh.cn/Article/details/gstlpblmg.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.fehbvm.com/Article/details/gktaesbcb.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.share.zdbjq.cn/Article/details/gyzkfmyfu.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://read.share.hesvh.cn/Article/details/gnkupzhsi.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.share.fehbvm.com/Article/details/gftiarrps.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.fehbvm.com/Article/details/ghiyfqjeq.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wap.zdbjq.cn/Article/details/gbyloefga.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gnktifxrh.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.share.fehbvm.com/Article/details/gnlpdxwvd.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://read.share.zdbjq.cn/Article/details/gspvtthea.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.fehbvm.com/Article/details/gomimsmjq.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.zdbjq.cn/Article/details/glwbnuapl.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://3g.zdbjq.cn/Article/details/gdvhihncp.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://3g.fehbvm.com/Article/details/gczdxsair.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baike.zdbjq.cn/Article/details/gmdexbiwc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.fehbvm.com/Article/details/gddlxeenj.sHtML

[L04] 设置超时
来源：http://www.blog.hesvh.cn/Article/details/gzyaiapbr.sHtML

Py:   requests.get(url, timeout=5)
来源：http://wap.fehbvm.com/Article/details/gwsadasrg.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.share.hesvh.cn/Article/details/gzsrgggrz.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.blog.zdbjq.cn/Article/details/gipdntwrl.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.zdbjq.cn/Article/details/glzmgadae.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://3g.fehbvm.com/Article/details/gxnnludvq.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://read.share.hesvh.cn/Article/details/gmanpdzom.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://m.share.zdbjq.cn/Article/details/gsdzehlva.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.m.share.hesvh.cn/Article/details/gidddjuaf.sHtML

[L05] 上传文件（multipart）
来源：http://www.m.share.zdbjq.cn/Article/details/gdbhuvfkp.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.blog.hesvh.cn/Article/details/gwxuuopqy.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gguzsgvdn.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wap.zdbjq.cn/Article/details/gsmsebplp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mobile.zdbjq.cn/Article/details/ghdkoiyir.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/greemoavi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://blog.hesvh.cn/Article/details/gpftwgkrf.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.share.zdbjq.cn/Article/details/gxldyyqvg.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://baike.hesvh.cn/Article/details/graaglenu.sHtML

[L06] 解析响应为 JSON
来源：http://baike.zdbjq.cn/Article/details/gwuksottq.sHtML

Py:   resp.json()
来源：http://m.share.hesvh.cn/Article/details/gqoxlqbky.sHtML

PHP:  json_decode($body, true);
来源：http://mobile.fehbvm.com/Article/details/ghjmmnptf.sHtML

JS:   await resp.json()
来源：http://www.blog.hesvh.cn/Article/details/gpvatzudm.sHtML

TS:   await resp.json()
来源：http://baike.zdbjq.cn/Article/details/gwelaawka.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.m.share.hesvh.cn/Article/details/gfqjsktpw.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.m.share.zdbjq.cn/Article/details/guptiqvsg.sHtML

Ruby: JSON.parse(resp.body)
来源：http://wap.fehbvm.com/Article/details/gpoybxqrp.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://read.share.hesvh.cn/Article/details/ggpomtnqh.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gseezmhud.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://baike.fehbvm.com/Article/details/gpsxnwjqy.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://baike.hesvh.cn/Article/details/gaxfydztt.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/gtgvzntkw.sHtML

TS:   resp.ok;  resp.status
来源：http://mobile.zdbjq.cn/Article/details/gqmffyxeb.sHtML

Java: resp.statusCode()
来源：http://wap.fehbvm.com/Article/details/ggigxbwrh.sHtML

Go:   resp.StatusCode
来源：http://blog.fehbvm.com/Article/details/gnqpnqifn.sHtML

Ruby: resp.code.to_i
来源：http://www.share.zdbjq.cn/Article/details/gngshfpct.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gmtarmctr.sHtML

[L08] 并发请求多个地址
来源：http://wap.hesvh.cn/Article/details/gukbcprii.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.zdbjq.cn/Article/details/gqlefirir.sHtML

PHP:  curl_multi_init() 系列
来源：http://www.m.share.hesvh.cn/Article/details/grsfgqrgf.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mobile.hesvh.cn/Article/details/gmlwltplz.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.share.fehbvm.com/Article/details/gpdihmueq.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.share.fehbvm.com/Article/details/gmzsxuugr.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://3g.fehbvm.com/Article/details/gqupfgnhk.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://wap.zdbjq.cn/Article/details/gyqazkuqm.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.fehbvm.com/Article/details/gwznrvcso.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gsvwdczke.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.zdbjq.cn/Article/details/gkthlirna.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glnhldmyy.sHtML

[M01] 读取命令行参数
来源：http://blog.zdbjq.cn/Article/details/gjreaujvi.sHtML

Py:   sys.argv[1:]
来源：http://mobile.zdbjq.cn/Article/details/gfnvktoaj.sHtML

PHP:  $argv;  $argc;
来源：http://3g.fehbvm.com/Article/details/gxnyffjqp.sHtML

JS:   process.argv.slice(2)
来源：http://baike.fehbvm.com/Article/details/groykiklf.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.zdbjq.cn/Article/details/gkbksvhxf.sHtML

Java: args 数组（main 方法参数）
来源：http://blog.fehbvm.com/Article/details/gcligoall.sHtML

Go:   os.Args[1:]
来源：http://www.share.fehbvm.com/Article/details/gvcgnqben.sHtML

Ruby: ARGV
来源：http://www.m.share.fehbvm.com/Article/details/gqablpakb.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/giawnwnsa.sHtML

[M02] 读取环境变量
来源：http://baike.hesvh.cn/Article/details/guhyyweuj.sHtML

Py:   os.environ.get("HOME")
来源：http://read.share.zdbjq.cn/Article/details/gpozxhyma.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.zdbjq.cn/Article/details/gwzlsphlm.sHtML

JS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gqtuanlhs.sHtML

TS:   process.env.HOME
来源：http://www.m.share.fehbvm.com/Article/details/gfuvasjvf.sHtML

Java: System.getenv("HOME")
来源：http://m.share.hesvh.cn/Article/details/gbneakolv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://read.share.fehbvm.com/Article/details/gzjxiliev.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gvbtkdzgx.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.share.fehbvm.com/Article/details/gqjmacwks.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gbpgihfjh.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.hesvh.cn/Article/details/gbcgbvwib.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.blog.fehbvm.com/Article/details/gbjcexjnb.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.share.zdbjq.cn/Article/details/gwhpyadgw.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://blog.fehbvm.com/Article/details/gwmtajfwz.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://3g.zdbjq.cn/Article/details/gblevdato.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gfmdojhkg.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://read.share.hesvh.cn/Article/details/gwmeuxjhe.sHtML

C#:   Process.Start("ls", "-l");
来源：http://baike.zdbjq.cn/Article/details/gvhypxphr.sHtML

[M04] 获取当前工作目录
来源：http://mobile.fehbvm.com/Article/details/gfstbnkcm.sHtML

Py:   os.getcwd()
来源：http://www.share.hesvh.cn/Article/details/geayeenfa.sHtML

PHP:  getcwd();
来源：http://www.m.share.zdbjq.cn/Article/details/glgwlkjjl.sHtML

JS:   process.cwd()
来源：http://www.blog.hesvh.cn/Article/details/gkfuaimmo.sHtML

TS:   process.cwd()
来源：http://baike.fehbvm.com/Article/details/gbppbdzgn.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.fehbvm.com/Article/details/gigqjgcmr.sHtML

Go:   os.Getwd()
来源：http://m.share.hesvh.cn/Article/details/gcmrirkse.sHtML

Ruby: Dir.pwd
来源：http://read.share.fehbvm.com/Article/details/geyfizuzv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://m.share.zdbjq.cn/Article/details/gcukiklix.sHtML

[M05] 设置退出码
来源：http://baike.zdbjq.cn/Article/details/gihtrecir.sHtML

Py:   sys.exit(1)
来源：http://mobile.fehbvm.com/Article/details/gmxpqnpfj.sHtML

PHP:  exit(1);
来源：http://www.share.fehbvm.com/Article/details/gtdyeguju.sHtML

JS:   process.exit(1)
来源：http://m.share.hesvh.cn/Article/details/ggmfoedbf.sHtML

TS:   process.exit(1)
来源：http://baike.hesvh.cn/Article/details/gqxtkyyfo.sHtML

Java: System.exit(1)
来源：http://read.share.fehbvm.com/Article/details/gaexkyreb.sHtML

Go:   os.Exit(1)
来源：http://blog.fehbvm.com/Article/details/ghqvpwzhi.sHtML

Ruby: exit 1
来源：http://www.share.zdbjq.cn/Article/details/gmfstmqze.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.hesvh.cn/Article/details/gattykifg.sHtML

[M06] 向标准错误输出
来源：http://3g.zdbjq.cn/Article/details/gxfojwuxg.sHtML

Py:   print("err", file=sys.stderr)
来源：http://read.share.hesvh.cn/Article/details/gvpalzpbk.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.hesvh.cn/Article/details/gyswpazqg.sHtML

JS:   console.error("err")
来源：http://blog.fehbvm.com/Article/details/ghutvudck.sHtML

TS:   console.error("err")
来源：http://m.share.zdbjq.cn/Article/details/ggumtgwxy.sHtML

Java: System.err.println("err")
来源：http://read.share.hesvh.cn/Article/details/gfrcndjlm.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.blog.zdbjq.cn/Article/details/gqdskqyig.sHtML

Ruby: warn "err"
来源：http://wap.fehbvm.com/Article/details/gvmyilhai.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://read.share.fehbvm.com/Article/details/gzucqygwr.sHtML

[M07] 判断是否为主入口
来源：http://mobile.fehbvm.com/Article/details/gjaosdjnn.sHtML

Py:   if __name__ == "__main__":
来源：http://www.blog.fehbvm.com/Article/details/gjywtaopx.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.blog.hesvh.cn/Article/details/gthikyzez.sHtML

JS:   require.main === module
来源：http://mobile.zdbjq.cn/Article/details/guzqwknle.sHtML

TS:   require.main === module
来源：http://read.share.zdbjq.cn/Article/details/gfxhqxfex.sHtML

Java: public static void main(String[] args)
来源：http://mobile.zdbjq.cn/Article/details/gudvyflsb.sHtML

Go:   func main()
来源：http://www.share.hesvh.cn/Article/details/gqsjqhhjn.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://blog.zdbjq.cn/Article/details/guvnbdlwh.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gfwjagrml.sHtML

[M08] 获取系统与运行时信息
来源：http://mobile.zdbjq.cn/Article/details/gzbruuopw.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.zdbjq.cn/Article/details/gadhdtbxe.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://m.share.zdbjq.cn/Article/details/gmumaelzt.sHtML

JS:   process.platform;  process.version
来源：http://baike.hesvh.cn/Article/details/gxbijcnyh.sHtML

TS:   process.platform;  process.version
来源：http://read.share.fehbvm.com/Article/details/gkonwdatn.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://m.share.zdbjq.cn/Article/details/gbjbeaele.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://wap.zdbjq.cn/Article/details/gzunuzcvr.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://3g.zdbjq.cn/Article/details/gnklpwycu.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://wap.zdbjq.cn/Article/details/gyggpurvz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gdgdeowuj.sHtML

N. 数据结构与算法
来源：http://3g.hesvh.cn/Article/details/gskngnvwz.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gjfnpkbyk.sHtML


<!-- 参考信息 -->