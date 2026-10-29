代发 wailian999

[J03] 字符串解析为日期
来源：http://www.m.share.zdbjq.cn/Article/details/gxlkzggkr.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.share.hesvh.cn/Article/details/gdmrroatu.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://baike.fehbvm.com/Article/details/gboqdlmlh.sHtML

JS:   new Date("2024-01-02")
来源：http://blog.hesvh.cn/Article/details/gsjwsfibo.sHtML

TS:   new Date("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/grcdjfiqb.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://3g.hesvh.cn/Article/details/gfvfkaakd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gbdadbfmb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://www.blog.hesvh.cn/Article/details/gesvimqvz.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://blog.zdbjq.cn/Article/details/gswyhgqix.sHtML

[J04] 时间戳与日期互转
来源：http://3g.zdbjq.cn/Article/details/gbgloaccl.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.m.share.fehbvm.com/Article/details/gycfdmntd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://wap.fehbvm.com/Article/details/gjpkzgjye.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://m.share.zdbjq.cn/Article/details/gtknwypsy.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.blog.fehbvm.com/Article/details/gstbjhyuy.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://read.share.zdbjq.cn/Article/details/gkgvsgekw.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.blog.fehbvm.com/Article/details/gdboajcyb.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://read.share.fehbvm.com/Article/details/gcmehpauz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.blog.hesvh.cn/Article/details/gyqjolfmk.sHtML

[J05] 时间加减（加 7 天）
来源：http://baike.fehbvm.com/Article/details/gaezpjffe.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.hesvh.cn/Article/details/gybmczash.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.zdbjq.cn/Article/details/gwqpavjjz.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.zdbjq.cn/Article/details/gwcfdjqhf.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.m.share.zdbjq.cn/Article/details/ganswgurk.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.hesvh.cn/Article/details/gaqjgxtcv.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.hesvh.cn/Article/details/gxzrvzffu.sHtML

Ruby: Time.now + 7 * 86400
来源：http://baike.hesvh.cn/Article/details/gewcisesb.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.m.share.fehbvm.com/Article/details/gtkibsnyu.sHtML

[J06] 计算两时间之差
来源：http://m.share.hesvh.cn/Article/details/gplfodyol.sHtML

Py:   (end - start).total_seconds()
来源：http://mobile.fehbvm.com/Article/details/gzjebnilg.sHtML

PHP:  $end->diff($start)->days;
来源：http://www.blog.zdbjq.cn/Article/details/gbtuumjzm.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.blog.fehbvm.com/Article/details/gthrxfskx.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://blog.hesvh.cn/Article/details/gnnjqiihm.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://mobile.zdbjq.cn/Article/details/gehbhjsxs.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gvooifyta.sHtML

Ruby: end - start                 # 返回秒数
来源：http://www.m.share.fehbvm.com/Article/details/gtboekcqe.sHtML

C#:   (end - start).TotalSeconds
来源：http://baike.hesvh.cn/Article/details/gdejspcbi.sHtML

[J07] 比较两个日期
来源：http://blog.zdbjq.cn/Article/details/gurqvfrwa.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://www.share.hesvh.cn/Article/details/gdxpdmnxv.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://3g.zdbjq.cn/Article/details/gvsqkrmpy.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://m.share.fehbvm.com/Article/details/gqzwhyxiy.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://wap.fehbvm.com/Article/details/grxgunrqz.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://baike.fehbvm.com/Article/details/gdyxugkas.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://mobile.fehbvm.com/Article/details/gmnwcxawf.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/ggxtuupqo.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.blog.zdbjq.cn/Article/details/gprbucykx.sHtML

[J08] 提取年月日与星期
来源：http://mobile.zdbjq.cn/Article/details/gotgbniac.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://blog.fehbvm.com/Article/details/gqiiysbbb.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mobile.fehbvm.com/Article/details/gccuuwbsu.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gbrikgfde.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://read.share.hesvh.cn/Article/details/gccfucqxl.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/ghsyogluo.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://blog.fehbvm.com/Article/details/gygaythlw.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://blog.zdbjq.cn/Article/details/ggoohrnrn.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.m.share.zdbjq.cn/Article/details/gddbhozkx.sHtML

[J09] 时区处理
来源：http://blog.hesvh.cn/Article/details/gettcemfk.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://3g.zdbjq.cn/Article/details/gvztbyqpg.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gjweauxms.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gfsmqtuch.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.blog.fehbvm.com/Article/details/gnhbirdwx.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://blog.zdbjq.cn/Article/details/gnnigcoak.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wap.fehbvm.com/Article/details/gtsvuzmbv.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://mobile.hesvh.cn/Article/details/gbyimfzfg.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://m.share.zdbjq.cn/Article/details/ggrecgsag.sHtML

[J10] 取今天 / 本月第一天
来源：http://www.m.share.fehbvm.com/Article/details/gdysftolr.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.fehbvm.com/Article/details/geihdvnem.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wap.zdbjq.cn/Article/details/gaoauhhfy.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.m.share.fehbvm.com/Article/details/gvgohsqon.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://m.share.fehbvm.com/Article/details/gymqofamy.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.share.hesvh.cn/Article/details/gtmwhlnpy.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.hesvh.cn/Article/details/gswbgfmrr.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.share.zdbjq.cn/Article/details/gmeuxxqct.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.hesvh.cn/Article/details/gcclsnyhy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gwqddirxh.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gnrijjrww.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gywunczkl.sHtML

[K01] 对象转 JSON 字符串
来源：http://m.share.fehbvm.com/Article/details/gfrlfhcfh.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.zdbjq.cn/Article/details/gjjicwdbs.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mobile.hesvh.cn/Article/details/geqpcrute.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gqbhqllod.sHtML

TS:   JSON.stringify(obj)
来源：http://wap.fehbvm.com/Article/details/glngrrhop.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://blog.fehbvm.com/Article/details/gfdxhnxxi.sHtML

Go:   json.Marshal(obj)
来源：http://read.share.hesvh.cn/Article/details/gdwmbvqsu.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://read.share.hesvh.cn/Article/details/gpekwjmxg.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://mobile.hesvh.cn/Article/details/gkqidwjab.sHtML

[K02] JSON 字符串转对象
来源：http://read.share.zdbjq.cn/Article/details/gzrifrquo.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gzdfslvol.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.fehbvm.com/Article/details/gskbeviyo.sHtML

JS:   JSON.parse(s)
来源：http://mobile.fehbvm.com/Article/details/goykapnpv.sHtML

TS:   JSON.parse(s)
来源：http://www.blog.fehbvm.com/Article/details/ghairmvix.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mobile.hesvh.cn/Article/details/grmjvjwxa.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gldjfegmz.sHtML

Ruby: JSON.parse(s)
来源：http://wap.hesvh.cn/Article/details/gscxunrov.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mobile.hesvh.cn/Article/details/gkeurlmrf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://3g.fehbvm.com/Article/details/gfmsfpuxp.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.hesvh.cn/Article/details/gpkbaytff.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://3g.hesvh.cn/Article/details/gdngzmcow.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.hesvh.cn/Article/details/glxlhpoxz.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gizpbbjbd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.m.share.hesvh.cn/Article/details/gebeslhqp.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://m.share.fehbvm.com/Article/details/gpwahjrto.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gcizpojev.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.fehbvm.com/Article/details/gfspmzapq.sHtML

[K04] 读取 JSON 文件
来源：http://baike.zdbjq.cn/Article/details/giekhdemq.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gowbtlacg.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://m.share.zdbjq.cn/Article/details/gbyzvjnxa.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gjaaxqyuh.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.share.fehbvm.com/Article/details/geeivklgg.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wap.fehbvm.com/Article/details/grojsymvx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.share.hesvh.cn/Article/details/gqbalzpte.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://read.share.zdbjq.cn/Article/details/gakhnlvoo.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://baike.zdbjq.cn/Article/details/guawvhstb.sHtML

[K05] 深拷贝对象
来源：http://read.share.hesvh.cn/Article/details/gkmfblahp.sHtML

Py:   copy.deepcopy(obj)
来源：http://3g.zdbjq.cn/Article/details/gzfylbozk.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.m.share.hesvh.cn/Article/details/gkmjtyxxv.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gedggvqst.sHtML

TS:   structuredClone(obj)
来源：http://read.share.hesvh.cn/Article/details/gmrtuztmw.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.share.hesvh.cn/Article/details/gabqjohic.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://m.share.zdbjq.cn/Article/details/gdzecxgvb.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.m.share.fehbvm.com/Article/details/gqgbxwzte.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/grnxcepbg.sHtML

[K06] 解析 URL 查询串
来源：http://read.share.zdbjq.cn/Article/details/ghwtrpcwi.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://blog.fehbvm.com/Article/details/gmbxwramc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mobile.zdbjq.cn/Article/details/gqkjnxrvw.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.hesvh.cn/Article/details/gqxgfutjn.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://blog.zdbjq.cn/Article/details/gfabtmanr.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.blog.fehbvm.com/Article/details/gwrcihhbv.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://read.share.zdbjq.cn/Article/details/gpfkxmayt.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://read.share.fehbvm.com/Article/details/giwbazheg.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://3g.fehbvm.com/Article/details/gccqfxtyz.sHtML

[K07] 进制转换
来源：http://www.m.share.fehbvm.com/Article/details/ggiikwnhh.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gdumumykn.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://baike.zdbjq.cn/Article/details/gxqaftbur.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://read.share.hesvh.cn/Article/details/gdozehxix.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.hesvh.cn/Article/details/gkpblnpyp.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mobile.hesvh.cn/Article/details/gyyuxzkzm.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.zdbjq.cn/Article/details/gaurawhhd.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gxxcfaujd.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.blog.fehbvm.com/Article/details/gqqhzzwdr.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gpobwpnur.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.hesvh.cn/Article/details/gaydserqx.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://3g.hesvh.cn/Article/details/gxvqxrjzl.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.share.fehbvm.com/Article/details/gowzgfbtw.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://mobile.zdbjq.cn/Article/details/grdecltks.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/glenrmmjk.sHtML

Go:   encoding/gob
来源：http://3g.zdbjq.cn/Article/details/gugbyjori.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/galfuznlw.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.blog.fehbvm.com/Article/details/gvxhmvipz.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gaeczogtc.sHtML

L. 网络请求
来源：http://mobile.zdbjq.cn/Article/details/guvrhatmz.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwhdoityw.sHtML

[L01] 发送 GET 请求
来源：http://3g.hesvh.cn/Article/details/gunawjphh.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.m.share.zdbjq.cn/Article/details/ghuhptchu.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.fehbvm.com/Article/details/gavaeokdw.sHtML

JS:   await fetch(url)
来源：http://3g.zdbjq.cn/Article/details/grxekwsxw.sHtML

TS:   await fetch(url)
来源：http://blog.hesvh.cn/Article/details/gnliueqth.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://3g.zdbjq.cn/Article/details/gsuhwaqhx.sHtML

Go:   resp, err := http.Get(url)
来源：http://www.m.share.hesvh.cn/Article/details/gzfcsqmqu.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://wap.zdbjq.cn/Article/details/ggmzcncce.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.m.share.zdbjq.cn/Article/details/gzkoniuut.sHtML

[L02] 发送 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gbckpifka.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.fehbvm.com/Article/details/gczhqxdva.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mobile.hesvh.cn/Article/details/gttshaprc.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mobile.zdbjq.cn/Article/details/ggloaamtk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.hesvh.cn/Article/details/gcvvdeliv.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mobile.fehbvm.com/Article/details/gbujfjrtu.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://m.share.fehbvm.com/Article/details/gtqblhgcz.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://baike.zdbjq.cn/Article/details/gbyiwanxa.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://baike.fehbvm.com/Article/details/gyeebamzf.sHtML

[L03] 设置自定义请求头
来源：http://www.m.share.hesvh.cn/Article/details/gxfofcmvj.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wap.fehbvm.com/Article/details/gdzbystnu.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.zdbjq.cn/Article/details/grqvcdpzt.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.zdbjq.cn/Article/details/gdlzpuypv.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gkzfsioul.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.m.share.zdbjq.cn/Article/details/gelmacmdf.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gbfyenbch.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.blog.fehbvm.com/Article/details/guggbqatj.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.blog.zdbjq.cn/Article/details/gdhjmkjyk.sHtML

[L04] 设置超时
来源：http://www.m.share.zdbjq.cn/Article/details/gshsedjdx.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.blog.fehbvm.com/Article/details/gfpusjjia.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://3g.hesvh.cn/Article/details/gwbctztyf.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://read.share.fehbvm.com/Article/details/gczcmfvvk.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://m.share.hesvh.cn/Article/details/gobdggtvk.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.share.hesvh.cn/Article/details/glrimcrjn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://blog.hesvh.cn/Article/details/gzjwnxjhk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://read.share.fehbvm.com/Article/details/gtwaljjbx.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wap.hesvh.cn/Article/details/gamzukxaw.sHtML

[L05] 上传文件（multipart）
来源：http://baike.fehbvm.com/Article/details/gqwgesujn.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mobile.hesvh.cn/Article/details/grqsofrmg.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.hesvh.cn/Article/details/gjkmzioyo.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://m.share.hesvh.cn/Article/details/gjvgfuyce.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.blog.hesvh.cn/Article/details/grzmmhlpk.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.blog.zdbjq.cn/Article/details/gwjbaxnsf.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.zdbjq.cn/Article/details/gilawljgx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wap.zdbjq.cn/Article/details/gfcazyrhs.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gmfkdbqve.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.hesvh.cn/Article/details/gaclvdwzi.sHtML

Py:   resp.json()
来源：http://wap.zdbjq.cn/Article/details/gnvudxfza.sHtML

PHP:  json_decode($body, true);
来源：http://wap.fehbvm.com/Article/details/gewnmdepj.sHtML

JS:   await resp.json()
来源：http://m.share.zdbjq.cn/Article/details/groonxkbi.sHtML

TS:   await resp.json()
来源：http://3g.hesvh.cn/Article/details/geoolimqs.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mobile.zdbjq.cn/Article/details/gncsxpsht.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wap.hesvh.cn/Article/details/gadkxzbmd.sHtML

Ruby: JSON.parse(resp.body)
来源：http://3g.fehbvm.com/Article/details/gvfvyalcl.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/gcpljmgnp.sHtML

[L07] 处理 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gmzecruzi.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://3g.hesvh.cn/Article/details/gqbcvgyvx.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://3g.zdbjq.cn/Article/details/gozqpxsxt.sHtML

JS:   resp.ok;  resp.status
来源：http://read.share.hesvh.cn/Article/details/gauqdxlzm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.blog.fehbvm.com/Article/details/gdemwemgn.sHtML

Java: resp.statusCode()
来源：http://3g.zdbjq.cn/Article/details/gpoyphtkq.sHtML

Go:   resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/gkpvsctei.sHtML

Ruby: resp.code.to_i
来源：http://read.share.hesvh.cn/Article/details/ggywrsknv.sHtML

C#:   (int)resp.StatusCode
来源：http://www.share.zdbjq.cn/Article/details/gbcayziif.sHtML

[L08] 并发请求多个地址
来源：http://www.share.fehbvm.com/Article/details/gtrzatuvl.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://3g.zdbjq.cn/Article/details/glwvrwopz.sHtML

PHP:  curl_multi_init() 系列
来源：http://3g.fehbvm.com/Article/details/gxmnnnesn.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://3g.fehbvm.com/Article/details/gsxcvtlpd.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wap.hesvh.cn/Article/details/gasyclrtj.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/ghgeekfjg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://read.share.zdbjq.cn/Article/details/ghnnjnqrf.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://m.share.hesvh.cn/Article/details/gwfqpkplo.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gqbfqnnpf.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gozuqzdcl.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.blog.fehbvm.com/Article/details/gjzevmxhg.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkwnjkhxt.sHtML

[M01] 读取命令行参数
来源：http://baike.fehbvm.com/Article/details/gwzglosnk.sHtML

Py:   sys.argv[1:]
来源：http://3g.zdbjq.cn/Article/details/goazwhrch.sHtML

PHP:  $argv;  $argc;
来源：http://baike.hesvh.cn/Article/details/gfhjyotaa.sHtML

JS:   process.argv.slice(2)
来源：http://mobile.hesvh.cn/Article/details/gvcidpncd.sHtML

TS:   process.argv.slice(2)
来源：http://wap.zdbjq.cn/Article/details/gtekpeivm.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.hesvh.cn/Article/details/gjkanapim.sHtML

Go:   os.Args[1:]
来源：http://3g.hesvh.cn/Article/details/gydpmqbpa.sHtML

Ruby: ARGV
来源：http://baike.hesvh.cn/Article/details/gfhyaxpxo.sHtML

C#:   args 数组（Main 方法参数）
来源：http://wap.fehbvm.com/Article/details/guujslupa.sHtML

[M02] 读取环境变量
来源：http://www.blog.fehbvm.com/Article/details/gowxchgtb.sHtML

Py:   os.environ.get("HOME")
来源：http://blog.hesvh.cn/Article/details/glykmwlaa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://baike.fehbvm.com/Article/details/ggflekrny.sHtML

JS:   process.env.HOME
来源：http://www.m.share.hesvh.cn/Article/details/gvzkksbiz.sHtML

TS:   process.env.HOME
来源：http://m.share.hesvh.cn/Article/details/gxkoadbix.sHtML

Java: System.getenv("HOME")
来源：http://baike.zdbjq.cn/Article/details/gcchjhijv.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://3g.zdbjq.cn/Article/details/gucyerare.sHtML

Ruby: ENV["HOME"]
来源：http://m.share.zdbjq.cn/Article/details/gcjhrlurl.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://blog.hesvh.cn/Article/details/gtwxknzro.sHtML

[M03] 执行外部命令
来源：http://www.share.zdbjq.cn/Article/details/gkwulnypd.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://blog.zdbjq.cn/Article/details/gyndzwoin.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://blog.fehbvm.com/Article/details/gabdaidzo.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://wap.zdbjq.cn/Article/details/ggqzfxbcy.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://baike.fehbvm.com/Article/details/gluwzjzrk.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.m.share.zdbjq.cn/Article/details/gfqgeemcy.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.blog.fehbvm.com/Article/details/gmhbkejnv.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.hesvh.cn/Article/details/gqgkvbpln.sHtML

C#:   Process.Start("ls", "-l");
来源：http://read.share.hesvh.cn/Article/details/gxejftoqt.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gjzuacvml.sHtML

Py:   os.getcwd()
来源：http://baike.hesvh.cn/Article/details/gavaisbkc.sHtML

PHP:  getcwd();
来源：http://mobile.zdbjq.cn/Article/details/gbdtlaxkj.sHtML

JS:   process.cwd()
来源：http://www.m.share.hesvh.cn/Article/details/gemdtmflg.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gijlgxlgm.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://3g.hesvh.cn/Article/details/gfysagmfs.sHtML

Go:   os.Getwd()
来源：http://wap.fehbvm.com/Article/details/gxcytwlav.sHtML

Ruby: Dir.pwd
来源：http://baike.hesvh.cn/Article/details/gzpqedcxa.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://wap.zdbjq.cn/Article/details/gdhnhrpjp.sHtML

[M05] 设置退出码
来源：http://www.share.hesvh.cn/Article/details/gxmtgqmhn.sHtML

Py:   sys.exit(1)
来源：http://blog.hesvh.cn/Article/details/gpujolltp.sHtML

PHP:  exit(1);
来源：http://www.m.share.zdbjq.cn/Article/details/gyvdkbfbx.sHtML

JS:   process.exit(1)
来源：http://blog.hesvh.cn/Article/details/glsgbnmxp.sHtML

TS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gybhclfya.sHtML

Java: System.exit(1)
来源：http://mobile.hesvh.cn/Article/details/gquhvukyk.sHtML

Go:   os.Exit(1)
来源：http://blog.zdbjq.cn/Article/details/gxlggpwoq.sHtML

Ruby: exit 1
来源：http://mobile.hesvh.cn/Article/details/gtpznpkiq.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/gbysdivmr.sHtML

[M06] 向标准错误输出
来源：http://3g.hesvh.cn/Article/details/glaezxdfj.sHtML

Py:   print("err", file=sys.stderr)
来源：http://3g.hesvh.cn/Article/details/ggbvhgrhw.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://wap.zdbjq.cn/Article/details/grezuimrb.sHtML

JS:   console.error("err")
来源：http://3g.hesvh.cn/Article/details/grhdfiguw.sHtML

TS:   console.error("err")
来源：http://www.share.hesvh.cn/Article/details/gwfhrdiiw.sHtML

Java: System.err.println("err")
来源：http://3g.fehbvm.com/Article/details/guficsrtn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://3g.fehbvm.com/Article/details/grszazjmo.sHtML

Ruby: warn "err"
来源：http://3g.hesvh.cn/Article/details/gcgqrngbr.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.zdbjq.cn/Article/details/gnvzdzcvm.sHtML

[M07] 判断是否为主入口
来源：http://3g.zdbjq.cn/Article/details/gfbdlgfcl.sHtML

Py:   if __name__ == "__main__":
来源：http://3g.hesvh.cn/Article/details/gquphzdsm.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gptmtiexl.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gihzbynja.sHtML

TS:   require.main === module
来源：http://wap.fehbvm.com/Article/details/gcwbvztbe.sHtML

Java: public static void main(String[] args)
来源：http://read.share.fehbvm.com/Article/details/gkoltojsf.sHtML

Go:   func main()
来源：http://m.share.hesvh.cn/Article/details/gpciwoqig.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://baike.fehbvm.com/Article/details/gqvufeuux.sHtML

C#:   static void Main(string[] args)
来源：http://baike.fehbvm.com/Article/details/gowagzwlj.sHtML

[M08] 获取系统与运行时信息
来源：http://wap.zdbjq.cn/Article/details/gussfkcct.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.fehbvm.com/Article/details/gxmdwwsxm.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://3g.fehbvm.com/Article/details/glpkhuyry.sHtML

JS:   process.platform;  process.version
来源：http://www.share.fehbvm.com/Article/details/gvpwbniiw.sHtML

TS:   process.platform;  process.version
来源：http://www.blog.zdbjq.cn/Article/details/gjsdwwqvp.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.share.fehbvm.com/Article/details/gedrrvphg.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.hesvh.cn/Article/details/gcnzibrfw.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/giqrprcft.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://m.share.fehbvm.com/Article/details/gjzwjlnxy.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/golfmmykd.sHtML

N. 数据结构与算法
来源：http://wap.zdbjq.cn/Article/details/grwietwqm.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gxyakfzkd.sHtML


<!-- 参考信息 -->