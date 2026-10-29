代发 wailian999

[J03] 字符串解析为日期
来源：http://www.m.share.hesvh.cn/Article/details/gqbyjrzxg.sHtML

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://baike.zdbjq.cn/Article/details/gzggrjtjm.sHtML

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://blog.zdbjq.cn/Article/details/gbakelrvk.sHtML

JS:   new Date("2024-01-02")
来源：http://www.m.share.zdbjq.cn/Article/details/gqryudhvc.sHtML

TS:   new Date("2024-01-02")
来源：http://read.share.zdbjq.cn/Article/details/gywabmkfz.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.hesvh.cn/Article/details/gbpbrmzid.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://mobile.hesvh.cn/Article/details/gpgpmfjqx.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://m.share.hesvh.cn/Article/details/gwgoluzzb.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.blog.zdbjq.cn/Article/details/gfasgyslt.sHtML

[J04] 时间戳与日期互转
来源：http://www.blog.fehbvm.com/Article/details/gmtjrqodt.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://mobile.zdbjq.cn/Article/details/gbxggonxw.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://blog.hesvh.cn/Article/details/gqrxzbryp.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.blog.hesvh.cn/Article/details/grzvfvvcs.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://www.share.fehbvm.com/Article/details/gofwgkboh.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.blog.hesvh.cn/Article/details/gasrtrgvl.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://blog.hesvh.cn/Article/details/gmvaoipsx.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://baike.hesvh.cn/Article/details/guyzeangz.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://wap.zdbjq.cn/Article/details/gmavjbaoa.sHtML

[J05] 时间加减（加 7 天）
来源：http://www.m.share.fehbvm.com/Article/details/gzfkpdelb.sHtML

Py:   now + timedelta(days=7)
来源：http://www.share.hesvh.cn/Article/details/gmvrjztcg.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://wap.zdbjq.cn/Article/details/gceltoprk.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.fehbvm.com/Article/details/gabirgvrz.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wap.hesvh.cn/Article/details/gxbjppvyo.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.share.hesvh.cn/Article/details/gzhykjybi.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/govjzruty.sHtML

Ruby: Time.now + 7 * 86400
来源：http://www.m.share.hesvh.cn/Article/details/gpggcnfqs.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://wap.hesvh.cn/Article/details/gmdvronez.sHtML

[J06] 计算两时间之差
来源：http://mobile.zdbjq.cn/Article/details/gpemwstmt.sHtML

Py:   (end - start).total_seconds()
来源：http://www.share.zdbjq.cn/Article/details/guvohlqgc.sHtML

PHP:  $end->diff($start)->days;
来源：http://baike.hesvh.cn/Article/details/gsyqzpory.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.fehbvm.com/Article/details/gpuyumetn.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.m.share.hesvh.cn/Article/details/gtmnzngls.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.blog.hesvh.cn/Article/details/grridwyep.sHtML

Go:   end.Sub(start).Hours()
来源：http://blog.zdbjq.cn/Article/details/gyiigfdpj.sHtML

Ruby: end - start                 # 返回秒数
来源：http://read.share.fehbvm.com/Article/details/ghfkwssde.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gphymokbr.sHtML

[J07] 比较两个日期
来源：http://www.blog.hesvh.cn/Article/details/gwqitaeef.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/guoesrvzd.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://blog.fehbvm.com/Article/details/grqjfkvpf.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://www.m.share.hesvh.cn/Article/details/gtforxyzo.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://www.blog.hesvh.cn/Article/details/gtzsilsmg.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://blog.zdbjq.cn/Article/details/gwoajmiuy.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/ggwklwcsl.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://m.share.zdbjq.cn/Article/details/gfhehsusa.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://www.m.share.hesvh.cn/Article/details/gcseythzj.sHtML

[J08] 提取年月日与星期
来源：http://baike.fehbvm.com/Article/details/gzqravgrk.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mobile.zdbjq.cn/Article/details/giqrdlkth.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://blog.hesvh.cn/Article/details/gmomngtxc.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wap.zdbjq.cn/Article/details/gutegjzpt.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://wap.fehbvm.com/Article/details/gbgwgzilu.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://blog.zdbjq.cn/Article/details/gjnjzcoru.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://wap.zdbjq.cn/Article/details/guaffbodm.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://m.share.zdbjq.cn/Article/details/gggpulmma.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.zdbjq.cn/Article/details/gthsoaick.sHtML

[J09] 时区处理
来源：http://read.share.fehbvm.com/Article/details/gsgohtgho.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mobile.fehbvm.com/Article/details/gsbqunofj.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://mobile.fehbvm.com/Article/details/gtunolpcx.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.hesvh.cn/Article/details/gestdexfx.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blog.zdbjq.cn/Article/details/gybskkdkc.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://baike.zdbjq.cn/Article/details/gjkedypzz.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mobile.zdbjq.cn/Article/details/gormzcdmk.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://3g.zdbjq.cn/Article/details/gfcoyltwd.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://blog.fehbvm.com/Article/details/graeurgff.sHtML

[J10] 取今天 / 本月第一天
来源：http://blog.fehbvm.com/Article/details/gapobdqzc.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://mobile.zdbjq.cn/Article/details/grwahcxay.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://blog.fehbvm.com/Article/details/gqdpvefwe.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.share.fehbvm.com/Article/details/gdmvatctm.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.share.zdbjq.cn/Article/details/gzlrhlqzk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://baike.zdbjq.cn/Article/details/gxeplhfnr.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://blog.hesvh.cn/Article/details/gbzviglwm.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://3g.zdbjq.cn/Article/details/gsqxfsxps.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://blog.zdbjq.cn/Article/details/glymrhyjb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjjpfwudy.sHtML

K. JSON 与序列化
来源：http://mobile.hesvh.cn/Article/details/gdsoamzbo.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gmreoxjbe.sHtML

[K01] 对象转 JSON 字符串
来源：http://3g.fehbvm.com/Article/details/gkrimfcsg.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wap.fehbvm.com/Article/details/giyfvunjp.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://read.share.zdbjq.cn/Article/details/gaefvwwij.sHtML

JS:   JSON.stringify(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gghtuyipv.sHtML

TS:   JSON.stringify(obj)
来源：http://www.blog.hesvh.cn/Article/details/gltfelehv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://wap.zdbjq.cn/Article/details/gfoqslfhs.sHtML

Go:   json.Marshal(obj)
来源：http://www.share.zdbjq.cn/Article/details/gxkdrurpm.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://3g.zdbjq.cn/Article/details/gfuvvvjgf.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://3g.fehbvm.com/Article/details/gdsxpltxf.sHtML

[K02] JSON 字符串转对象
来源：http://3g.fehbvm.com/Article/details/gpdpdyoru.sHtML

Py:   json.loads(s)
来源：http://www.m.share.hesvh.cn/Article/details/glvspvmwi.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.zdbjq.cn/Article/details/gecxqcsvc.sHtML

JS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gpxevxbku.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gskglqsrm.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://blog.zdbjq.cn/Article/details/gmjnwjrmk.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.m.share.hesvh.cn/Article/details/gkkjdktxj.sHtML

Ruby: JSON.parse(s)
来源：http://www.share.fehbvm.com/Article/details/gbgoqamnh.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.share.zdbjq.cn/Article/details/govosopxz.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://m.share.hesvh.cn/Article/details/gxmafnftb.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.m.share.hesvh.cn/Article/details/gbqgquqyx.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.blog.fehbvm.com/Article/details/gzjlprvxk.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.fehbvm.com/Article/details/gtrtamffp.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://www.blog.hesvh.cn/Article/details/gugqzzlqo.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.share.fehbvm.com/Article/details/gtatbtumi.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://read.share.zdbjq.cn/Article/details/grkcvbtls.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.blog.zdbjq.cn/Article/details/gqdkfdasu.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mobile.zdbjq.cn/Article/details/grwcuydgh.sHtML

[K04] 读取 JSON 文件
来源：http://mobile.hesvh.cn/Article/details/gcwxmdisv.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://m.share.zdbjq.cn/Article/details/gqbgipaik.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.share.zdbjq.cn/Article/details/gkisqboif.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://blog.fehbvm.com/Article/details/gopaykcls.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gvxbejrwl.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://blog.zdbjq.cn/Article/details/gwdbfsmmb.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.m.share.zdbjq.cn/Article/details/grbmzyklv.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://wap.fehbvm.com/Article/details/gthnlngtn.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://blog.fehbvm.com/Article/details/ghlrsjkrx.sHtML

[K05] 深拷贝对象
来源：http://mobile.fehbvm.com/Article/details/gaqqgdzbw.sHtML

Py:   copy.deepcopy(obj)
来源：http://www.share.zdbjq.cn/Article/details/gwnxrnmbt.sHtML

PHP:  unserialize(serialize($obj));
来源：http://www.blog.hesvh.cn/Article/details/gjuefkqdi.sHtML

JS:   structuredClone(obj)
来源：http://wap.zdbjq.cn/Article/details/gsdjtfwwn.sHtML

TS:   structuredClone(obj)
来源：http://m.share.fehbvm.com/Article/details/gecszughs.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://www.blog.fehbvm.com/Article/details/grcbqkibb.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wap.hesvh.cn/Article/details/gehdfevzj.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.zdbjq.cn/Article/details/gthklnvdg.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://baike.zdbjq.cn/Article/details/gvnonqjri.sHtML

[K06] 解析 URL 查询串
来源：http://mobile.hesvh.cn/Article/details/gilsrfogy.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.fehbvm.com/Article/details/gcelyaroc.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.hesvh.cn/Article/details/gtuqwhjqp.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gjqeehrkd.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.m.share.hesvh.cn/Article/details/gzfubbown.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wap.fehbvm.com/Article/details/gwfykikxq.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.share.fehbvm.com/Article/details/galtmvyau.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gwnnvxgek.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wap.hesvh.cn/Article/details/grpxdhyeq.sHtML

[K07] 进制转换
来源：http://www.share.hesvh.cn/Article/details/gcptdzmom.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://m.share.fehbvm.com/Article/details/gcubyyrln.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wap.fehbvm.com/Article/details/gydulxbpe.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gbhnjawsr.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wap.fehbvm.com/Article/details/gmncsinxw.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.blog.zdbjq.cn/Article/details/gehfomrcc.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.m.share.fehbvm.com/Article/details/gbspsqppc.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wap.fehbvm.com/Article/details/gnkgieypz.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mobile.fehbvm.com/Article/details/gqcbtvyem.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://m.share.fehbvm.com/Article/details/gtctkhgwp.sHtML

Py:   pickle.dumps(obj)
来源：http://m.share.zdbjq.cn/Article/details/gsylucfdh.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://wap.hesvh.cn/Article/details/gpzojjghs.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://m.share.hesvh.cn/Article/details/gnebmhhyo.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://baike.fehbvm.com/Article/details/gayabwrsw.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://3g.fehbvm.com/Article/details/guldlsmmd.sHtML

Go:   encoding/gob
来源：http://read.share.fehbvm.com/Article/details/gxafhxfea.sHtML

Ruby: Marshal.dump(obj)
来源：http://3g.zdbjq.cn/Article/details/glsdwggho.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://blog.hesvh.cn/Article/details/gppfhkmcv.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghxbwicvu.sHtML

L. 网络请求
来源：http://mobile.hesvh.cn/Article/details/gdlelydii.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gavnibmen.sHtML

[L01] 发送 GET 请求
来源：http://m.share.fehbvm.com/Article/details/ggvgdslwq.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.blog.zdbjq.cn/Article/details/gdejmqnhs.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.share.zdbjq.cn/Article/details/gmavglhut.sHtML

JS:   await fetch(url)
来源：http://3g.hesvh.cn/Article/details/gejjhfkwa.sHtML

TS:   await fetch(url)
来源：http://blog.zdbjq.cn/Article/details/genurcrrp.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.share.hesvh.cn/Article/details/gfciabzlg.sHtML

Go:   resp, err := http.Get(url)
来源：http://blog.fehbvm.com/Article/details/gsyfhzmei.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://m.share.zdbjq.cn/Article/details/gkbmsydla.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://read.share.hesvh.cn/Article/details/gkjswnsih.sHtML

[L02] 发送 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gmiuhhsuh.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://blog.hesvh.cn/Article/details/gzpaeytov.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/glrcdhcge.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wap.fehbvm.com/Article/details/ghwkdfvlk.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://m.share.hesvh.cn/Article/details/gkizdcpgw.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://blog.fehbvm.com/Article/details/gebiqdvnl.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mobile.hesvh.cn/Article/details/gfwfavues.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.share.zdbjq.cn/Article/details/gxtmipfnl.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.share.fehbvm.com/Article/details/gwhwoyzgi.sHtML

[L03] 设置自定义请求头
来源：http://mobile.zdbjq.cn/Article/details/gcmeaxdmp.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://mobile.hesvh.cn/Article/details/gneuxmcec.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://baike.hesvh.cn/Article/details/gsifgfzkz.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/ghytviizp.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://read.share.fehbvm.com/Article/details/gfsiwjvrz.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://baike.fehbvm.com/Article/details/gakmbtsfx.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wap.zdbjq.cn/Article/details/gbvubsulm.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://3g.fehbvm.com/Article/details/ggfrvfddx.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://blog.zdbjq.cn/Article/details/gshnycqxi.sHtML

[L04] 设置超时
来源：http://wap.hesvh.cn/Article/details/gmytdtmhu.sHtML

Py:   requests.get(url, timeout=5)
来源：http://baike.fehbvm.com/Article/details/gktndmsdc.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.fehbvm.com/Article/details/gfvixkzve.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://3g.fehbvm.com/Article/details/glyjewvzs.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://blog.fehbvm.com/Article/details/gyxzhpvdx.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mobile.hesvh.cn/Article/details/ghcpgopcn.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://wap.hesvh.cn/Article/details/gueazwzai.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.zdbjq.cn/Article/details/gupnkfchm.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://3g.fehbvm.com/Article/details/gutpfmhnl.sHtML

[L05] 上传文件（multipart）
来源：http://m.share.fehbvm.com/Article/details/gevzjjyzx.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://3g.zdbjq.cn/Article/details/gfqeyjkjk.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.share.hesvh.cn/Article/details/gucpcdwsd.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gwwgroknp.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://3g.fehbvm.com/Article/details/gucigxplf.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wap.fehbvm.com/Article/details/gmuajcrfx.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mobile.hesvh.cn/Article/details/goqyxqjhi.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://3g.hesvh.cn/Article/details/gmsaoodan.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wap.hesvh.cn/Article/details/gouniuemw.sHtML

[L06] 解析响应为 JSON
来源：http://www.share.fehbvm.com/Article/details/gnlqtkswy.sHtML

Py:   resp.json()
来源：http://read.share.zdbjq.cn/Article/details/giimgqyiv.sHtML

PHP:  json_decode($body, true);
来源：http://wap.hesvh.cn/Article/details/gyqhsqmhz.sHtML

JS:   await resp.json()
来源：http://3g.zdbjq.cn/Article/details/gekokakyp.sHtML

TS:   await resp.json()
来源：http://www.blog.fehbvm.com/Article/details/gypjxmwne.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wap.zdbjq.cn/Article/details/gwrunqjbd.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://blog.hesvh.cn/Article/details/ggiihpoya.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.zdbjq.cn/Article/details/gsatqnekg.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.hesvh.cn/Article/details/gidxhggdv.sHtML

[L07] 处理 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gssgwidne.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.fehbvm.com/Article/details/gdqmjakic.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://m.share.fehbvm.com/Article/details/gmedmksuu.sHtML

JS:   resp.ok;  resp.status
来源：http://www.m.share.hesvh.cn/Article/details/gkmyktonm.sHtML

TS:   resp.ok;  resp.status
来源：http://www.share.zdbjq.cn/Article/details/gddeevscg.sHtML

Java: resp.statusCode()
来源：http://read.share.zdbjq.cn/Article/details/gynhbpgzk.sHtML

Go:   resp.StatusCode
来源：http://www.share.fehbvm.com/Article/details/gxyscints.sHtML

Ruby: resp.code.to_i
来源：http://www.share.fehbvm.com/Article/details/gonchnryk.sHtML

C#:   (int)resp.StatusCode
来源：http://mobile.zdbjq.cn/Article/details/gmjzrrsyh.sHtML

[L08] 并发请求多个地址
来源：http://mobile.hesvh.cn/Article/details/gpbbgdiva.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://m.share.hesvh.cn/Article/details/grajomydz.sHtML

PHP:  curl_multi_init() 系列
来源：http://wap.fehbvm.com/Article/details/guqhjuisx.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.hesvh.cn/Article/details/gifspdfzk.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.zdbjq.cn/Article/details/gekbehbkk.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.fehbvm.com/Article/details/gxpfrutri.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.hesvh.cn/Article/details/goawroucn.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://blog.hesvh.cn/Article/details/gcwtfmhya.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://3g.zdbjq.cn/Article/details/gvixflolt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gjpodaqcx.sHtML

M. 命令行 / 进程 / 环境
来源：http://read.share.fehbvm.com/Article/details/gfqzvmxei.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxlabhhsr.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gvwytknky.sHtML

Py:   sys.argv[1:]
来源：http://mobile.fehbvm.com/Article/details/gccqdorjg.sHtML

PHP:  $argv;  $argc;
来源：http://blog.fehbvm.com/Article/details/gzuwuusce.sHtML

JS:   process.argv.slice(2)
来源：http://3g.fehbvm.com/Article/details/gjtewukhl.sHtML

TS:   process.argv.slice(2)
来源：http://3g.hesvh.cn/Article/details/gemijldon.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.fehbvm.com/Article/details/gfiqtrytv.sHtML

Go:   os.Args[1:]
来源：http://m.share.hesvh.cn/Article/details/gdjzwvwpf.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gspgswvbw.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gzdmyzjac.sHtML

[M02] 读取环境变量
来源：http://3g.fehbvm.com/Article/details/gfnkbhtfk.sHtML

Py:   os.environ.get("HOME")
来源：http://wap.zdbjq.cn/Article/details/gyfgsirvl.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mobile.zdbjq.cn/Article/details/gczumfdwr.sHtML

JS:   process.env.HOME
来源：http://mobile.fehbvm.com/Article/details/gprlgedlq.sHtML

TS:   process.env.HOME
来源：http://wap.zdbjq.cn/Article/details/goyathgwh.sHtML

Java: System.getenv("HOME")
来源：http://read.share.zdbjq.cn/Article/details/ggnbkvoef.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.fehbvm.com/Article/details/gpyhrjslr.sHtML

Ruby: ENV["HOME"]
来源：http://www.share.fehbvm.com/Article/details/gchzkdlls.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://3g.hesvh.cn/Article/details/gxoxqhgut.sHtML

[M03] 执行外部命令
来源：http://wap.hesvh.cn/Article/details/gbevqqzyt.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.blog.zdbjq.cn/Article/details/gnpspwyza.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.zdbjq.cn/Article/details/gywwvpdxs.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://read.share.fehbvm.com/Article/details/gnmctmaol.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.zdbjq.cn/Article/details/gtvjoddev.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.fehbvm.com/Article/details/ghnimvosn.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://www.share.hesvh.cn/Article/details/gnaijqbck.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.fehbvm.com/Article/details/gtwrlkqkl.sHtML

C#:   Process.Start("ls", "-l");
来源：http://blog.fehbvm.com/Article/details/gcoiuhwwe.sHtML

[M04] 获取当前工作目录
来源：http://www.share.zdbjq.cn/Article/details/gmtpwpmoh.sHtML

Py:   os.getcwd()
来源：http://m.share.zdbjq.cn/Article/details/guqmdnppa.sHtML

PHP:  getcwd();
来源：http://wap.hesvh.cn/Article/details/gumtniftz.sHtML

JS:   process.cwd()
来源：http://www.share.zdbjq.cn/Article/details/gazdjogrp.sHtML

TS:   process.cwd()
来源：http://www.share.fehbvm.com/Article/details/gtdrfzgsi.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://www.share.fehbvm.com/Article/details/ggtsiqfew.sHtML

Go:   os.Getwd()
来源：http://mobile.fehbvm.com/Article/details/glcgmvgng.sHtML

Ruby: Dir.pwd
来源：http://3g.hesvh.cn/Article/details/geofkokjv.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://read.share.hesvh.cn/Article/details/giwaohtuv.sHtML

[M05] 设置退出码
来源：http://wap.zdbjq.cn/Article/details/gkqmbajui.sHtML

Py:   sys.exit(1)
来源：http://read.share.hesvh.cn/Article/details/grrjdimwx.sHtML

PHP:  exit(1);
来源：http://read.share.hesvh.cn/Article/details/gzeuewubc.sHtML

JS:   process.exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjpmngsz.sHtML

TS:   process.exit(1)
来源：http://www.m.share.fehbvm.com/Article/details/gufcjdlzb.sHtML

Java: System.exit(1)
来源：http://www.share.zdbjq.cn/Article/details/gdxyyxknr.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gjcugjwtd.sHtML

Ruby: exit 1
来源：http://www.share.fehbvm.com/Article/details/gwjilgjlw.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://m.share.hesvh.cn/Article/details/ghtqagazu.sHtML

[M06] 向标准错误输出
来源：http://www.share.zdbjq.cn/Article/details/glifudzol.sHtML

Py:   print("err", file=sys.stderr)
来源：http://m.share.fehbvm.com/Article/details/ghhsdfodh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://baike.hesvh.cn/Article/details/gkgikwmdf.sHtML

JS:   console.error("err")
来源：http://wap.hesvh.cn/Article/details/gbbkidchy.sHtML

TS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gojrffxnc.sHtML

Java: System.err.println("err")
来源：http://www.share.fehbvm.com/Article/details/gtbnuzgrn.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.m.share.zdbjq.cn/Article/details/gmbeasejn.sHtML

Ruby: warn "err"
来源：http://read.share.fehbvm.com/Article/details/gsdpxhbjg.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://baike.fehbvm.com/Article/details/gxhahagax.sHtML

[M07] 判断是否为主入口
来源：http://wap.zdbjq.cn/Article/details/glsrnslor.sHtML

Py:   if __name__ == "__main__":
来源：http://blog.fehbvm.com/Article/details/giwlxynoc.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blog.hesvh.cn/Article/details/gomhbtqpu.sHtML

JS:   require.main === module
来源：http://3g.zdbjq.cn/Article/details/gstdzuqme.sHtML

TS:   require.main === module
来源：http://wap.hesvh.cn/Article/details/gpfepwcje.sHtML

Java: public static void main(String[] args)
来源：http://3g.hesvh.cn/Article/details/glxuajona.sHtML

Go:   func main()
来源：http://read.share.zdbjq.cn/Article/details/gfjdqiene.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.hesvh.cn/Article/details/gjfshmfwi.sHtML

C#:   static void Main(string[] args)
来源：http://www.m.share.fehbvm.com/Article/details/gsolhesio.sHtML

[M08] 获取系统与运行时信息
来源：http://blog.fehbvm.com/Article/details/gquqjxucf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://3g.zdbjq.cn/Article/details/gpdiwemdr.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://blog.fehbvm.com/Article/details/gpyybywfs.sHtML

JS:   process.platform;  process.version
来源：http://wap.hesvh.cn/Article/details/gfrofhsyz.sHtML

TS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/gpsyrxkqy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mobile.hesvh.cn/Article/details/galmvryzx.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.fehbvm.com/Article/details/gfxvdklms.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.fehbvm.com/Article/details/ghpallpir.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.fehbvm.com/Article/details/gmwsobtmj.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gzmspdotq.sHtML

N. 数据结构与算法
来源：http://www.m.share.hesvh.cn/Article/details/gorwyyulh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gyvsgyjic.sHtML


<!-- 参考信息 -->