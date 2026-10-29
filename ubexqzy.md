代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.m.share.fehbvm.com/Article/details/gxtajhisl.sHtML

Java: LocalDate.parse("2024-01-02")
来源：http://baike.zdbjq.cn/Article/details/gmktbefjd.sHtML

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://m.share.zdbjq.cn/Article/details/gxnhwfdnb.sHtML

Ruby: Date.parse("2024-01-02")
来源：http://mobile.fehbvm.com/Article/details/gbbsgoqzq.sHtML

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://m.share.fehbvm.com/Article/details/gzwuecnxp.sHtML

[J04] 时间戳与日期互转
来源：http://m.share.hesvh.cn/Article/details/gkgemldps.sHtML

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://3g.zdbjq.cn/Article/details/gipvoquvd.sHtML

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://3g.zdbjq.cn/Article/details/gtooydanu.sHtML

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://blog.hesvh.cn/Article/details/gmkthsxte.sHtML

TS:   Math.floor(Date.now() / 1000)
来源：http://3g.fehbvm.com/Article/details/gznuuqaas.sHtML

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://blog.fehbvm.com/Article/details/gkokhaavy.sHtML

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://m.share.hesvh.cn/Article/details/gefgfuogk.sHtML

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://m.share.hesvh.cn/Article/details/ghejiqptw.sHtML

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://baike.hesvh.cn/Article/details/gurcvehbr.sHtML

[J05] 时间加减（加 7 天）
来源：http://m.share.fehbvm.com/Article/details/gpqhsnofq.sHtML

Py:   now + timedelta(days=7)
来源：http://baike.fehbvm.com/Article/details/ghxrnwkaz.sHtML

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.share.fehbvm.com/Article/details/gcwvmpnum.sHtML

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://3g.zdbjq.cn/Article/details/gjbgayrpn.sHtML

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://mobile.zdbjq.cn/Article/details/gjntvpifs.sHtML

Java: LocalDate.now().plusDays(7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghajwdtuk.sHtML

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.share.fehbvm.com/Article/details/gkvmvpjwm.sHtML

Ruby: Time.now + 7 * 86400
来源：http://wap.hesvh.cn/Article/details/gvhgnigyj.sHtML

C#:   DateTime.Now.AddDays(7)
来源：http://www.blog.hesvh.cn/Article/details/gamfziuql.sHtML

[J06] 计算两时间之差
来源：http://www.blog.hesvh.cn/Article/details/gwtljwuqn.sHtML

Py:   (end - start).total_seconds()
来源：http://blog.hesvh.cn/Article/details/gwmbynavp.sHtML

PHP:  $end->diff($start)->days;
来源：http://3g.zdbjq.cn/Article/details/geyttympk.sHtML

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://3g.zdbjq.cn/Article/details/ghyazsdip.sHtML

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://read.share.zdbjq.cn/Article/details/gigsladsz.sHtML

Java: Duration.between(start, end).toSeconds()
来源：http://www.m.share.hesvh.cn/Article/details/gxnspgpxh.sHtML

Go:   end.Sub(start).Hours()
来源：http://m.share.zdbjq.cn/Article/details/gupyukuac.sHtML

Ruby: end - start                 # 返回秒数
来源：http://3g.fehbvm.com/Article/details/gylrhnsyy.sHtML

C#:   (end - start).TotalSeconds
来源：http://wap.fehbvm.com/Article/details/gvpqxyduj.sHtML

[J07] 比较两个日期
来源：http://wap.fehbvm.com/Article/details/gybhnrugf.sHtML

Py:   d1 < d2;  d1 == d2
来源：http://blog.zdbjq.cn/Article/details/gbhrzgwcp.sHtML

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wap.fehbvm.com/Article/details/gsgveneph.sHtML

JS:   d1.getTime() < d2.getTime()
来源：http://read.share.hesvh.cn/Article/details/govithqtg.sHtML

TS:   d1.getTime() < d2.getTime()
来源：http://3g.fehbvm.com/Article/details/gohjmrbtm.sHtML

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.m.share.fehbvm.com/Article/details/gimoiusxa.sHtML

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://blog.zdbjq.cn/Article/details/gnqoqjiwx.sHtML

Ruby: d1 < d2;  d1 == d2
来源：http://3g.zdbjq.cn/Article/details/gofonkkdr.sHtML

C#:   d1 < d2;  d1 == d2
来源：http://m.share.hesvh.cn/Article/details/gjqfphbqd.sHtML

[J08] 提取年月日与星期
来源：http://wap.fehbvm.com/Article/details/gxidgyjkf.sHtML

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://read.share.fehbvm.com/Article/details/gtctacado.sHtML

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.share.zdbjq.cn/Article/details/gcklyxlel.sHtML

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://blog.fehbvm.com/Article/details/gkivcdvhw.sHtML

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.share.zdbjq.cn/Article/details/grqvftsfe.sHtML

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.m.share.zdbjq.cn/Article/details/ggfeljijm.sHtML

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://3g.zdbjq.cn/Article/details/gyknherul.sHtML

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://mobile.fehbvm.com/Article/details/goqnotlbw.sHtML

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://3g.fehbvm.com/Article/details/gjwgsltlc.sHtML

[J09] 时区处理
来源：http://m.share.fehbvm.com/Article/details/gfqbypgjs.sHtML

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.m.share.hesvh.cn/Article/details/gytebdvjr.sHtML

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://baike.hesvh.cn/Article/details/goganvqpv.sHtML

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://read.share.fehbvm.com/Article/details/goohkwvmt.sHtML

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://baike.fehbvm.com/Article/details/gpfebtmgy.sHtML

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://m.share.zdbjq.cn/Article/details/gqeupjdab.sHtML

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://m.share.hesvh.cn/Article/details/gmbwckdgz.sHtML

Ruby: Time.now.getlocal("+08:00")
来源：http://m.share.hesvh.cn/Article/details/grwaklofx.sHtML

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://wap.fehbvm.com/Article/details/guepudyda.sHtML

[J10] 取今天 / 本月第一天
来源：http://mobile.fehbvm.com/Article/details/gedkuipip.sHtML

Py:   date.today();  date.today().replace(day=1)
来源：http://read.share.hesvh.cn/Article/details/gqgnarxor.sHtML

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.share.fehbvm.com/Article/details/gjkrqllup.sHtML

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://3g.fehbvm.com/Article/details/gezcvefny.sHtML

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://baike.zdbjq.cn/Article/details/gbltvlgkk.sHtML

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://m.share.fehbvm.com/Article/details/gmhymdqzi.sHtML

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://wap.fehbvm.com/Article/details/gzedfxlki.sHtML

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://baike.zdbjq.cn/Article/details/gyzbkogxz.sHtML

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gixnuihpw.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gdvymwysl.sHtML

K. JSON 与序列化
来源：http://wap.hesvh.cn/Article/details/gbvlrwoto.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcifxogym.sHtML

[K01] 对象转 JSON 字符串
来源：http://www.share.hesvh.cn/Article/details/gtjccqnti.sHtML

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://3g.hesvh.cn/Article/details/gyipkmvht.sHtML

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://m.share.hesvh.cn/Article/details/gieupsmqz.sHtML

JS:   JSON.stringify(obj)
来源：http://www.blog.fehbvm.com/Article/details/gncmqmhrs.sHtML

TS:   JSON.stringify(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gmpxputkv.sHtML

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://3g.hesvh.cn/Article/details/gcesjuimi.sHtML

Go:   json.Marshal(obj)
来源：http://baike.fehbvm.com/Article/details/gtmiokhef.sHtML

Ruby: obj.to_json                                     // require "json"
来源：http://blog.zdbjq.cn/Article/details/gdrodesof.sHtML

C#:   JsonSerializer.Serialize(obj)
来源：http://m.share.fehbvm.com/Article/details/gverqyaqa.sHtML

[K02] JSON 字符串转对象
来源：http://www.share.hesvh.cn/Article/details/gxdnuxpox.sHtML

Py:   json.loads(s)
来源：http://wap.zdbjq.cn/Article/details/gfhldggdf.sHtML

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://m.share.hesvh.cn/Article/details/ggwungwxy.sHtML

JS:   JSON.parse(s)
来源：http://baike.fehbvm.com/Article/details/giosnhycp.sHtML

TS:   JSON.parse(s)
来源：http://m.share.hesvh.cn/Article/details/gohmohihi.sHtML

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wap.fehbvm.com/Article/details/gblqehwcc.sHtML

Go:   json.Unmarshal(data, &v)
来源：http://www.share.fehbvm.com/Article/details/gpzbsjwqv.sHtML

Ruby: JSON.parse(s)
来源：http://wap.fehbvm.com/Article/details/ghpktvmha.sHtML

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://baike.hesvh.cn/Article/details/gzrxjpatf.sHtML

[K03] JSON 美化输出（带缩进）
来源：http://www.blog.hesvh.cn/Article/details/gqlpliqta.sHtML

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://read.share.zdbjq.cn/Article/details/ggahpxtxd.sHtML

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.m.share.hesvh.cn/Article/details/gkvulaent.sHtML

JS:   JSON.stringify(obj, null, 2)
来源：http://3g.zdbjq.cn/Article/details/gbtriyygo.sHtML

TS:   JSON.stringify(obj, null, 2)
来源：http://blog.fehbvm.com/Article/details/gramwmsbd.sHtML

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://m.share.fehbvm.com/Article/details/gvkcmwilv.sHtML

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.m.share.hesvh.cn/Article/details/gkxfsdrcp.sHtML

Ruby: JSON.pretty_generate(obj)
来源：http://www.m.share.zdbjq.cn/Article/details/gsoepvghk.sHtML

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.blog.hesvh.cn/Article/details/gxrnpatpr.sHtML

[K04] 读取 JSON 文件
来源：http://3g.hesvh.cn/Article/details/gkucifcqt.sHtML

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://read.share.fehbvm.com/Article/details/gbiqvnads.sHtML

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wap.hesvh.cn/Article/details/gwwaudwiv.sHtML

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://3g.hesvh.cn/Article/details/gdmzvvlau.sHtML

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://read.share.zdbjq.cn/Article/details/gxdlclzec.sHtML

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://m.share.zdbjq.cn/Article/details/gtqiyawvx.sHtML

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://blog.fehbvm.com/Article/details/gdspgwynw.sHtML

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.m.share.hesvh.cn/Article/details/gjuacsomy.sHtML

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.share.zdbjq.cn/Article/details/gygibezik.sHtML

[K05] 深拷贝对象
来源：http://wap.hesvh.cn/Article/details/gbbnopola.sHtML

Py:   copy.deepcopy(obj)
来源：http://read.share.zdbjq.cn/Article/details/gtlvpfrsg.sHtML

PHP:  unserialize(serialize($obj));
来源：http://3g.zdbjq.cn/Article/details/gisgzrert.sHtML

JS:   structuredClone(obj)
来源：http://www.m.share.fehbvm.com/Article/details/gcwbdsxyi.sHtML

TS:   structuredClone(obj)
来源：http://m.share.zdbjq.cn/Article/details/gvryksbra.sHtML

Java: // 手写拷贝构造，或序列化往返
来源：http://wap.fehbvm.com/Article/details/guyvjmdtk.sHtML

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://blog.hesvh.cn/Article/details/geshzpwbg.sHtML

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.blog.hesvh.cn/Article/details/gkgfcqkhi.sHtML

C#:   // 序列化往返，或自定义 Clone
来源：http://wap.hesvh.cn/Article/details/gezjswozo.sHtML

[K06] 解析 URL 查询串
来源：http://3g.fehbvm.com/Article/details/gdmfshfqx.sHtML

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://read.share.hesvh.cn/Article/details/gjebhuzsx.sHtML

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.blog.fehbvm.com/Article/details/gqhpwaspb.sHtML

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://baike.zdbjq.cn/Article/details/gjeqrzwdj.sHtML

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.blog.fehbvm.com/Article/details/gygcdadnz.sHtML

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.m.share.fehbvm.com/Article/details/gdmtdoynd.sHtML

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.blog.hesvh.cn/Article/details/gwoyugvwp.sHtML

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mobile.hesvh.cn/Article/details/gzmtskhjt.sHtML

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://m.share.fehbvm.com/Article/details/gqwdozysl.sHtML

[K07] 进制转换
来源：http://www.m.share.hesvh.cn/Article/details/gtqjptqjn.sHtML

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.blog.hesvh.cn/Article/details/gzdxiaxiq.sHtML

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mobile.hesvh.cn/Article/details/gkinodxvn.sHtML

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.m.share.fehbvm.com/Article/details/ggyovlmtg.sHtML

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.m.share.hesvh.cn/Article/details/gbbgejykc.sHtML

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/ghqwtwrad.sHtML

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://3g.fehbvm.com/Article/details/gpvtjyhvh.sHtML

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mobile.hesvh.cn/Article/details/gjoiengsg.sHtML

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.share.zdbjq.cn/Article/details/gzzxatpds.sHtML

[K08] 二进制序列化（非 JSON）
来源：http://www.share.zdbjq.cn/Article/details/gzxjcacuz.sHtML

Py:   pickle.dumps(obj)
来源：http://mobile.zdbjq.cn/Article/details/gllsenewm.sHtML

PHP:  serialize($obj);  unserialize($s);
来源：http://www.share.hesvh.cn/Article/details/gkvlaqqge.sHtML

JS:   v8.serialize(obj)        // Node
来源：http://www.blog.fehbvm.com/Article/details/ggnqsnqrv.sHtML

TS:   v8.serialize(obj)        // Node
来源：http://m.share.fehbvm.com/Article/details/gwxscrfmd.sHtML

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mobile.hesvh.cn/Article/details/gtzuasfln.sHtML

Go:   encoding/gob
来源：http://www.share.fehbvm.com/Article/details/gogwqowzb.sHtML

Ruby: Marshal.dump(obj)
来源：http://blog.zdbjq.cn/Article/details/ggaqslfla.sHtML

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wap.hesvh.cn/Article/details/gqxacjgvd.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gfycpphbx.sHtML

L. 网络请求
来源：http://blog.hesvh.cn/Article/details/gmjsffepi.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gsuywaavj.sHtML

[L01] 发送 GET 请求
来源：http://www.blog.fehbvm.com/Article/details/gzimvcduk.sHtML

Py:   requests.get(url)                        # 第三方库 requests
来源：http://read.share.hesvh.cn/Article/details/gtonicewc.sHtML

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://read.share.zdbjq.cn/Article/details/gnsixngxy.sHtML

JS:   await fetch(url)
来源：http://baike.hesvh.cn/Article/details/ggfagoznv.sHtML

TS:   await fetch(url)
来源：http://www.blog.hesvh.cn/Article/details/gmduyelta.sHtML

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mobile.zdbjq.cn/Article/details/gldpzchuz.sHtML

Go:   resp, err := http.Get(url)
来源：http://baike.zdbjq.cn/Article/details/gufychwsq.sHtML

Ruby: Net::HTTP.get(URI(url))
来源：http://www.blog.fehbvm.com/Article/details/gcqlhfneg.sHtML

C#:   await new HttpClient().GetStringAsync(url)
来源：http://baike.hesvh.cn/Article/details/gxgqztddp.sHtML

[L02] 发送 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gtydkfnpb.sHtML

Py:   requests.post(url, json={"a": 1})
来源：http://wap.hesvh.cn/Article/details/gjivkcjqc.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://blog.fehbvm.com/Article/details/gnoivucmp.sHtML

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.m.share.zdbjq.cn/Article/details/gmarkwzbi.sHtML

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://3g.zdbjq.cn/Article/details/gxosxuxoc.sHtML

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://baike.zdbjq.cn/Article/details/ghmsnqzyh.sHtML

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://3g.fehbvm.com/Article/details/gtxtknykw.sHtML

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.m.share.fehbvm.com/Article/details/gqllsarcw.sHtML

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://3g.hesvh.cn/Article/details/gexsicjxb.sHtML

[L03] 设置自定义请求头
来源：http://baike.hesvh.cn/Article/details/gzlanuhjn.sHtML

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://read.share.zdbjq.cn/Article/details/gmpmfaayt.sHtML

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mobile.hesvh.cn/Article/details/gxvccsoib.sHtML

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wap.hesvh.cn/Article/details/gpwimgfsx.sHtML

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.share.hesvh.cn/Article/details/gozgpbrnh.sHtML

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wap.zdbjq.cn/Article/details/gzzfgqctn.sHtML

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.m.share.zdbjq.cn/Article/details/grxduoill.sHtML

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.m.share.zdbjq.cn/Article/details/gdfhtabtc.sHtML

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mobile.zdbjq.cn/Article/details/gefcixlpp.sHtML

[L04] 设置超时
来源：http://www.m.share.fehbvm.com/Article/details/gxtanqinm.sHtML

Py:   requests.get(url, timeout=5)
来源：http://www.share.zdbjq.cn/Article/details/gzuoyoqpl.sHtML

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.m.share.zdbjq.cn/Article/details/gqgpotuvi.sHtML

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gzjhpflfu.sHtML

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wap.zdbjq.cn/Article/details/gufmtaxku.sHtML

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.m.share.zdbjq.cn/Article/details/gmurzvbgp.sHtML

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://baike.zdbjq.cn/Article/details/gujeyaftk.sHtML

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://blog.fehbvm.com/Article/details/gygjyrecy.sHtML

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.share.hesvh.cn/Article/details/gifwzxzyw.sHtML

[L05] 上传文件（multipart）
来源：http://blog.hesvh.cn/Article/details/geczetsgv.sHtML

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://m.share.hesvh.cn/Article/details/gojtmdjpo.sHtML

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://blog.zdbjq.cn/Article/details/giskrsqeu.sHtML

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://baike.zdbjq.cn/Article/details/gjepuhsye.sHtML

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://blog.zdbjq.cn/Article/details/gtjqvsqnr.sHtML

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.m.share.zdbjq.cn/Article/details/gkcfimmpi.sHtML

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.share.hesvh.cn/Article/details/gwyofvflx.sHtML

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://read.share.fehbvm.com/Article/details/gpotrnumk.sHtML

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gxdrkgooe.sHtML

[L06] 解析响应为 JSON
来源：http://baike.fehbvm.com/Article/details/gsuqycjdi.sHtML

Py:   resp.json()
来源：http://read.share.hesvh.cn/Article/details/gyylkpecb.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.zdbjq.cn/Article/details/gobeqsdqw.sHtML

JS:   await resp.json()
来源：http://www.share.zdbjq.cn/Article/details/gpwghqfjl.sHtML

TS:   await resp.json()
来源：http://blog.zdbjq.cn/Article/details/gbslvadiw.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://3g.zdbjq.cn/Article/details/gcarqmqmu.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mobile.zdbjq.cn/Article/details/gxzkylwen.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.hesvh.cn/Article/details/gyafsqpei.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://m.share.zdbjq.cn/Article/details/glaukzioi.sHtML

[L07] 处理 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gfrwutsbl.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://m.share.fehbvm.com/Article/details/gewhesrfu.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://read.share.fehbvm.com/Article/details/gxtlrtoca.sHtML

JS:   resp.ok;  resp.status
来源：http://baike.fehbvm.com/Article/details/glaidaitj.sHtML

TS:   resp.ok;  resp.status
来源：http://read.share.zdbjq.cn/Article/details/ghfrygsja.sHtML

Java: resp.statusCode()
来源：http://read.share.fehbvm.com/Article/details/gdsrnxcqy.sHtML

Go:   resp.StatusCode
来源：http://m.share.zdbjq.cn/Article/details/grnouqlmh.sHtML

Ruby: resp.code.to_i
来源：http://www.blog.zdbjq.cn/Article/details/gqkgyjojr.sHtML

C#:   (int)resp.StatusCode
来源：http://3g.fehbvm.com/Article/details/glgynhdvp.sHtML

[L08] 并发请求多个地址
来源：http://3g.zdbjq.cn/Article/details/gmylieojp.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.share.zdbjq.cn/Article/details/gfiazklgf.sHtML

PHP:  curl_multi_init() 系列
来源：http://m.share.hesvh.cn/Article/details/ghiiapcvl.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://baike.zdbjq.cn/Article/details/gayqqwtft.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.fehbvm.com/Article/details/gquhzrfkc.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://3g.hesvh.cn/Article/details/gogmhpqvk.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wap.fehbvm.com/Article/details/giwnjoqgj.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.zdbjq.cn/Article/details/gbwhildbx.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://read.share.fehbvm.com/Article/details/gnnzsrsib.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gjomdllor.sHtML

M. 命令行 / 进程 / 环境
来源：http://mobile.hesvh.cn/Article/details/ghyghmtuh.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gpbvrzdws.sHtML

[M01] 读取命令行参数
来源：http://read.share.hesvh.cn/Article/details/gmqbaztjn.sHtML

Py:   sys.argv[1:]
来源：http://m.share.hesvh.cn/Article/details/gqwczbojf.sHtML

PHP:  $argv;  $argc;
来源：http://www.m.share.zdbjq.cn/Article/details/gghaccxtq.sHtML

JS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gmombxbgb.sHtML

TS:   process.argv.slice(2)
来源：http://www.blog.fehbvm.com/Article/details/gtubyphix.sHtML

Java: args 数组（main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/gxbfrwqhk.sHtML

Go:   os.Args[1:]
来源：http://3g.fehbvm.com/Article/details/gvjmngaxg.sHtML

Ruby: ARGV
来源：http://www.share.fehbvm.com/Article/details/gkbljlyft.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.hesvh.cn/Article/details/ghitfbjca.sHtML

[M02] 读取环境变量
来源：http://m.share.fehbvm.com/Article/details/gyncxmqez.sHtML

Py:   os.environ.get("HOME")
来源：http://www.share.zdbjq.cn/Article/details/gglmtsgqa.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://m.share.fehbvm.com/Article/details/ghkbsgzqn.sHtML

JS:   process.env.HOME
来源：http://mobile.hesvh.cn/Article/details/gpkbdyzpe.sHtML

TS:   process.env.HOME
来源：http://blog.hesvh.cn/Article/details/gadqekukp.sHtML

Java: System.getenv("HOME")
来源：http://blog.fehbvm.com/Article/details/gogxyzfkw.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mobile.hesvh.cn/Article/details/gxfzgkxnc.sHtML

Ruby: ENV["HOME"]
来源：http://baike.zdbjq.cn/Article/details/guhtujjjg.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mobile.fehbvm.com/Article/details/gvkirxyle.sHtML

[M03] 执行外部命令
来源：http://www.share.fehbvm.com/Article/details/gtxpvjpnw.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://baike.fehbvm.com/Article/details/goevxwrgq.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wap.hesvh.cn/Article/details/ggldvbqot.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://www.m.share.zdbjq.cn/Article/details/glvvqthfi.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://read.share.hesvh.cn/Article/details/grfivtgjc.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mobile.zdbjq.cn/Article/details/glnkbwubm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://blog.zdbjq.cn/Article/details/gorbfbpfu.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://3g.zdbjq.cn/Article/details/gacvtquok.sHtML

C#:   Process.Start("ls", "-l");
来源：http://www.m.share.zdbjq.cn/Article/details/guyczbaum.sHtML

[M04] 获取当前工作目录
来源：http://read.share.fehbvm.com/Article/details/gqpmmzhrf.sHtML

Py:   os.getcwd()
来源：http://baike.fehbvm.com/Article/details/gkpdqgjvs.sHtML

PHP:  getcwd();
来源：http://www.share.zdbjq.cn/Article/details/grchqiwij.sHtML

JS:   process.cwd()
来源：http://wap.hesvh.cn/Article/details/gftyvuvgi.sHtML

TS:   process.cwd()
来源：http://read.share.hesvh.cn/Article/details/gwoswnkoy.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://m.share.hesvh.cn/Article/details/gklvhgvub.sHtML

Go:   os.Getwd()
来源：http://m.share.zdbjq.cn/Article/details/gkmoclriu.sHtML

Ruby: Dir.pwd
来源：http://3g.fehbvm.com/Article/details/gcuxcdtly.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://blog.fehbvm.com/Article/details/gfsyctuuf.sHtML

[M05] 设置退出码
来源：http://www.blog.zdbjq.cn/Article/details/gouxkaixv.sHtML

Py:   sys.exit(1)
来源：http://3g.hesvh.cn/Article/details/gjqukifei.sHtML

PHP:  exit(1);
来源：http://www.m.share.fehbvm.com/Article/details/glgssdfjo.sHtML

JS:   process.exit(1)
来源：http://blog.zdbjq.cn/Article/details/glnmgqunb.sHtML

TS:   process.exit(1)
来源：http://baike.zdbjq.cn/Article/details/gmwxlbnxr.sHtML

Java: System.exit(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbtfiedut.sHtML

Go:   os.Exit(1)
来源：http://3g.zdbjq.cn/Article/details/gqyvcnyoi.sHtML

Ruby: exit 1
来源：http://www.m.share.fehbvm.com/Article/details/ghcafhlhk.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://blog.zdbjq.cn/Article/details/gfflsoxgf.sHtML

[M06] 向标准错误输出
来源：http://mobile.zdbjq.cn/Article/details/gnynlsfwb.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.blog.hesvh.cn/Article/details/gjnahyxud.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://mobile.zdbjq.cn/Article/details/gwbpzqmjr.sHtML

JS:   console.error("err")
来源：http://m.share.fehbvm.com/Article/details/gmfvfbzft.sHtML

TS:   console.error("err")
来源：http://mobile.fehbvm.com/Article/details/ghigkrefv.sHtML

Java: System.err.println("err")
来源：http://www.blog.hesvh.cn/Article/details/gzemassxx.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mobile.fehbvm.com/Article/details/gmcbwiqbu.sHtML

Ruby: warn "err"
来源：http://www.m.share.fehbvm.com/Article/details/gdoamxrdy.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://www.blog.fehbvm.com/Article/details/guymtjtwl.sHtML

[M07] 判断是否为主入口
来源：http://3g.fehbvm.com/Article/details/gtyafsklg.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.fehbvm.com/Article/details/gsqhjqrgy.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://read.share.fehbvm.com/Article/details/gyfezhogk.sHtML

JS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gnymvfojz.sHtML

TS:   require.main === module
来源：http://baike.fehbvm.com/Article/details/gdxjrituu.sHtML

Java: public static void main(String[] args)
来源：http://3g.fehbvm.com/Article/details/gnugmszhg.sHtML

Go:   func main()
来源：http://blog.zdbjq.cn/Article/details/gzrvmhibj.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.blog.fehbvm.com/Article/details/gvqcecfbq.sHtML

C#:   static void Main(string[] args)
来源：http://www.blog.zdbjq.cn/Article/details/gsjbtowie.sHtML

[M08] 获取系统与运行时信息
来源：http://www.m.share.hesvh.cn/Article/details/gqyfqocmu.sHtML

Py:   platform.system();  platform.python_version()
来源：http://www.m.share.hesvh.cn/Article/details/gvpejqgnu.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.blog.fehbvm.com/Article/details/gaqmkxtgg.sHtML

JS:   process.platform;  process.version
来源：http://mobile.fehbvm.com/Article/details/ggkaltlgt.sHtML

TS:   process.platform;  process.version
来源：http://wap.zdbjq.cn/Article/details/gqxymfgzy.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.hesvh.cn/Article/details/gmazsttaq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.blog.zdbjq.cn/Article/details/ghyyoonka.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://read.share.hesvh.cn/Article/details/gstiszzql.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.hesvh.cn/Article/details/gwgtjcfpv.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gwgvenptb.sHtML

N. 数据结构与算法
来源：http://www.blog.zdbjq.cn/Article/details/gbgcwflxr.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/ghfoppate.sHtML

[N01] 二分查找（有序数组）
来源：http://3g.fehbvm.com/Article/details/gkvdsojhj.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://mobile.hesvh.cn/Article/details/gowtsumia.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mobile.zdbjq.cn/Article/details/gudpgytgx.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://m.share.zdbjq.cn/Article/details/gsmnmifkd.sHtML


<!-- 参考信息 -->