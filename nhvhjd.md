代发 wailian999

[J03] 字符串解析为日期
来源：http://www.ydjk.org.cn/Article/details/gt3caqyvzhk.html

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://www.52xcode.cn/Article/details/gt3sagngeav.html

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://www.52xcode.cn/Article/details/gt3pxnitxgu.html

JS:   new Date("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zewddxjt.html

TS:   new Date("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3mqiinvex.html

Java: LocalDate.parse("2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3zlssuxpq.html

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://www.52xcode.cn/Article/details/gt3uholatom.html

Ruby: Date.parse("2024-01-02")
来源：http://www.ydjk.org.cn/Article/details/gt3znrpedud.html

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://www.52xcode.cn/Article/details/gt3yvksdwmk.html

[J04] 时间戳与日期互转
来源：http://www.52xcode.cn/Article/details/gt3kgtddaac.html

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3sdhepkhw.html

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://www.52xcode.cn/Article/details/gt3ujkulmus.html

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://www.52xcode.cn/Article/details/gt3wfzhbmpi.html

TS:   Math.floor(Date.now() / 1000)
来源：http://www.ydjk.org.cn/Article/details/gt3uewnetoe.html

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://www.ydjk.org.cn/Article/details/gt3tqitzgvs.html

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://www.52xcode.cn/Article/details/gt3roojxwei.html

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://www.52xcode.cn/Article/details/gt3eflkknxh.html

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://www.52xcode.cn/Article/details/gt3wpcnujto.html

[J05] 时间加减（加 7 天）
来源：http://www.52xcode.cn/Article/details/gt3hgfluvzo.html

Py:   now + timedelta(days=7)
来源：http://www.52xcode.cn/Article/details/gt3bfpmnwwc.html

PHP:  (new DateTime())->modify("+7 days");
来源：http://www.52xcode.cn/Article/details/gt3rwvgkezi.html

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.ydjk.org.cn/Article/details/gt3iharqaae.html

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://www.52xcode.cn/Article/details/gt3nzjnhkmp.html

Java: LocalDate.now().plusDays(7)
来源：http://www.52xcode.cn/Article/details/gt3flekelhs.html

Go:   time.Now().AddDate(0, 0, 7)
来源：http://www.52xcode.cn/Article/details/gt3nrqorwuh.html

Ruby: Time.now + 7 * 86400
来源：http://www.52xcode.cn/Article/details/gt3hjrroyoz.html

C#:   DateTime.Now.AddDays(7)
来源：http://www.ydjk.org.cn/Article/details/gt3rhppxmoz.html

[J06] 计算两时间之差
来源：http://www.52xcode.cn/Article/details/gt3oqwkkkro.html

Py:   (end - start).total_seconds()
来源：http://www.52xcode.cn/Article/details/gt3keuxytgx.html

PHP:  $end->diff($start)->days;
来源：http://www.52xcode.cn/Article/details/gt3xntuacxk.html

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://www.52xcode.cn/Article/details/gt3clovkfsz.html

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://www.ydjk.org.cn/Article/details/gt3hjrcosfd.html

Java: Duration.between(start, end).toSeconds()
来源：http://www.52xcode.cn/Article/details/gt3cmlmlasz.html

Go:   end.Sub(start).Hours()
来源：http://www.52xcode.cn/Article/details/gt3baiudcvs.html

Ruby: end - start                 # 返回秒数
来源：http://www.52xcode.cn/Article/details/gt3yxhynaqb.html

C#:   (end - start).TotalSeconds
来源：http://www.ydjk.org.cn/Article/details/gt3isviytip.html

[J07] 比较两个日期
来源：http://www.ydjk.org.cn/Article/details/gt3omxfkwob.html

Py:   d1 < d2;  d1 == d2
来源：http://www.ydjk.org.cn/Article/details/gt3nhshopjh.html

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://www.52xcode.cn/Article/details/gt3gkmwhvrm.html

JS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3bhvdcxzu.html

TS:   d1.getTime() < d2.getTime()
来源：http://www.52xcode.cn/Article/details/gt3jhhlhlcz.html

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3aanoccge.html

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://www.ydjk.org.cn/Article/details/gt3omypxquy.html

Ruby: d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3tsctyiil.html

C#:   d1 < d2;  d1 == d2
来源：http://www.52xcode.cn/Article/details/gt3jctwbztk.html

[J08] 提取年月日与星期
来源：http://www.ydjk.org.cn/Article/details/gt3yejhbpey.html

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://www.52xcode.cn/Article/details/gt3qddfdxvl.html

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://www.52xcode.cn/Article/details/gt3edphuuhh.html

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://www.ydjk.org.cn/Article/details/gt3ahncfrvp.html

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://www.52xcode.cn/Article/details/gt3ltqerywi.html

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://www.ydjk.org.cn/Article/details/gt3qmggdied.html

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://www.52xcode.cn/Article/details/gt3nstfohun.html

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://www.52xcode.cn/Article/details/gt3usxjgekd.html

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://www.52xcode.cn/Article/details/gt3okmmarlu.html

[J09] 时区处理
来源：http://www.ydjk.org.cn/Article/details/gt3zfewjvsk.html

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://www.ydjk.org.cn/Article/details/gt3wuadmvpw.html

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://www.52xcode.cn/Article/details/gt3yzkensrg.html

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3mbnekgyf.html

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://www.52xcode.cn/Article/details/gt3zhjigsvl.html

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://www.52xcode.cn/Article/details/gt3ctcveonc.html

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://www.52xcode.cn/Article/details/gt3ntqrklih.html

Ruby: Time.now.getlocal("+08:00")
来源：http://www.ydjk.org.cn/Article/details/gt3ikvitwuo.html

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://www.52xcode.cn/Article/details/gt3xsmvdgcq.html

[J10] 取今天 / 本月第一天
来源：http://www.ydjk.org.cn/Article/details/gt3jtjgrzdk.html

Py:   date.today();  date.today().replace(day=1)
来源：http://www.ydjk.org.cn/Article/details/gt3lxdphpdr.html

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://www.ydjk.org.cn/Article/details/gt3zgavppcy.html

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3dmwiwwui.html

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://www.52xcode.cn/Article/details/gt3forjdbwz.html

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://www.52xcode.cn/Article/details/gt3reuntyut.html

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://www.52xcode.cn/Article/details/gt3stwpfhiz.html

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://www.ydjk.org.cn/Article/details/gt3wvsjutev.html

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://www.ydjk.org.cn/Article/details/gt3arxqzupg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ntoalejw.html

K. JSON 与序列化
来源：http://www.52xcode.cn/Article/details/gt3vilstjul.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzoiidep.html

[K01] 对象转 JSON 字符串
来源：http://www.ydjk.org.cn/Article/details/gt3hhcihykj.html

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://www.52xcode.cn/Article/details/gt3gdwlsekf.html

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://www.ydjk.org.cn/Article/details/gt3vlxwrjgw.html

JS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3zwfqhbba.html

TS:   JSON.stringify(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ghyzqsrn.html

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://www.ydjk.org.cn/Article/details/gt3zspamepj.html

Go:   json.Marshal(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ddthtjrb.html

Ruby: obj.to_json                                     // require "json"
来源：http://www.ydjk.org.cn/Article/details/gt3enhhehae.html

C#:   JsonSerializer.Serialize(obj)
来源：http://www.52xcode.cn/Article/details/gt3ofuicomg.html

[K02] JSON 字符串转对象
来源：http://www.ydjk.org.cn/Article/details/gt3zdpyyldw.html

Py:   json.loads(s)
来源：http://www.52xcode.cn/Article/details/gt3umrwmzwj.html

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://www.52xcode.cn/Article/details/gt3oeqtdxnj.html

JS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3pmgrhvmx.html

TS:   JSON.parse(s)
来源：http://www.52xcode.cn/Article/details/gt3vskbmbvv.html

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://www.ydjk.org.cn/Article/details/gt3voeunqou.html

Go:   json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3hectnttc.html

Ruby: JSON.parse(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vgaqediu.html

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://www.ydjk.org.cn/Article/details/gt3otxrrjqt.html

[K03] JSON 美化输出（带缩进）
来源：http://www.ydjk.org.cn/Article/details/gt3bzkzukbh.html

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://www.ydjk.org.cn/Article/details/gt3cjnetwpa.html

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://www.52xcode.cn/Article/details/gt3xxovvvgc.html

JS:   JSON.stringify(obj, null, 2)
来源：http://www.52xcode.cn/Article/details/gt3qrltyaej.html

TS:   JSON.stringify(obj, null, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3njrmavfx.html

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3ksfrbeuh.html

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://www.ydjk.org.cn/Article/details/gt3ymyxcujc.html

Ruby: JSON.pretty_generate(obj)
来源：http://www.ydjk.org.cn/Article/details/gt3lhtmovne.html

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://www.ydjk.org.cn/Article/details/gt3yegrohpr.html

[K04] 读取 JSON 文件
来源：http://www.52xcode.cn/Article/details/gt3nkfysuwm.html

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://www.ydjk.org.cn/Article/details/gt3lozoepap.html

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://www.52xcode.cn/Article/details/gt3iqijfcvu.html

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.ydjk.org.cn/Article/details/gt3bohsettg.html

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://www.52xcode.cn/Article/details/gt3hzzjuazt.html

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3vxhqvoln.html

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://www.ydjk.org.cn/Article/details/gt3sqahafag.html

Ruby: JSON.parse(File.read("a.json"))
来源：http://www.52xcode.cn/Article/details/gt3xkliukml.html

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://www.ydjk.org.cn/Article/details/gt3ivjvdgaz.html

[K05] 深拷贝对象
来源：http://www.52xcode.cn/Article/details/gt3pfvyylia.html

Py:   copy.deepcopy(obj)
来源：http://www.52xcode.cn/Article/details/gt3khwifuca.html

PHP:  unserialize(serialize($obj));
来源：http://www.ydjk.org.cn/Article/details/gt3wtnffpdr.html

JS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3kbrgbmmk.html

TS:   structuredClone(obj)
来源：http://www.52xcode.cn/Article/details/gt3czwsenwt.html

Java: // 手写拷贝构造，或序列化往返
来源：http://www.ydjk.org.cn/Article/details/gt3oxwsmoev.html

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://www.ydjk.org.cn/Article/details/gt3hwrnuywr.html

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://www.ydjk.org.cn/Article/details/gt3wprmqkyx.html

C#:   // 序列化往返，或自定义 Clone
来源：http://www.ydjk.org.cn/Article/details/gt3dskheaay.html

[K06] 解析 URL 查询串
来源：http://www.52xcode.cn/Article/details/gt3dzugtpeg.html

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3fguuhsox.html

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://www.ydjk.org.cn/Article/details/gt3mmfippfk.html

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cqlihxsn.html

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://www.52xcode.cn/Article/details/gt3wqjsytzx.html

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://www.ydjk.org.cn/Article/details/gt3iwsutsew.html

Go:   url.ParseQuery("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3zwnrnuet.html

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://www.ydjk.org.cn/Article/details/gt3ckwkhagd.html

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://www.52xcode.cn/Article/details/gt3wlonqwwc.html

[K07] 进制转换
来源：http://www.52xcode.cn/Article/details/gt3bqhgqghx.html

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3nmgikmtc.html

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://www.52xcode.cn/Article/details/gt3atutowea.html

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3oizdfwjp.html

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3viaomhua.html

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://www.ydjk.org.cn/Article/details/gt3ffpwwdhg.html

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://www.52xcode.cn/Article/details/gt3iqpxferp.html

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://www.52xcode.cn/Article/details/gt3swjvbfwf.html

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://www.52xcode.cn/Article/details/gt3ahudjral.html

[K08] 二进制序列化（非 JSON）
来源：http://www.52xcode.cn/Article/details/gt3varxuhxe.html

Py:   pickle.dumps(obj)
来源：http://www.52xcode.cn/Article/details/gt3yhpyokrz.html

PHP:  serialize($obj);  unserialize($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fdptqpsq.html

JS:   v8.serialize(obj)        // Node
来源：http://www.ydjk.org.cn/Article/details/gt3qmjopzvv.html

TS:   v8.serialize(obj)        // Node
来源：http://www.52xcode.cn/Article/details/gt3uimriqum.html

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://www.ydjk.org.cn/Article/details/gt3ackhdjfh.html

Go:   encoding/gob
来源：http://www.52xcode.cn/Article/details/gt3vtdflwvm.html

Ruby: Marshal.dump(obj)
来源：http://www.52xcode.cn/Article/details/gt3gnuigggx.html

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://www.ydjk.org.cn/Article/details/gt3bkqeuitu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3smuiskxl.html

L. 网络请求
来源：http://www.52xcode.cn/Article/details/gt3ibkyimxr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ywlmcnwm.html

[L01] 发送 GET 请求
来源：http://www.ydjk.org.cn/Article/details/gt3oycdvoal.html

Py:   requests.get(url)                        # 第三方库 requests
来源：http://www.52xcode.cn/Article/details/gt3ehpyrfpc.html

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://www.52xcode.cn/Article/details/gt3sucvzfxh.html

JS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3rnysdznc.html

TS:   await fetch(url)
来源：http://www.52xcode.cn/Article/details/gt3wgbwemho.html

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://www.ydjk.org.cn/Article/details/gt3txhidfnv.html

Go:   resp, err := http.Get(url)
来源：http://www.ydjk.org.cn/Article/details/gt3rhebbvsw.html

Ruby: Net::HTTP.get(URI(url))
来源：http://www.ydjk.org.cn/Article/details/gt3dmcugmbx.html

C#:   await new HttpClient().GetStringAsync(url)
来源：http://www.52xcode.cn/Article/details/gt3iukppmpz.html

[L02] 发送 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3daxwqezx.html

Py:   requests.post(url, json={"a": 1})
来源：http://www.52xcode.cn/Article/details/gt3qggqkwfv.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://www.52xcode.cn/Article/details/gt3vfmnnfsm.html

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.ydjk.org.cn/Article/details/gt3njijzbzi.html

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://www.52xcode.cn/Article/details/gt3auyuqyth.html

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://www.ydjk.org.cn/Article/details/gt3uoemxvig.html

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://www.52xcode.cn/Article/details/gt3gnqxhexz.html

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://www.52xcode.cn/Article/details/gt3yaqcmsmu.html

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://www.52xcode.cn/Article/details/gt3vsmqhgoq.html

[L03] 设置自定义请求头
来源：http://www.52xcode.cn/Article/details/gt3ipiizecd.html

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://www.52xcode.cn/Article/details/gt3tavejenn.html

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://www.52xcode.cn/Article/details/gt3ktliwcow.html

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.52xcode.cn/Article/details/gt3uoxiganm.html

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://www.ydjk.org.cn/Article/details/gt3myfxomjz.html

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://www.52xcode.cn/Article/details/gt3tgzhwkkd.html

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://www.ydjk.org.cn/Article/details/gt3doqdkadm.html

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://www.52xcode.cn/Article/details/gt3gvnlqnuw.html

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://www.52xcode.cn/Article/details/gt3zzyrncao.html

[L04] 设置超时
来源：http://www.ydjk.org.cn/Article/details/gt3zskkwqbu.html

Py:   requests.get(url, timeout=5)
来源：http://www.ydjk.org.cn/Article/details/gt3jglywzuu.html

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://www.ydjk.org.cn/Article/details/gt3buayeyqw.html

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3aboohsoo.html

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://www.52xcode.cn/Article/details/gt3prerkrvn.html

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://www.52xcode.cn/Article/details/gt3wntblsfn.html

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://www.52xcode.cn/Article/details/gt3ssokythg.html

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://www.52xcode.cn/Article/details/gt3yzybwwhc.html

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://www.ydjk.org.cn/Article/details/gt3orucoqlc.html

[L05] 上传文件（multipart）
来源：http://www.52xcode.cn/Article/details/gt3bnemazvc.html

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://www.ydjk.org.cn/Article/details/gt3sxhsncnr.html

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://www.52xcode.cn/Article/details/gt3jjntpupi.html

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3zqiyejjo.html

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://www.ydjk.org.cn/Article/details/gt3lapapgyj.html

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://www.52xcode.cn/Article/details/gt3rpfehotf.html

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://www.52xcode.cn/Article/details/gt3uxpmzexo.html

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://www.ydjk.org.cn/Article/details/gt3zffbtyas.html

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qmbeundp.html

[L06] 解析响应为 JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jpetoxds.html

Py:   resp.json()
来源：http://www.52xcode.cn/Article/details/gt3zuisnhxh.html

PHP:  json_decode($body, true);
来源：http://www.ydjk.org.cn/Article/details/gt3tczivswa.html

JS:   await resp.json()
来源：http://www.52xcode.cn/Article/details/gt3wrmoxdrs.html

TS:   await resp.json()
来源：http://www.ydjk.org.cn/Article/details/gt3nbmretya.html

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://www.52xcode.cn/Article/details/gt3ldihtvvo.html

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.ydjk.org.cn/Article/details/gt3okwhroue.html

Ruby: JSON.parse(resp.body)
来源：http://www.52xcode.cn/Article/details/gt3qxltuvrr.html

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://www.ydjk.org.cn/Article/details/gt3dmlwxolh.html

[L07] 处理 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3phbcpaml.html

Py:   resp.status_code;  resp.raise_for_status()
来源：http://www.ydjk.org.cn/Article/details/gt3ymrdmjqw.html

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://www.52xcode.cn/Article/details/gt3sbkklpgp.html

JS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3svthfgec.html

TS:   resp.ok;  resp.status
来源：http://www.52xcode.cn/Article/details/gt3nluqivtb.html

Java: resp.statusCode()
来源：http://www.ydjk.org.cn/Article/details/gt3nuutfshd.html

Go:   resp.StatusCode
来源：http://www.52xcode.cn/Article/details/gt3hvadjgsh.html

Ruby: resp.code.to_i
来源：http://www.52xcode.cn/Article/details/gt3pisdrcsm.html

C#:   (int)resp.StatusCode
来源：http://www.ydjk.org.cn/Article/details/gt3qmgqjkei.html

[L08] 并发请求多个地址
来源：http://www.ydjk.org.cn/Article/details/gt3udgsqaby.html

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.ydjk.org.cn/Article/details/gt3btrlnpfl.html

PHP:  curl_multi_init() 系列
来源：http://www.52xcode.cn/Article/details/gt3fmyorrqe.html

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3vlymcjch.html

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3utrlhcaa.html

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://www.ydjk.org.cn/Article/details/gt3ojlvfmui.html

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.ydjk.org.cn/Article/details/gt3baprhdqq.html

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://www.ydjk.org.cn/Article/details/gt3olijgidw.html

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.ydjk.org.cn/Article/details/gt3uvrqnhqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zrpfgkkn.html

M. 命令行 / 进程 / 环境
来源：http://www.ydjk.org.cn/Article/details/gt3jvpuscwb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sloboszo.html

[M01] 读取命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3pusivnmi.html

Py:   sys.argv[1:]
来源：http://www.52xcode.cn/Article/details/gt3cnmddlrb.html

PHP:  $argv;  $argc;
来源：http://www.52xcode.cn/Article/details/gt3eqravcbl.html

JS:   process.argv.slice(2)
来源：http://www.ydjk.org.cn/Article/details/gt3vwxicsqh.html

TS:   process.argv.slice(2)
来源：http://www.52xcode.cn/Article/details/gt3gxmfapdp.html

Java: args 数组（main 方法参数）
来源：http://www.52xcode.cn/Article/details/gt3vdffyebb.html

Go:   os.Args[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ldpvozxd.html

Ruby: ARGV
来源：http://www.52xcode.cn/Article/details/gt3hhjdiqnv.html

C#:   args 数组（Main 方法参数）
来源：http://www.ydjk.org.cn/Article/details/gt3kkexqtvg.html

[M02] 读取环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3izgusygd.html

Py:   os.environ.get("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3onqzbblq.html

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://www.ydjk.org.cn/Article/details/gt3fkhghtum.html

JS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3cnwfhfza.html

TS:   process.env.HOME
来源：http://www.ydjk.org.cn/Article/details/gt3zpcuieme.html

Java: System.getenv("HOME")
来源：http://www.ydjk.org.cn/Article/details/gt3cadykaoj.html

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://www.52xcode.cn/Article/details/gt3srxuvyif.html

Ruby: ENV["HOME"]
来源：http://www.52xcode.cn/Article/details/gt3rltkpdhw.html

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://www.52xcode.cn/Article/details/gt3kdbfxvrm.html

[M03] 执行外部命令
来源：http://www.ydjk.org.cn/Article/details/gt3orugcskf.html

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://www.ydjk.org.cn/Article/details/gt3mxycmjpp.html

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://www.ydjk.org.cn/Article/details/gt3efzdddeb.html

JS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3trfmaume.html

TS:   child_process.execSync("ls -l").toString()
来源：http://www.52xcode.cn/Article/details/gt3ghynbbog.html

Java: new ProcessBuilder("ls", "-l").start()
来源：http://www.ydjk.org.cn/Article/details/gt3veagpdaa.html

Go:   exec.Command("ls", "-l").Output()
来源：http://www.52xcode.cn/Article/details/gt3xipmtnwr.html

Ruby: system("ls -l");  `ls -l`
来源：http://www.52xcode.cn/Article/details/gt3dtvhwyhk.html

C#:   Process.Start("ls", "-l");
来源：http://www.52xcode.cn/Article/details/gt3xbwfnmhr.html

[M04] 获取当前工作目录
来源：http://www.ydjk.org.cn/Article/details/gt3gxzwcvrh.html

Py:   os.getcwd()
来源：http://www.ydjk.org.cn/Article/details/gt3bijnbqwe.html

PHP:  getcwd();
来源：http://www.ydjk.org.cn/Article/details/gt3inwgpoxn.html

JS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3aonqrukc.html

TS:   process.cwd()
来源：http://www.52xcode.cn/Article/details/gt3xwlnkbeg.html

Java: Path.of("").toAbsolutePath()
来源：http://www.ydjk.org.cn/Article/details/gt3mbijhfeg.html

Go:   os.Getwd()
来源：http://www.ydjk.org.cn/Article/details/gt3rfzyqemn.html

Ruby: Dir.pwd
来源：http://www.ydjk.org.cn/Article/details/gt3nnzbkrrl.html

C#:   Directory.GetCurrentDirectory()
来源：http://www.ydjk.org.cn/Article/details/gt3yzzydzmb.html

[M05] 设置退出码
来源：http://www.ydjk.org.cn/Article/details/gt3hrmaioat.html

Py:   sys.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eetjqlgh.html

PHP:  exit(1);
来源：http://www.52xcode.cn/Article/details/gt3stzeyxdw.html

JS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3obisvjtz.html

TS:   process.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3palgugbp.html

Java: System.exit(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ihptxbdu.html

Go:   os.Exit(1)
来源：http://www.52xcode.cn/Article/details/gt3kcxgbmvx.html

Ruby: exit 1
来源：http://www.52xcode.cn/Article/details/gt3scxqerin.html

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://www.ydjk.org.cn/Article/details/gt3pzjfugzo.html

[M06] 向标准错误输出
来源：http://www.52xcode.cn/Article/details/gt3jrwxwozd.html

Py:   print("err", file=sys.stderr)
来源：http://www.ydjk.org.cn/Article/details/gt3lxzirxvt.html

PHP:  fwrite(STDERR, "err\n");
来源：http://www.ydjk.org.cn/Article/details/gt3edorlhqr.html

JS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3zoaxsywr.html

TS:   console.error("err")
来源：http://www.52xcode.cn/Article/details/gt3qiigdfwa.html

Java: System.err.println("err")
来源：http://www.ydjk.org.cn/Article/details/gt3gobqmgrd.html

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.ydjk.org.cn/Article/details/gt3xtpezmzq.html

Ruby: warn "err"
来源：http://www.52xcode.cn/Article/details/gt3ldiqgyak.html

C#:   Console.Error.WriteLine("err")
来源：http://www.ydjk.org.cn/Article/details/gt3ffgonwav.html

[M07] 判断是否为主入口
来源：http://www.52xcode.cn/Article/details/gt3ygekbjor.html

Py:   if __name__ == "__main__":
来源：http://www.ydjk.org.cn/Article/details/gt3okogmkgc.html

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://www.ydjk.org.cn/Article/details/gt3kignunpw.html

JS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3terehgac.html

TS:   require.main === module
来源：http://www.ydjk.org.cn/Article/details/gt3rrkhayqv.html

Java: public static void main(String[] args)
来源：http://www.52xcode.cn/Article/details/gt3iblxeehc.html

Go:   func main()
来源：http://www.ydjk.org.cn/Article/details/gt3waitkqqt.html

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.52xcode.cn/Article/details/gt3meormbgi.html

C#:   static void Main(string[] args)
来源：http://www.ydjk.org.cn/Article/details/gt3imhkhqxr.html

[M08] 获取系统与运行时信息
来源：http://www.52xcode.cn/Article/details/gt3mykcyavo.html

Py:   platform.system();  platform.python_version()
来源：http://www.ydjk.org.cn/Article/details/gt3khmwpvyw.html

PHP:  PHP_OS;  phpversion();
来源：http://www.52xcode.cn/Article/details/gt3ejapmuhh.html

JS:   process.platform;  process.version
来源：http://www.ydjk.org.cn/Article/details/gt3qokxbsyb.html

TS:   process.platform;  process.version
来源：http://www.52xcode.cn/Article/details/gt3pjlvrled.html

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://www.ydjk.org.cn/Article/details/gt3vxxergfu.html

Go:   runtime.GOOS;  runtime.Version()
来源：http://www.ydjk.org.cn/Article/details/gt3cxopihbx.html

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.ydjk.org.cn/Article/details/gt3vdxijaor.html

C#:   Environment.OSVersion;  Environment.Version
来源：http://www.ydjk.org.cn/Article/details/gt3oceojgki.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3odpspprx.html

N. 数据结构与算法
来源：http://www.ydjk.org.cn/Article/details/gt3bogxzyzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pvlxnbrv.html


<!-- 参考信息 -->