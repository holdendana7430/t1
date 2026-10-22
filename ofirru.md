代发 wailian999

[J03] 字符串解析为日期
来源：http://www.52xcode.cn/Article/details/gt2xxeldohl.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.ydjk.org.cn/Article/details/gt2dlkgbzfj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.ydjk.org.cn/Article/details/gt2rcwzqeze.html

JS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2hlbdzecv.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2xmstcoxv.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2rxmyvmwq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2jtcehroj.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2butmfwch.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2gizwwxvz.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2dyeupxpj.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt2ltjwugrd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.ydjk.org.cn/Article/details/gt2rvhkrcjl.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2qnpuokei.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2vdzkcqno.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2hmhquvwa.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2uyppneiq.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2aceoucvz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2szptzasj.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2dmfeorcb.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt2lczoxpkw.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt2eyrdgyzt.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2cmopdsst.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2hzprllcd.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2cmauroji.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jpdmtkcd.html

Ruby: Time.now + 7 * 86400
来源：http://www.ydjk.org.cn/Article/details/gt2upjqkepa.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2tnnlhgrq.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2mljmspqk.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2wgjpkjsp.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2fhubzwmg.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt2qienfuis.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2ghjadfwi.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2ozxbjfpv.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2lyxfehlr.html

Ruby: end - start                 # 返回秒数
来源：http://www.ydjk.org.cn/Article/details/gt2wsvflmvo.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2jyylyvma.html

[J07] 比较两个日期
来源：http://www.52xcode.cn/Article/details/gt2sdhiyecj.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2yygtwilz.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2pnprgbjx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2rfmyfxwt.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt2abepxoso.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2hbgobnwe.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.52xcode.cn/Article/details/gt2rwpjbhfs.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2knuhfggp.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2yyvlljgf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2wgoawfqg.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2hnjoenhn.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt2ssumvsee.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2zrtxxybm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2pmjprjxf.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2agxvathx.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt2yiailtve.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2rptkdmkb.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt2yspbapfc.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2oesphxtk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2rvkixteh.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt2povqbetc.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2diyjudzd.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2roccqnod.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2cvoynqjo.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2ifowwpok.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt2etfcmfqo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2bzdrbfdq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2fpgrvqyw.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.52xcode.cn/Article/details/gt2gukrcmmb.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2ccyplkeg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2tucxqmjs.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2zeczzzuk.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2hnuybgad.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2fdgrsfmv.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.52xcode.cn/Article/details/gt2dfudjgcm.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt2qanxvyeh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sggcjdak.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt2dbetdphg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bcognijq.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lscatrax.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2djkakppj.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2ygbyuueb.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt2qdcywrxo.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2wiadrvda.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt2xtlficgx.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uqewkejg.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2kolpzbux.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2auklhete.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt2vvhmuanc.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2riygdndr.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2jztcttap.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wbhfqviw.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2lnguohlv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ydfkkrlc.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2kpcxsiov.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2rfurqtkf.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt2urawhuxb.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt2gnzojcby.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2rsdcoxve.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2yshrtkug.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2estekihh.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2pxyuicyx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.52xcode.cn/Article/details/gt2jowdwbjt.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2hhrlqzsj.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2hvutzpqv.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2ixjymibb.html

[K04] 读取 JSON 文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfmxqzlu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2khtpjdmi.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2dwyreugm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2zchmcqpx.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt2brfhnyjh.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wddvaxot.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt2upgzumfw.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2bvqmbgqs.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2xrszybvc.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt2perbwhps.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt2qhjbkrul.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt2ayiccsab.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2nmvffqpc.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2junbamos.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt2vakoodmw.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2blebcnyv.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.52xcode.cn/Article/details/gt2filkedjg.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt2nfddneos.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt2ugcrhzoh.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2yihaslwe.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2ybggevny.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rwmegkrd.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2ndfnguvi.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2jlytduee.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ladwxlhl.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2beoyfuhi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2vlfrdpya.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2oqzahsjv.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2xrgvuzlq.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2yyotpbmf.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2rvxktixq.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2zakkxrqm.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2qdpsrwde.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt2ojzmxhhk.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt2pbktehxx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2wckqegky.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt2avyntesb.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqcwydl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2gbksgipm.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xvqreaek.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2vfmbnhoh.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2dqiuneeg.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt2apshpmpt.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2xustoumm.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2fnzonxpd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uztujihk.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt2uongctno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qvqtqaxz.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt2rskqfnhc.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2gtwdgrmx.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt2yfvckiey.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt2spodcqqe.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2zrnzlash.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2vaebrzae.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt2nmhmhpxa.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt2spisrvsr.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.ydjk.org.cn/Article/details/gt2peibzmcw.html

[L02] 发送 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xewsvejt.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt2kovtxrco.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2lezadfjd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2ygnbuxie.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2zsziwagb.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2atnohbfo.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt2wsrscndf.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt2sidgnncq.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt2xxrkmcdo.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2musokram.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2vgmcgeah.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2oimjnpxs.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2gkesjdly.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt2ejdwvlog.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2avqypoft.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2tyhndhwi.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt2kpmajdoq.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2hvhslwko.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2qjulruoh.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2mwbjttdp.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt2anyfjdtf.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2lmqmvpzc.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2bgdzpaal.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt2kpzemafn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2zipopbwf.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2ooutcuzo.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt2abnreamu.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2ogqtcvwd.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2wvicsbst.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2wbgonkbg.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2eteynlvn.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2sfcxotjm.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2srlqzzvu.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2vmdnisco.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2ifftfqhe.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hlockeqt.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2bmzmmorz.html

Py:   resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2gmhnfjag.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zyjmvbta.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2vgspsrqx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2hnzhmaoa.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2aiqcuenl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt2tkluzxwr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt2wjvszhtn.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.52xcode.cn/Article/details/gt2qlustvcg.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kyogdmbe.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2msgumqvj.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt2zglketrj.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2sjfhzggz.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt2jmpdwzge.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt2jnzcbocz.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2omachxzi.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2frnviyig.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2jqknrwbp.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt2lomppsuz.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2ksprgbil.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2tnaelbwy.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2arbamfqs.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt2onximflv.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt2bifsdlhw.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2herpendr.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2flmcbpwv.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.52xcode.cn/Article/details/gt2nhdvaqot.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zjpqgomw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2jxoyxwqh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lrhasbdj.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt2unkvizhg.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2pxvazdrg.html

PHP:  $argv;  $argc;
来源：http://www.ydjk.org.cn/Article/details/gt2hcgadkqi.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt2pnbinnzp.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2rnuenmdn.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2bhmkdbvm.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2aylsctcq.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2hgwjywuq.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2yygvqcbk.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2byjuigmw.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2wyobztxm.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt2stlkhrbj.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2qrnsfkqu.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt2dhoomlkk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2fwfprxsa.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2lrxzoojo.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt2ipczyffl.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2jqdgijjp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2oqaykjum.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2rjfmvfyy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt2aqoykdhl.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2umekfesq.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt2jivyigjv.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt2hbgnhczd.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt2qdczuiga.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt2jyrfysoc.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt2kimdhnzv.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt2shozxkye.html

Py:   os.getcwd()
来源：http://www.52xcode.cn/Article/details/gt2fotxufie.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt2pebpsndt.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2mqkstjfb.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ypoushwb.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2cjcwtwzb.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt2ywkhhnnf.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt2ithqwyxd.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2vnmiuchy.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2thyxflxi.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xauukbow.html

PHP:  exit(1);
来源：http://www.ydjk.org.cn/Article/details/gt2oogpfpuk.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hzdagidj.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2klltbroe.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ufforrfa.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt2uldjupkm.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2jpyvytho.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt2kewtxupy.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt2huhlolbl.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt2akcyptpn.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt2xgakbuxc.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt2knwczsan.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2nbkhxwka.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2ydsvibsp.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2wzujbnhq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt2ylgubzxw.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt2uilfvqli.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt2rauiitrd.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt2ymcfvefk.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.52xcode.cn/Article/details/gt2benyfsyb.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2vewinnnk.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt2vsdxbvpk.html

Java: public static void main(String[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2lyvoxkwh.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2cpbjffyl.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2mzxmrwuv.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt2guopfdid.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt2njytglrm.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt2ebnnvxyu.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2yfttywqu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2szscecbf.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2dmisthob.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt2knsutytk.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2ldobjgan.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2tuybupnl.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.52xcode.cn/Article/details/gt2qdibhgvj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eyowitlq.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt2slxgizsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2szdpahrq.html


<!-- 参考信息 -->