代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3xbapdluz.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3ivupmnmj.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3uzsjwgmf.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3ndmqxyqr.html

TS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3migomblp.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3nymciqho.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3vcjimvab.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mfwmkvbp.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.ydjk.org.cn/Article/details/gt3hcdccjsz.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3djywcxzf.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3prxulcwe.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3qwzfqlmz.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3zmxiolou.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3ywooqddp.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrswflf.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3oeokpbdj.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3caltdsij.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3jwvrnzqh.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3yoiobfgu.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3ecyxdnpm.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3pywbbuei.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3iankjbgq.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3jpwpagzk.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3oexksuqr.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fjizfuhn.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3pztbimvc.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3potfvhxe.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3gwgjhvrs.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt3wupudeor.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3jqsgczsk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3ycymisud.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3wpjdtgus.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3fvujaawl.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3dfarhhli.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jwjxdhyr.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3ulcyqxdy.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3yncxowkx.html

Py:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3xostwekl.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3ilzryxkx.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3mhqqjhrl.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3csxfnaoc.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt3akxkrpdy.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3yofbbufa.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3njwxcpwc.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3qpcjaleu.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt3kzjthcpc.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.ydjk.org.cn/Article/details/gt3ltowmfaj.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3uphtycyn.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt3cqmpowpe.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3vnwxrqsy.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt3ibjppkks.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.ydjk.org.cn/Article/details/gt3qrhsqmfy.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3hmbmhpah.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3cbkbfghp.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3jzfeaxgh.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3axjibpan.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3gzsobejd.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3exrnmnzz.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3pucwzprf.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3gslyyzpd.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.ydjk.org.cn/Article/details/gt3xpteivic.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3grucctzb.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt3bflyzshe.html

[J10] 取今天 / 本月第一天
来源：http://www.52xcode.cn/Article/details/gt3hmpbnwfk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3vetuydsj.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3phdoowpg.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3twkbepwl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mwawhmhw.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3gfnfhmia.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3izcxnhvu.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3qcmbfqbt.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3ktdtpdqy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izyrugai.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3dureofzz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ntxeorxm.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dmnlnftx.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3vmluibbn.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3argknkhj.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3dewzowed.html

TS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3vwnpweuw.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3lwdrqeqv.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rlhghaxh.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3jkhvipbm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3smysgnfo.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3xjxugtcb.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wobuzwes.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3espoqwms.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lkfhaxlz.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3scfmfauf.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3excoskfx.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3ajzunqog.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3jurrblue.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3lzsdbxuv.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3zkarqmde.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3asbepavw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3lmsrtdai.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3krjgndyu.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3wrarmsrj.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3akgktaue.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3iadoxzma.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3fxyohcer.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt3byminiyh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3laosynzz.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3rweyzioq.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt3krslzjid.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3ckoblbta.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3khvacfmq.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3nlpvsbxx.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3wbvvrzuy.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3lssuysyo.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3znfxlxer.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt3himwklyh.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3xchuxfii.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3pqlpuwhx.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3caxsdoyz.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ktzzllvi.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt3vaxgutwr.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3smghasyj.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3gtasjvue.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt3lllztist.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3bebxopja.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3ysboxnbr.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.52xcode.cn/Article/details/gt3gtxambbs.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qsshijdn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3fcsmaoqp.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3bfhwenjj.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mscizejb.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3jefirlbi.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3mbnbaooh.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3kshbtbsc.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jpcjjayw.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt3rsqdcahi.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3sjpoeiki.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3eahayyaf.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3jtmkqmte.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3unufwcox.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3zlzyptnx.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3lvlnpwth.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3qvuzwewp.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3jndbmgbb.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qozytmpu.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3dwaexnqc.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3hefifhjw.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3qnbllxmg.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt3nrsxoqvf.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3nwsvsmmi.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3duhcegut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lestnnap.html

L. 网络请求
来源：http://www.ydjk.org.cn/Article/details/gt3krzaepeo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ihvhkysy.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt3phlkunkk.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3cgvgpnne.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3gmzfxwhh.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3mbkytjdy.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3gecczdww.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt3tgoiykih.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt3kekiewfn.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3aamvvbrb.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3yeypmkne.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3othlehdx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3jwosmuws.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3btnugygc.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3eeoyzahn.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3cdxifvjw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3oamxifhs.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3rdiachin.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3kbdkhqhs.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3rytuvczp.html

[L03] 设置自定义请求头
来源：http://www.ydjk.org.cn/Article/details/gt3lkszbncm.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3xgzzkxpm.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3wywstlwb.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3fghkkqra.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3xexigetw.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3mdbokuic.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3qtwfbjvj.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3mwbscvys.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3pfwuqbuw.html

[L04] 设置超时
来源：http://www.52xcode.cn/Article/details/gt3wgrrcllg.html

Py:   requests.get(url, timeout=5)
来源：http://www.52xcode.cn/Article/details/gt3kyxzpwvx.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3mssnwpsu.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3ugmkruss.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3xbcqrvpe.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3ranfmruc.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3eggesawa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3pugvwdbu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rbhfyyvg.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3pvylnshi.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3sngnjhyd.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkcmaobt.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3pyqdqglb.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3kgzwjrhp.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3ddknorhw.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.ydjk.org.cn/Article/details/gt3osdimvkd.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt3yutlvtim.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3llccexce.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3wmwpjjqq.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3huqnahoe.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ikfjbrls.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3srevtaqm.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3rbxdcrgn.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3btpgpumy.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.52xcode.cn/Article/details/gt3rjqplnak.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3brnbrquc.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3ucqfrjdj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wdrfneye.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt3yshlmsds.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3pnpkuhgy.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3axdvcjca.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3ykrsoyhx.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3frtabgrk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3focirzuq.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt3dngwkzrv.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3rqixgdbu.html

[L08] 并发请求多个地址
来源：http://www.52xcode.cn/Article/details/gt3ddpbpwgk.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3jdndimxl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3dxvcfakz.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3ggxcbzxa.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3ocglakee.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3tpxisrds.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3fhquaorj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3huwcejxs.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3prjgvekg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dhydmizj.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3vrbatukr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzcwpwos.html

[M01] 读取命令行参数
来源：http://www.52xcode.cn/Article/details/gt3itlcpzkm.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3ragbhpsw.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3kwfqkmic.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3sckxfvxy.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3qsuotjrs.html

Java: args 数组（main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3joxlrxzi.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3gteyzpfb.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt3nxbekglb.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3emghqnzq.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3whcquutk.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3tkqjtycw.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3qomnkisi.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3svaqnnsk.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt3hmkzxfkk.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3vfjxfgtf.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3kdzvxbni.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt3blbrirhx.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3zikwathd.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3eeecfcrh.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3nxtrhbkv.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt3oswyqzmu.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oarwyaqx.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3auixhhck.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.52xcode.cn/Article/details/gt3hijjmunp.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3mthxyjbh.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3vyljfhgt.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xvlhkjfy.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt3xbsgjwca.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3krnjwcpa.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3keiydjkh.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3rzdxztcx.html

TS:   process.cwd()
来源：http://www.ydjk.org.cn/Article/details/gt3zehxowfr.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3tugvsofe.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kcwltxxd.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3wtbsrcbq.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt3xljgwbtd.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3utmsxetw.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vgocvowp.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3cfbrhqvw.html

JS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fwqdxxcj.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jyufhkho.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fkbqjiru.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3fcfejvzr.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mwvcuxay.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt3grhmepri.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3fqgzkkcw.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3ohnvwkwo.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3xapgfjyn.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3fcgxbgmq.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3jargzcno.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3zxgxnucg.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3jcurzbcd.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3mmbxbaws.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ozrlfzqq.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt3jmjyjqkn.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3ryasnzbq.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3cjxohsuk.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3rdxfaeus.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt3xtzisuiu.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3ffcbpbud.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt3zrtxwmxq.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3aaiohbfw.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3onbxtqwc.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3jtlyckwc.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3bhkazbzm.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3ybnbfccy.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3lvvowtfz.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3sqtlqmfl.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt3vwxjjwxa.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xgqiuqez.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt3hslsnudc.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3awiywagb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eopsatpy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt3agbisdaw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bsivkqfx.html


<!-- 参考信息 -->