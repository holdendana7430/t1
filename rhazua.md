代发 wailian999

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt2oktozeyk.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2ljwawzki.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2nduuqfuu.html

Ruby: Date.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt2pesggqju.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt2sfgnxdrv.html

[J04] 时间戳与日期互转
来源：http://www.ydjk.org.cn/Article/details/gt2zbvphyiu.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2iszgdyqd.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt2cipszzda.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt2rcgxbbhb.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt2bwmwtkya.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2lswaypjw.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt2yrldmrtl.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt2oiekiayz.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.ydjk.org.cn/Article/details/gt2xswfuuzl.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt2lkakgrrb.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt2kivlkgzn.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt2ehvgtmpz.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt2lfziqzvb.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt2esauaaen.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt2lgksnngt.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kqjgznub.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt2xvncdxlv.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt2jqorwreo.html

[J06] 计算两时间之差
来源：http://www.ydjk.org.cn/Article/details/gt2ehixamew.html

Py:   (end - start).total_seconds()
来源：http://www.ydjk.org.cn/Article/details/gt2mmnltsne.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt2ehbryeum.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.ydjk.org.cn/Article/details/gt2nsojdaiq.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.52xcode.cn/Article/details/gt2hrzbnewg.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt2laieatvo.html

Go:   end.Sub(start).Hours()
来源：http://www.ydjk.org.cn/Article/details/gt2snupqzzc.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt2lxtqdhid.html

C#:   (end - start).TotalSeconds
来源：http://www.52xcode.cn/Article/details/gt2slqzgdvl.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt2mzetgywq.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2irkuqttn.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt2vbysqvwb.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2exhsbkpv.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.ydjk.org.cn/Article/details/gt2hnxvtssh.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.52xcode.cn/Article/details/gt2bcxsfxba.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt2lwmfjvfo.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt2buyssvib.html

C#:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt2hoausxbf.html

[J08] 提取年月日与星期
来源：http://www.52xcode.cn/Article/details/gt2lhzdsgez.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt2xgudzpfc.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt2kygzhywz.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.52xcode.cn/Article/details/gt2gegbhwbq.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt2fzydcmfx.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.52xcode.cn/Article/details/gt2adiiijko.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt2ujidsugx.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt2avzizeka.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.ydjk.org.cn/Article/details/gt2kyudjgxb.html

[J09] 时区处理
来源：http://www.52xcode.cn/Article/details/gt2evzbgaza.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.52xcode.cn/Article/details/gt2aixfppgs.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.ydjk.org.cn/Article/details/gt2avxdckxf.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt2sbnhjtdq.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.ydjk.org.cn/Article/details/gt2lthawjmb.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.ydjk.org.cn/Article/details/gt2zvhhljnj.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt2pgctherc.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.52xcode.cn/Article/details/gt2mfjmmtup.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.ydjk.org.cn/Article/details/gt2byfdmzru.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt2bujonidj.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt2iuchiooo.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt2snuufpru.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.52xcode.cn/Article/details/gt2bavbzyjl.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt2owlcrgsx.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt2jwrnkdia.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.ydjk.org.cn/Article/details/gt2ebxpgzte.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt2zzalirfs.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfobofnt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2andodilz.html

K. JSON 与序列化
来源：http://www.ydjk.org.cn/Article/details/gt2kcaaqcam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2varatzxu.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lkccjuhh.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt2mhlgmdkv.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt2cbrgudbf.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2uhwlplwa.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vbgylykj.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt2wmufunpj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2esnltkry.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt2mylewqgq.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2vcwiqivr.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt2dzypywsv.html

Py:   json.loads(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ppjgkbqu.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.ydjk.org.cn/Article/details/gt2vyeykufm.html

JS:   JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wglntnfb.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2eknnjlpn.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2wvpdjkqh.html

Go:   json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2nsmrsige.html

Ruby: JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt2fpxakljp.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.52xcode.cn/Article/details/gt2socdxsds.html

[K03] JSON 美化输出（带缩进）
来源：http://www.52xcode.cn/Article/details/gt2hmuttwwd.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt2lfdaivaw.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt2bzwdlwlu.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2hxblfiax.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt2ghrbxgmw.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2cvywbhpn.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.52xcode.cn/Article/details/gt2znvytwgb.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.52xcode.cn/Article/details/gt2qjnbtlwd.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.52xcode.cn/Article/details/gt2dbgcvpdh.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt2kslpwcgu.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ojggwyfs.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.ydjk.org.cn/Article/details/gt2wnrkzudm.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2ainpcjfl.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt2niriftrm.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt2wcuavgtz.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.52xcode.cn/Article/details/gt2dosbdcjo.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt2pelfgqej.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.52xcode.cn/Article/details/gt2eqjtkghj.html

[K05] 深拷贝对象
来源：http://www.ydjk.org.cn/Article/details/gt2gehjdoek.html

Py:   copy.deepcopy(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2qywkwkof.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt2ubwqhpgg.html

JS:   structuredClone(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2nguesokm.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt2kdkajjet.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.52xcode.cn/Article/details/gt2iugculbj.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.52xcode.cn/Article/details/gt2rxrwiikd.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt2omgzdpzc.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.52xcode.cn/Article/details/gt2mwhapbzk.html

[K06] 解析 URL 查询串
来源：http://www.ydjk.org.cn/Article/details/gt2xrhttdkc.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2ojiuupaj.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt2uptwjidn.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2nsjpxnjg.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt2mhhxvtom.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.52xcode.cn/Article/details/gt2zjvmhikf.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2ryilnmnm.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt2erjcnrow.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt2lxkehrsj.html

[K07] 进制转换
来源：http://www.ydjk.org.cn/Article/details/gt2clqxyrza.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mwsqlxju.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.ydjk.org.cn/Article/details/gt2gykteodx.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2mfnswfhb.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt2frubgmjo.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2pocyqeci.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt2bweyszqd.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt2bwxyskrz.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt2xcogfsny.html

[K08] 二进制序列化（非 JSON）
来源：http://www.ydjk.org.cn/Article/details/gt2tmrdwbwk.html

Py:   pickle.dumps(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2gjphqhzn.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.52xcode.cn/Article/details/gt2dmsrituv.html

JS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt2ewjivkiv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt2xmvbczrs.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.52xcode.cn/Article/details/gt2xnzfqthx.html

Go:   encoding/gob
来源：http://www.ydjk.org.cn/Article/details/gt2afyzdojj.html

Ruby: Marshal.dump(obj)
来源：http://www.ydjk.org.cn/Article/details/gt2iztfymno.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.52xcode.cn/Article/details/gt2jiwwlzty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jkmbpyjq.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt2lkgtqqsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xgdnxcpq.html

[L01] 发送 GET 请求
来源：http://www.52xcode.cn/Article/details/gt2umjpcjlz.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.ydjk.org.cn/Article/details/gt2dkpcvfbm.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.ydjk.org.cn/Article/details/gt2idprhotc.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2ututnkxb.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt2emylbzng.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.52xcode.cn/Article/details/gt2zuzfccwm.html

Go:   resp, err := http.Get(url)
来源：http://www.52xcode.cn/Article/details/gt2hnidfkzh.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.52xcode.cn/Article/details/gt2ijhmzxff.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt2rzvxzapz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2furjtrzw.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt2vfxbhoml.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.ydjk.org.cn/Article/details/gt2ungqyjyd.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt2fhojbaiu.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt2xznxioiw.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.52xcode.cn/Article/details/gt2atqpcfht.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.ydjk.org.cn/Article/details/gt2xzofhbjo.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt2jhulosmg.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.ydjk.org.cn/Article/details/gt2xqeckeys.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt2mcmscblq.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt2zskblhud.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.ydjk.org.cn/Article/details/gt2pioomtsg.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gqmgnmcf.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt2gimiabyg.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.ydjk.org.cn/Article/details/gt2jbddvbnr.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt2ciysvblp.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt2osygdszg.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt2rzwyvkif.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt2kpvjecpn.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt2avwtyckj.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.52xcode.cn/Article/details/gt2waiddjit.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt2siuebjkb.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.ydjk.org.cn/Article/details/gt2vjdvhclt.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.ydjk.org.cn/Article/details/gt2jpldhggl.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt2wnpqrdsl.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt2oneawktw.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.52xcode.cn/Article/details/gt2txcwoadn.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt2spoahkro.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt2cuaktgnl.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt2fncgpugd.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.52xcode.cn/Article/details/gt2cjyppruy.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt2vdaygumz.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt2nnoyhwig.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt2wlgwfwwy.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.52xcode.cn/Article/details/gt2wqbcxmwp.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vjnlydra.html

[L06] 解析响应为 JSON
来源：http://www.52xcode.cn/Article/details/gt2vktpkysd.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt2wjgjkvze.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt2jvvktpzk.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt2yabrkarx.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt2msuexhkc.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt2ihyavefb.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt2zrlghzhw.html

Ruby: JSON.parse(resp.body)
来源：http://www.ydjk.org.cn/Article/details/gt2itsbyqyi.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt2egkghjzy.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2nbfvmpmk.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.52xcode.cn/Article/details/gt2beffqzsz.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.ydjk.org.cn/Article/details/gt2lcjoaswg.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2bopnassv.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt2yggqfzxu.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt2mpyvbmwk.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt2pcedlrwe.html

Ruby: resp.code.to_i
来源：http://www.ydjk.org.cn/Article/details/gt2qmwzhwrt.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt2ptfgiqbb.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt2uejsjjec.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt2tozrpodi.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt2nytcbvzc.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2vvqzoous.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2apfucxab.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt2laxdieib.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt2jamztaab.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt2igcazdsa.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt2mwcrfzcn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qmgonrxn.html

M. 命令行 / 进程 / 环境
来源：http://www.52xcode.cn/Article/details/gt2quabruxf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyjwvpwk.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vgoniako.html

Py:   sys.argv[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bcdeswsk.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt2bzepdcov.html

JS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2lferxghf.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt2oakjdfyd.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt2ghgrsduf.html

Go:   os.Args[1:]
来源：http://www.52xcode.cn/Article/details/gt2gwncieku.html

Ruby: ARGV
来源：http://www.ydjk.org.cn/Article/details/gt2obcgmrfj.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt2doveygwp.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2vhecgwpf.html

Py:   os.environ.get("HOME")
来源：http://www.52xcode.cn/Article/details/gt2degujxen.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.52xcode.cn/Article/details/gt2lpmcdtto.html

JS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2xxzshgfb.html

TS:   process.env.HOME
来源：http://www.52xcode.cn/Article/details/gt2jyuwituw.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt2xaybbgon.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt2qvipdjnq.html

Ruby: ENV["HOME"]
来源：http://www.ydjk.org.cn/Article/details/gt2wrjhasgn.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt2mqehbmqk.html

[M03] 执行外部命令
来源：http://www.52xcode.cn/Article/details/gt2berhtapp.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.52xcode.cn/Article/details/gt2vgnxqugy.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.52xcode.cn/Article/details/gt2sjzhwknv.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2nrycclsz.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt2tqljlglg.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt2lqtlcsfx.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt2yritbsft.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.ydjk.org.cn/Article/details/gt2psvtowrw.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt2cuqfbejp.html

[M04] 获取当前工作目录
来源：http://www.52xcode.cn/Article/details/gt2pekcbwwi.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt2mtevolmj.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt2ahtuvkub.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2lojjiaiy.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt2fpbqxzzk.html

Java: Path.of("").toAbsolutePath()
来源：http://www.52xcode.cn/Article/details/gt2wsczfrry.html

Go:   os.Getwd()
来源：http://www.52xcode.cn/Article/details/gt2wqwigfqr.html

Ruby: Dir.pwd
来源：http://www.52xcode.cn/Article/details/gt2jeirruod.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.52xcode.cn/Article/details/gt2fuctbdgo.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt2qmptulit.html

Py:   sys.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2ipuburxh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt2svumhqew.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mexofica.html

TS:   process.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2nzzxtrei.html

Java: System.exit(1)
来源：http://www.52xcode.cn/Article/details/gt2jxrdrkgh.html

Go:   os.Exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wamkakwu.html

Ruby: exit 1
来源：http://www.ydjk.org.cn/Article/details/gt2rcsrbepb.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.52xcode.cn/Article/details/gt2jpltkbya.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt2tcwmysgo.html

Py:   print("err", file=sys.stderr)
来源：http://www.52xcode.cn/Article/details/gt2bkoolqej.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt2adxpoxbv.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2qdewhjao.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt2amlyialh.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt2dgfnjtqo.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.52xcode.cn/Article/details/gt2ucewxneu.html

Ruby: warn "err"
来源：http://www.ydjk.org.cn/Article/details/gt2fiqxrooq.html

C#:   Console.Error.WriteLine("err")
来源：http://www.52xcode.cn/Article/details/gt2oesqttgt.html

[M07] 判断是否为主入口
来源：http://www.ydjk.org.cn/Article/details/gt2bfpxyuim.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt2oiapmqbg.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt2xfsqeffh.html

JS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2qwfjzqlj.html

TS:   require.main === module
来源：http://www.52xcode.cn/Article/details/gt2dpudgthr.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt2ciprubex.html

Go:   func main()
来源：http://www.52xcode.cn/Article/details/gt2knxbrxbn.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt2iwdgjnlv.html

C#:   static void Main(string[] args)
来源：http://www.52xcode.cn/Article/details/gt2yqnvjviy.html

[M08] 获取系统与运行时信息
来源：http://www.ydjk.org.cn/Article/details/gt2owtiglre.html

Py:   platform.system();  platform.python_version()
来源：http://www.52xcode.cn/Article/details/gt2lomnzmax.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt2liniwrcu.html

JS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt2aoporuld.html

TS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt2ijozrdxg.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.52xcode.cn/Article/details/gt2buksxctx.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.52xcode.cn/Article/details/gt2jmdetueq.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.52xcode.cn/Article/details/gt2yiaweiju.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt2zdevohpq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bddbwfmy.html

N. 数据结构与算法
来源：http://www.52xcode.cn/Article/details/gt2zaswxpvz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mxzgisoi.html

[N01] 二分查找（有序数组）
来源：http://www.52xcode.cn/Article/details/gt2xkzasrma.html

Py:   bisect.bisect_left(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2iiifqlee.html

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://www.ydjk.org.cn/Article/details/gt2kyovdids.html

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.52xcode.cn/Article/details/gt2flzwsllw.html


<!-- 参考信息 -->