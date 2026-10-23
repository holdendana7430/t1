代发 wailian999

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3cpiuqcsl.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt3stahldlw.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.52xcode.cn/Article/details/gt3qkyrudps.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3roduuuch.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3npclvzqq.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3rxqhbdac.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.52xcode.cn/Article/details/gt3hsfpdwdj.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3pkqjqqvu.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3eysupsle.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3ltnfemtf.html

[J05] 时间加减（加 7 天）
来源：http://www.ydjk.org.cn/Article/details/gt3jdvugfvm.html

Py:   now + timedelta(days=7)
来源：http://www.ydjk.org.cn/Article/details/gt3suafrohz.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.ydjk.org.cn/Article/details/gt3pmivoayy.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3enfiqfgl.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3orhyarjg.html

Java: LocalDate.now().plusDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3myfsywfj.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3drmyoljm.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3vwlkhfqm.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.52xcode.cn/Article/details/gt3ndrhrztv.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt3cknhsupb.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3tdmmnycf.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3fsggsnja.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt3ctqdehzy.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt3eccsatng.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3vryytsit.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3iemkzyit.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3jvzsosxc.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt3eckupcaf.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3qquoxjar.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3erxjlqbk.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.ydjk.org.cn/Article/details/gt3jncthbzk.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3yuekmnop.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt3nrignwbv.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3qpatbitr.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3odlduvky.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3muspfiyw.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3irrrgahb.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3bzhxbryn.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3splzdulc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.ydjk.org.cn/Article/details/gt3awdkjzfw.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3amijjfgm.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.ydjk.org.cn/Article/details/gt3ldojenpj.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3dhtvuvqw.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3ybcljfcu.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.ydjk.org.cn/Article/details/gt3wcbxhxrv.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3qelvbuxq.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3vkvjxjaq.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt3xsqufamt.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt3xmkajled.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt3yqwpggdg.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3vakxklyy.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3reyzfsuk.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3hzsmhgep.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt3qjsqoswo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3ryhwuuhl.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3aenzsiiz.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3irrysntu.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.52xcode.cn/Article/details/gt3qawrwqje.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt3jornljij.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dkntepao.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yuwlyogy.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt3noxaalfk.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3hviynwkc.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.52xcode.cn/Article/details/gt3odkzurbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sfdbchif.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt3nbykfdbu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3glanjwmr.html

[K01] 对象转 JSON 字符串
来源：http://www.52xcode.cn/Article/details/gt3dpvqeclh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3jqsnbczr.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3hriaotrt.html

JS:   JSON.stringify(obj)
来源：http://www.52xcode.cn/Article/details/gt3yjjfwfxo.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3cumfitjn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.52xcode.cn/Article/details/gt3vjgewdmc.html

Go:   json.Marshal(obj)
来源：http://www.52xcode.cn/Article/details/gt3rbadyjcj.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3ujhpxudm.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3deevcyzx.html

[K02] JSON 字符串转对象
来源：http://www.52xcode.cn/Article/details/gt3giairgiz.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnprjgsj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt3dqexokre.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nwjcqdve.html

TS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hrksvxqh.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.52xcode.cn/Article/details/gt3kshelvyh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3emywaqxv.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3fgighjse.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt3cogvfsju.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt3metyxlnp.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3skujkehi.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3cpdqapet.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3eodqaeeb.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3snqkksmu.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ajcqzswa.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt3ulvfvivo.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3rxovqyws.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3gbwnvxdd.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3swomhhhu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3enlisgvt.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3unhzzrxw.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3fjetvhlq.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3mmyejejx.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3qiglynwu.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt3uirbxweg.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3hvieglip.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3raqcwedr.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3xmkroqqg.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3oqfeeeqh.html

PHP:  unserialize(serialize($obj));
来源：http://www.52xcode.cn/Article/details/gt3peqalvab.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3idialifd.html

TS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3bqbgkxpx.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3ilxctlsv.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt3evzmvauh.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3ppkronsf.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3sdqyisug.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt3rssymhkz.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.ydjk.org.cn/Article/details/gt3odkrycte.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3zbgtgoij.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dxgespzg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3osacdpyh.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3erhkucyt.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zeidxaml.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3qyprukmj.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3zfpsxjhf.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3kkfczugs.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3psvpgfke.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3fcxxnqbs.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3tjbikqtf.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3idyvermw.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oladptjl.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.ydjk.org.cn/Article/details/gt3dnremsii.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.ydjk.org.cn/Article/details/gt3cctorugm.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3qntotxnv.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt3qvtonigk.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3ybtvaenl.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt3whndfmps.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3aevqtnca.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3kqfancfj.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt3dapjjqxz.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3ycuvengi.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3mhtirood.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt3yntpgeqa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mbfqduil.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3mspelopc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fquupzkj.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3xxboejhf.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3voppkvqr.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt3qdoqvyxm.html

JS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rmwyaupi.html

TS:   await fetch(url)
来源：http://www.ydjk.org.cn/Article/details/gt3bmlxrecz.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3ioypqrsp.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3jvcmzonk.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt3ybljkrid.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3cosqbqla.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3mnlbsrmy.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3tjfkcnem.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt3trgclrvb.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3uokwkyeg.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3uctjlets.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3thmrsuvi.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3jmotdjtu.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.ydjk.org.cn/Article/details/gt3hazuupao.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt3jhikkdxh.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3irrlmudu.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.ydjk.org.cn/Article/details/gt3wmfbqbvq.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt3qkbgkspp.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3lcwhuvlj.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3uyponegy.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3pehegigt.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3wumjyrob.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.ydjk.org.cn/Article/details/gt3wcwopigy.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3hxttnsbs.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3ludtrpvz.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3daxycmzi.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt3efrahzod.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3zfekuhdp.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt3soflumvy.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3exlksitx.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.ydjk.org.cn/Article/details/gt3ycpxymxa.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3kzgydtlu.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt3yowmlyag.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3gjunmskp.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3lrchqjyl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.ydjk.org.cn/Article/details/gt3dukniort.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt3rryeeltp.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3tahlxrws.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.ydjk.org.cn/Article/details/gt3jesweusi.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3xtduthnv.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3xclkpfyk.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fepglfoy.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gkwlwvfx.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zxuvwlpd.html

PHP:  json_decode($body, true);
来源：http://www.52xcode.cn/Article/details/gt3kngxlobt.html

JS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3kwcjxehx.html

TS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3dgxcpatz.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3psqaugsl.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3msmxufqr.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3nutkkvjt.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3nhdmtxdj.html

[L07] 处理 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3cnvamtmm.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3uvlklmvn.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt3tncfyxxw.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3fcuhgtuf.html

TS:   resp.ok;  resp.status
来源：http://www.ydjk.org.cn/Article/details/gt3gwumfcvb.html

Java: resp.statusCode()
来源：http://www.52xcode.cn/Article/details/gt3yzsnmovw.html

Go:   resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3bbbdjgjb.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3xbmqsqlo.html

C#:   (int)resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3dkpaurfy.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3bkzgqbcv.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.52xcode.cn/Article/details/gt3mzbsghip.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3mlhchfkt.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.52xcode.cn/Article/details/gt3renxxqlv.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oqfgucun.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.52xcode.cn/Article/details/gt3xhkoqbap.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.52xcode.cn/Article/details/gt3lienwlyj.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.52xcode.cn/Article/details/gt3loluxbum.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3oecyrqjb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3piuckqiw.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt3lstlvxjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwkanqyn.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3udlvaaui.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zzdzcuef.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3buvwcppo.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3rmyoisel.html

TS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vxjmqoeq.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vwznmpqm.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt3betmuutj.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3znvrvymg.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3isojxfxt.html

[M02] 读取环境变量
来源：http://www.52xcode.cn/Article/details/gt3qldgskns.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3uwmpjmxz.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3sussqeng.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3ztouauxb.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zzhnswzv.html

Java: System.getenv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3mkcjomjy.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3cnqwsnqq.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3kignmjwk.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3oqppdikp.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt3tzzyqgjm.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3cihmctlf.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3hcqbkrsc.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3tyavjbfy.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xkfwzytt.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3cuzphdph.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.ydjk.org.cn/Article/details/gt3cpshwmnj.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3wgqoldyv.html

C#:   Process.Start("ls", "-l");
来源：http://www.ydjk.org.cn/Article/details/gt3phnunlfj.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3bjtvsxvg.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3kyopytch.html

PHP:  getcwd();
来源：http://www.52xcode.cn/Article/details/gt3lmllhohr.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3oexswfsu.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3pkpslyti.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt3ofuihxcu.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3hzveurqs.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3setwbzrw.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3vnblshbx.html

[M05] 设置退出码
来源：http://www.52xcode.cn/Article/details/gt3macoikdh.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3vrqramvl.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3dhcctaml.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qmuvmjfx.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt3ksethhhp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3djyioesg.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3frhkyrss.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt3mmztrnnt.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3asbjfozn.html

[M06] 向标准错误输出
来源：http://www.ydjk.org.cn/Article/details/gt3aiqrakmi.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt3oxbbnauu.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.52xcode.cn/Article/details/gt3npjiamjw.html

JS:   console.error("err")
来源：http://www.ydjk.org.cn/Article/details/gt3cxdevzcu.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3opiojghq.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3bybfpwmh.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt3mhrodrmk.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt3kobprqfm.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt3slxbjhnp.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3bqnpqmyv.html

Py:   if __name__ == "__main__":
来源：http://www.52xcode.cn/Article/details/gt3lhzsorgt.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3ycriqmqa.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3vjnsjwuo.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3bhdwoiwy.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3jcksgfjt.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3fobpafkj.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.ydjk.org.cn/Article/details/gt3fdxpiuya.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3aooggict.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3yliltnuo.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt3dgtgtabz.html

PHP:  PHP_OS;  phpversion();
来源：http://www.ydjk.org.cn/Article/details/gt3wgocfogh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3jesqkqje.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3xeadriga.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3enckiakq.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt3xufsucph.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3uxamalcp.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3tkiriuqs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sryeryat.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3jmkbugmf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubwfzuwt.html

[N01] 二分查找（有序数组）
来源：http://www.ydjk.org.cn/Article/details/gt3dioayhvn.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3khpyeyun.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.52xcode.cn/Article/details/gt3nxcrxvzo.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3ovpzkawi.html

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt3tprromzb.html

Java: Arrays.binarySearch(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqbmxand.html

Go:   sort.SearchInts(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3tlrhfhgw.html

Ruby: arr.bsearch { |e| e >= x }
来源：http://www.52xcode.cn/Article/details/gt3rxrdjwbw.html


<!-- 参考信息 -->